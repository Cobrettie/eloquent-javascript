# Chapter Two. Please, allow me to express meaningful prose, and do some *real* programming


# Expressions and Statements

What is an **expression**?
- any fragment of code that produces a value, is called an **expression**
- Every value that is written literally is an **expression**
```
let value = 22;

let test = (value * 2) * 2;
```

What is a **statement**?
- a **statement** is a list of instructions
- Think of an *expression* as a sentence fragment, and a *statement* as the entire sentence.
```
function tellTime() {
  return Date.now();
};
```


# Bindings

Our programs are full of values. JavaScript provides us with a way to store and hold values. 

**Binding**, or a **Variable**

*Binding* basically means assigning a value to something
```
let ten = 10;
console.log(ten * ten)
// 100
// we are binding the value 10 to ten
```

### Binding Names
- Can be any word that is not a reserved keyword in JavaScript
- Can contain numbers, but not *begin* with a number
- Can contain dollar sign $ or underscore _ but no other punctuation or special characters
- camelCase is usually used

### Binding Tips
- The '=' operator can be used to disconnect the binding from a value, and point the binding to a new value
```
let mood = 'bright';
console.log(mood);
// 'bright'

let mood = 'sunny'
console.log(mood);
// 'sunny'
```
- Imagine *bindings* as tentacles, not boxes
  - *bindings* grasp values, not contain them
  - if you need to remember a value in your program, "grow a tentacle" to grasp that value, or assign the value to a current binding
- two or more bindings can point to the same value
- empty binding === undefined
- you can use *var*, *let*, *const* to create bindings
- useful for tracking state in your program

### The Environment
The collection of bindings and their values at a given time, is called the **environment**


# Functions
Functions are special values that encapsulate a piece of a program

### Function Tips
- function is a piece of a program, wrapped in a value
  - those values can be applied, to run the wrapped function
```
prompt("Enter passcode");
// the binding *prompt* holds a function, that when invoked will make a dialog box appear on screen
```
- executing a function is called *invoking*, *calling*, *applying* it
- execute a function by putting parenthesis after an expression that produces a function value
```
invokedFunction('argument1', 'argument2', 'etc');
```
  - notice the strings inside of the parentheses?
  - each comma separated value is called an *argument*, which is a value given to the function


# Control Flow
When your program contains more than one statement, those statements are executed from top to bottom

You can interrupt the normal control flow with
- if/else, switch conditional statements
- looping (while, do, for) statements


# while and do loops

## while loop

**loop** === running a piece of code multiple times

while loop runs the expressions in curly braces repeatedly as long as condition given in parentheses returns true

create a **while** loop
- begin a statement with *while*
- put condition inside of parentheses
- finish statement in curly braces
```
let result = 1;
let counter = 0;

while (counter < 10) {
  result = result * 2;
  counter = counter + 1;
}

console.log(result);
// 1024
```

- Lets look at the above while loop
  - our program initially runs, condition in parentheses is true, expressions in curly braces run
  - since this is a while loop, our program is going to run repeatedly until the condition in the parentheses returns false

If the condition in the while loop parenthesis initially returns false, the expressions in the curly braces will never run

## do loop
Similar to a while loop, a do loop will also execute the expressions inside of the curly braces, even if the condition in parenthesis initially returns false

The do loop will start testing if it should continue running, after the first initial execution
```
let yourName;

do {
  yourName = prompt('Enter name');
} while (!yourName);
// console.log(yourName);
```
- This program will repeatedly run until you provide a value


# for loops
For loops are another syntactical way to write loops in programs, but for loops provide a shorter way to accomplish the same task.

- all statements related to the 'state' of the loop are grouped together after *for*

Let's look at an example
```
for (let number = 1; number < 100; number += 2) {
  console.log(number);
};
```
- you'll notice three expressions inside our parentheses, separated by semi colons ;
  - the first expression usually initializes the loop
  - the second expression checks whether the loop will continue
  - the third expression updates the state of the loop after every iteration

In most cases, this is shorter and clearer than a while loop, as you may notice out in the field