# Q 9-What are lambda expressions or arrow functions

Ans- Arrow functions JavaScript mein ek concise aur simple tarika hai functions likhne ka

#### Basic Syntax

Arrow function likhne ka basic syntax kuch aisa hota hai:

```javascript
const functionName = (parameters) => {
  // function body
};
```

#### Examples

1.  **Single Parameter**: Agar function sirf ek parameter leta hai, to parentheses (`()`) optional hain:

    ```javascript
    const square = x => x * x;
    console.log(square(5)); // Output: 25
    ```
2.  **Multiple Parameters**: Multiple parameters ke saath parentheses zaroori hain:

    ```javascript
    const add = (a, b) => a + b;
    console.log(add(3, 4)); // Output: 7
    ```
3.  **No Parameters**: Agar function koi parameter nahi leta, to empty parentheses use karte hain:

    ```javascript
    const greet = () => 'Hello, world!';
    console.log(greet()); // Output: Hello, world!
    ```
4.  **Multiple Statements in Function Body**: Agar function body mein multiple statements hain, to curly braces `{}` use karte hain, aur explicitly `return` statement likhna padta hai:

    ```javascript
    const addAndDouble = (a, b) => {
      const sum = a + b;
      return sum * 2;
    };
    console.log(addAndDouble(3, 4)); // Output: 14
    ```
