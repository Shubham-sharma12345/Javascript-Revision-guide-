---
description: >-
  splice method basically modify the original array used to add ,remove and
  replace the elements from an array.
---

# What is Splice() method

Aap specified index se elements ko remove, add, ya replace kar sakte hain.Examples

1.  **Elements Remove Karna**:

    ```javascript
    const fruits = ['apple', 'banana', 'cherry', 'date', 'elderberry'];
    const removed = fruits.splice(2, 2);
    console.log(fruits); // Output: ['apple', 'banana', 'elderberry']
    console.log(removed); // Output: ['cherry', 'date']
    ```
2.  **Elements Add Karna**:

    ```javascript
    const fruits = ['apple', 'banana', 'elderberry'];
    fruits.splice(2, 0, 'cherry', 'date');
    console.log(fruits); // Output: ['apple', 'banana', 'cherry', 'date', 'elderberry']
    ```
3.  **Elements Replace Karna**:

    ```javascript
    const fruits = ['apple', 'banana', 'cherry', 'date'];
    fruits.splice(1, 2, 'kiwi', 'mango');
    console.log(fruits); // Output: ['apple', 'kiwi', 'mango', 'date']
    ```
