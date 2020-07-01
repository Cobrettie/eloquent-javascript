# Looping a Triangle
Write a loop that makes seven calls to console.log to output the following triangle: *image in Eloquent JavaScript 3rd Edition p.37*

Basically, 
<!-- 
#
##
###
####
#####
######
#######
 -->


It may be helpful to know that you can find the length of a string by writing .length after it
```
let string1 = 'hey friend';
console.log(string1.length);
// 10
```

## My Solution

```
let string = '';

for (let counter = 0; counter < 7; counter++) {
  string +='#';
  console.log(string);
}
```

## Eloquent JS Solution
```
for (let line = '#'; line.length < 8; line += '#') 
  console.log(line)
```


