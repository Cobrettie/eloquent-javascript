# Chessboard

- 8x8 grid
- new line after 8 characters
- space counts as character
- 

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
    } 
  }
    string += '#';
  string += '\n';
}
console.log(string);
```