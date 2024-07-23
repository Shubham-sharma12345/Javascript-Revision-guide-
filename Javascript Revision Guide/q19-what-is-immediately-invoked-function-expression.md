# Q19-what is Immediately Invoked Function Expression,

An IIFE, or Immediately Invoked Function Expression, is a design pattern in JavaScript used to execute a function immediately after it's defined. This is achieved by defining a function and then immediately invoking it.

#### Syntax

An IIFE is typically written like this:

```javascript
 (function() {
    // Code here runs immediately
})();

```

```javascript
(function() {
    var message = "Hello, World!";
    console.log(message); // Outputs: Hello, World!
})();
```

```javascript
   var result = (function(a, b) {
    return a + b;
});

console.log(result(5,10));
```

The primary reason to use an IIFE is to obtain data privacy because any variables declared within the IIFE cannot be accessed by the outside world. i.e, If you try to access variables from the IIFE then it throws an error as below,

```javascript
(function () {
  var message = "IIFE";
  console.log(message);
})();
console.log(message); //Error: message is not defined
```
