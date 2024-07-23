# Q15-What is the purpose of the (let) keyword and how diff from (var)keyword

he `let` and `var` keywords are both used for variable declaration in JavaScript, but they have some important differences:

#### `let` Keyword

*   **Block Scope**: Variables declared with `let` are block-scoped. This means they are only accessible within the block (enclosed by curly braces `{}`) where they are defined. For example, a variable declared with `let` inside a loop or an `if` block cannot be accessed outside of that block.

    ```javascript
    if (true) {
        let x = 10;
        console.log(x); // 10
    }
    console.log(x); // ReferenceError: x is not defined
    ```
*   **No Hoisting**: `let` variables are not hoisted to the top of their block. They remain in a "temporal dead zone" from the start of the block until they are initialized.

    ```javascript
    console.log(y); // ReferenceError: y is not defined
    let y = 20;
    ```
*   **No Re-declaration in the Same Scope**: You cannot declare the same variable more than once in the same block scope using `let`.

    ```javascript
    let z = 30;
    let z = 40; // SyntaxError: Identifier 'z' has already been declared
    ```

#### `var` Keyword

*   **Function Scope**: Variables declared with `var` are function-scoped. If `var` is used inside a function, the variable is accessible throughout the entire function, regardless of block boundaries. If `var` is used outside of any function, the variable is globally scoped.

    ```javascript
    if (true) {
        var a = 50;
    }
    console.log(a); // 50
    ```
*   **Hoisting**: `var` variables are hoisted to the top of their function or global context. They are initialized with `undefined` until the code execution reaches their actual declaration.

    ```javascript
    console.log(b); // undefined
    var b = 60;
    ```
*   **Re-declaration Allowed**: You can declare the same variable multiple times within the same scope using `var`.

    ```javascript
    var c = 70;
    var c = 80; // No error
    ```
