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

### The Breakdown

So let's break down what we are doing here. The challenge is asking us to create a grid, and log it to the console. Easy enough, right?

For this problem, I am using a top-bottom approach for explaining. 

First things first. We already know our grid needs to be exactly 8x8. 8 characters by 8 characters. Our grid only needs to be logged to the console **once**, remember that. 

How do we ensure our grid remains 8x8? With our code!

Lets first initialize a variable **size**, and give it a value of 8, since our grid size is 8x8.

<!-- If you're wondering why not two variables with a value of 8, it's simply because our grid has equal dimensions. If it were 10x8, 14x23, or any other unequal dimensions, we would have two separate variables to hold the values. -->

Next, let's initialize our actual 'grid'. You'll see mine named **string**, a better name for this value is **board** or **grid**, since this is our actual grid that we will log to the console. In my refactor, you will notice the difference.

Everything is rolling smoothly. Great!

Now for the fun part. Let's start looping!

Why looping? Well, you need to log different characters, for different conditions, and you need to do this repeatedly. Sounds like a loop could come in handy!

Onward! 

Those of you eagle-eyed scouts will notice the nested for loop. Good eye, friend!

In short, one loop is for the length of the grid, the second loop is for the width of the grid.

With that information alone, you could come pretty close to a working solution, if not solved completely.

Loop one. Creating a counter, as long as the counter is less than **size**(8), keep counting. 
- The logic in this loop is simple. After loop two has ran its course, add a *newline* character to the grid.

Loop two. Create your counter, if count is less than **size**(8), keep counting. This loop has a bit more juicy logic. Nothing crazy though! You already know what's happening here, just break it down. 
- First, we are going to check some conditions. if statement? Yes! 
  - Add **a** and **b**. If the value of **a** + **b** divides by 2 evenly, add a space to **string**. If the value does not divide by 2 evenly, add a # to our **string**.

At this point, if your code is written properly, you should have a working solution!