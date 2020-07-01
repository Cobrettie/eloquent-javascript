# FizzBuzz

Write a program that uses *console.log* to print all numbers from 1 to 100, with two exceptions.
- For numbers divisible by 3, print "Fizz" instead of the number
- For numbers divisible by 5(and not 3), print "Buzz" instead of the number

When you have that working, modify your program to print "FizzBuzz" for numbers that are divisible by both 3 and 5. Still print "Fizz" or "Buzz" for numbers only divisible by either 3 or 5.

## My Solution
```
for (let number = 1; number <= 100; number ++) {
  if (number % 3 === 0 && number % 5 === 0) {
    console.log("FizzBuzz", number);
  } else if (number % 3 === 0) {
    console.log("Fizz", number);
  } else if (number % 5 === 0) {
    console.log("Buzz", number);
  } else {
    console.log(number);
  }
}
```

## Refactored My Solution
```
for (let n = 1; n <= 100; n++) {
  let output = "";
  if (n % 3 == 0) output += "Fizz";
  if (n % 5 == 0) output += "Buzz";
  console.log(output || n);
}
```

## Eloquent JS Solution
```
for (let n = 1; n <= 100; n++) {
  let output = "";
  if (n % 3 == 0) output += "Fizz";
  if (n % 5 == 0) output += "Buzz";
  console.log(output || n);
}
```

I know, my refactored solution IS the *E JS* solution. I love how concise their solution is, so I refactored mine from scratch and came up with the same solution. I used a similar naming convention because I see this naming convention used *a lot* when dealing with these types of problems