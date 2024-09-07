# Q 12-What is Higher order function

**Higher-Order Function** (HOF) wo function hota hai jo ya toh ek function ko **argument** ke roop mein accept karta hai ya phir ek function ko **return** karta hai. Matlab, yeh functions doosre functions ko as input le sakte hain ya output ke roop mein function de sakte hain.

#### Characteristics of Higher-Order Functions:

1. **Accepts a function as an argument.**
2. **Returns a function as a result.**

```javascript
// Some code
function greet(name) {
  return function(message) {
    console.log('Hello ' + name + ', ' + message);
  };
}

const personalizedGreet = greet('Amit'); // `greet` function ek doosra function return karta hai
personalizedGreet('How are you?'); // Yeh returned function ko baad mein call kiya jaa raha hai
```
