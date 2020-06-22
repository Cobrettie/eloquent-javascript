# Value Types

## Numbers

You guessed it. Number value types are numeric values. 13, 27, -986, 18.84, are all examples of numbers, and are all represented as bits. JavaScript uses a fixed number of bits to define ANY numeric value.

The main thing to do with numbers, is arithmetic. 

### Arithmetic Operators

- addition (+)
- subtraction (-)
- multiplication (*)
- division (/)
- remainder of (%) 
- remainder of (%) is often referred to as *modulo*

These are self explanatory, however, the % operator will return the remainder of the division of two numbers
```
100 % 2 = 0
314 % 100 = 14 
```
- The remainder of 100 / 2 is 0
- The remainder of 314 / 100 is 14

### Special Numbers

There are three special values in JavaScript that are considered numbers, they just don't behave like normal numbers

- Infinity (The positive representation of infinity)
- -Infinity (The negative representation of infinity)
- NaN (Not a Number)
  - although NaN is returned when calculating operations that don't return a meaningful result, NaN still is a value of the number type


## Strings

Our next basic data type is the string. Strings are used to represent text! It's that simple.

Strings are written by enclosing their content in quotes. You can use single quotes(' '), double quotes(" "), or backticks (` `) to define strings, as long as you use the same quote at the beginning/end of the string.

```
let testString = 'Hey I am a string!'
let testString2 = "Hey I am also a string!"
let testString3 = `Hey I am an invalid string! Why?"
```

Strings are, you guessed it, bits. At the deepest root of any data, is a sequence of bits, allowing the computer to decipher the data.

You can add strings together using +
```
let string1 = "String 1 ready for duty, ";

let string2 = "and my buddy String 2 is right next to me";

let joinedStrings = string1 + string2;

console.log(joinedStrings);
// returns "String 1 ready for duty, and my buddy String 2 is right next to me"
```

You can do many other things with strings. As you need, research further. For now, fundamentals are key.


## Boolean Values

A *boolean type* has only two possibilities. True or False. Nothing more, nothing less.

It's that simple. A boolean is either true or false.

A quick example
```
console.log(3 > 2);
// true

console.log(10 > 20);
// false
```

A boolean is basically saying 'yes, this is true', or 'no, this is false'