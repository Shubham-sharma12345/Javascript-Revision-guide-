---
description: >-
  A callback function is a function passed into another function as an argument.
  This function is invoked inside the outer function to complete an action.
---

# What is a callback function

```javascript
// Some code
function greet(name, callback) {
  console.log('Hello ' + name);
  callback();
}

function sayGoodbye() {
  console.log('Goodbye!');
}

// Passing 'sayGoodbye' as a callback to the 'greet' function
greet('Alice', sayGoodbye);


```
