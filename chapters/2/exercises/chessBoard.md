# Chessboard

Write a program that creates a string that represents an 8x8 grid, using newline characters to separate lines. At each portion of the grid, there is either a space or a # character. The characters should form a chessboard. Passing this string to *console.log* should show something like this
```
 # # # #
# # # # 
 # # # #
# # # # 
 # # # #
# # # # 
 # # # #
# # # # 
```

## My Solution

```
let size = 8;
let string = '';

for (let a = 0; a < size; a++) {
  for (let b = 0; b < size; b++) {
    if ((a + b) % 2 == 0) {
      string += ' ';
    } else {
      string += '#';
    }
  }
  string += '\n';
}
console.log(string);
```

So let's break down what we are doing here. The challenge is asking us to create a grid, and log it to the console. Easy enough, right?

For this problem, I am using a top-bottom approach for explaining. 

First things first. We already know our grid needs to be exactly 8x8. 8 characters by 8 characters. It only needs to be logged to the console **once**, remember that. 

How do we ensure our grid remains 8x8? With our code!

Lets first initialize a variable **size**, and give it a value of 8


