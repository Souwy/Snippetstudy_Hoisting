# Snippetstudy_Hoisting

## Description of snippet
Investigate variables and hoisting. Illustrate the difference between `var` and `let` in terms of hoisting.

## Learning objectives (keywords)
* How `var` and `let` (functioning differently with regard to hoisting)
* Concept of hoisting

## Code snippet #1
```js
var x = "a string";

console.log(x);
console.log(y);
console.log(z);

var y = "two strings";
let z = "three strings";

console.log(x + " is great, " + y + " is better but the best is " + z)
```

The code doesn't work because the variable let is not hoisted, therefore not declared. It breaks down at the point that I try to `console.log` `z`. 
It is possible to log `x` because it has already been declared and defined, and `y` because it has been hoisted and thus has the value `undefined`.

## The Fix
Two options are possible. Either declare `z` before trying to log it, or use `var` instead of `let`.
```js
var x = "a string";
let z = "three strings";

console.log(x);
console.log(y);
console.log(z);

var y = "two strings";


console.log(x + " is great, " + y + " is better but the best is " + z)
```

## Vocabulary
- 
   
## Review
* Struggles: 
  * 
* Learning objectives that need extra work?   
  * 
* next steps: 
  * 

## Helpful links
[Good explanation on W3](https://www.w3schools.com/js/js_hoisting.asp)
