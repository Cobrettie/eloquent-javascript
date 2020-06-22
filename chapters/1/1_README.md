# Ah yes, Chapter One. We begin with values, types, and operators

In this chapter, we will take a deeper dive into value types, and the operators we can perform on those values. 

## Values 

In the computer's world, there is only data. We as humans, are simply viewing that data. Every single thing you see on a computer screen, is data.

As humans, we can do many things with that data, such as reading, modifying, creating new data, etc.

Well how does the computer know what we are requesting?

Every action produces bits. Bits are what your computer needs to display data. 

Bits are any kind of two-valued things, such as zeros and ones. Any piece of discrete information can be reduced to a sequence of zeroes and ones and represented in bits.

Numbers, letters, mouse/keyboard events, any single thing you can do on a computer, can be reduced to bits. It's an extremely complex world behind the scenes of the computer.

A typical modern computer has more than 30 billion bits in its working memory!

That's not really feasible to work with. To be able to work with so many bits, and not get lost, JavaScript separates the bits into chunks, and those chunks represent pieces of information.

Those chunks are called **values**. ALL **Values** are made entirely of bits. Each value can play a different role. Some values are numbers, some values are strings(letters), some are functions, and so on.


## Value Types

### Numbers

You guessed it. Number value types are numeric values. 13, 27, -986, 18.84, are all examples of numbers, and are all represented as bits. JavaScript uses a fixed number of bits to define ANY numeric value.

The main thing to do with numbers, is arithmetic. 

#### Arithmetic Operators

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