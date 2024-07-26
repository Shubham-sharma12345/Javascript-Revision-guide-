# what are clousers

A closure is the combination of a function bundled(enclosed) together with its lexical environment within which that function was declared. i.e, It is an inner function that has access to the outer or enclosing function’s variables, functions and other data even after the outer function has finished its execution. The closure has three scope chains.

1. Own scope where variables defined between its curly brackets
2. Outer function's variables
3. Global variables

```javascript
// Some code
function outerFunction(outerVariable) {
    return function innerFunction(innerVariable) {
        // innerFunction has access to outerVariable from outerFunction
        console.log("Outer Variable: " + outerVariable);
        console.log("Inner Variable: " + innerVariable);
    };
}

const closureFunction = outerFunction("Hello");
closureFunction("World");
// Output:
// Outer Variable: Hello
// Inner Variable: World

```
