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
let testString2 = "Hey I am also a string!'
let testString3 = `Hey I am an invalid string! Why?"
```