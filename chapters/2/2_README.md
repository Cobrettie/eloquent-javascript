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

### The Environment
The collection of bindings and their values at a given time, is called the **environment**


# Functions

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
invokedFunction('argument1', 'argument2', 'etc') {
  return 'function has been invoked';
} 
```
  - notice the strings inside of the parenthesis?
  - each comma separated value is called an *argument*, which is a value given to the function