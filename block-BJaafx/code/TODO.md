1. Using loops take 10 inputs from user and find the average of all the numbers.

```js
let sum = 0 ;
for (i = 1 ; i <= 10 ; i++){
  let number = +prompt("Enter Number")
  sum = sum + number ;
}  
let average = sum / 10 ;
alert (`Average of 10 number is ${average}`) ;
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}

// println is not defined
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

```js
function getEvenSum (max = 10){
let evenSum = 0 ;
for (i = 2 ; i <= max ; i++){
  if (i % 2 === 0){
    evenSum = evenSum + i
  }
}
return evenSum ;
}
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

```js
function getOddSum (max = 10){
let OddSum = 0 ;
for (i = 1 ; i <= max ; i++){
  if (i % 2 !== 0){
    OddSum = OddSum + i
  }
}
return OddSum ;
}
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

```js
function getProductOfDigits (num){
  let product = 0 ;
  while (num > 0){
    let lastDigit = num % 10;
    product = product + lastDigit;
    num = Math.floor (num / 10);
  }
  return product ;
}
```

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // 'Bigger than 5'
check(1); // 'Smaller than 5'
check(5); // 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // 'You are arya'  
getOutput('John'); // 'You are john'
getOutput(); // 'Who are you'

// once it execut return it will come out of function {}
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // console (You are arya) and return ('Who are you')
getOutput('John'); // console (You are john) and  ('Who are you')
getOutput(); // 'Who are you'

// it will return 'Who are you' in each case and when if condition executed it will console it
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

Yes , function can have multiple return statement
```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

// function can have multiple return statement but it will execut only one return .
```

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

We should use `while` loop when we only have condition.
```js
let i = +prompt("Enter number")
while (i < 10){
  console.log (i);
  i = i + 1
}
```

We should use `for` loop when we have initial value , final value and what to do after each iteration.
```js
let n = +prompt("Enter number")
for (i = 0 ; i < n ; i++ ){
  console.log (i);
}
```