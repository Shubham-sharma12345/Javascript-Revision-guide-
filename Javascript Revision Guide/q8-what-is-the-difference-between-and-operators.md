# Q8-What is the difference between == and === operators

`==` (Equality Operator)

* **Type Conversion**: The `==` operator compares two values for equality after converting both values to a common type. This is known as "type coercion".
* **Purpose**: Useful when you want to compare values without worrying about their types.
*   **Example**:

    ```javascript
    console.log(2 == '2'); // Output: true
    console.log(true == 1); // Output: true
    console.log(null == undefined); // Output: true
    ```

#### `===` (Strict Equality Operator)

* **No Type Conversion**: The `===` operator compares two values for equality without converting them to a common type. It checks both the value and the type.
* **Purpose**: Preferred when you want to ensure that both the value and the type are the same.
*   **Example**:

    ```javascript
    console.log(2 === '2'); // Output: false
    console.log(true === 1); // Output: false
    console.log(null === undefined); // Output: false
    ```
