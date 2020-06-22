## Arithmetic Operators

The main thing to do with numbers, is arithmetic. 

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


## Unary Operators

A unary operator is just an operator that takes one value.

A binary operator is an operator that takes two values.

Not all operators are symbols, some are written as words.

### Examples of Unary Operators

#### typeof

The *typeof* operator, which names the type of the value you give it
```
console.log(typeof(4));
// number

console.log(typeof('Hey friend'));
// string
```

#### not

The not operator is written as !

An exclamation point? You may be wondering. Yes, exactly an exclamation point. 

The not operator flips the value given to it
```
console.log(!true);
// false

console.log(!false);
//true
```

## Logical Operators

JavaScript supports three *logical operators*
- and
  - represents logical *and*
  - binary operator
  - only returns true when both values given are true
- or
  - represents logical *or*
  - binary operator
  - returns true when at least one value given is true
- not
  - represents logical *not*
  - unary operator
  - returns a flipped value of value given

### Conditional/Ternary Operator

The conditional/ternary operator operates on three given values
- The first value given will determine which of the other two values will be returned
- The second value given will be returned if the first value is true
- The third value given will be returned if the first value is false
- Of the second and third values, only the value selected will be evaluated
```
console.log(true ? 1 : 2);
// returns 1

console.log(false ? 1 : 2);
// returns 2
```


