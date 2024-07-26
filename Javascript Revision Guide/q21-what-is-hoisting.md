# Q21-What is hoisting ?

&#x20;Hoisting  refers to the process that appears to move the _declaration_ of functions, variables, classes, or imports to the top of their [scope](https://developer.mozilla.org/en-US/docs/Glossary/Scope), prior to execution of the code.

&#x20;In MANY WEBSITES its written that is moves to to the top of the scope but that's not true&#x20;

for example

```javascript
// Some code
greet();
function greet(){
console.log("hello ji")
}
```

```javascript
// Some code
console.log(a);// undefined
var a=5;
```

but if we gave let

```javascript
// Some code
console.log(a)// it will gave reference error becoz we accessing this before variable intialized
let a=5;
// same goes with const.

```
