---
description: What is slice () method in Javascript and how to use this with example
---

# &#x20;Q 5-what is slice method()

**Ans**-`slice` method ka purpose JavaScript mein ek array ke ek section ko extract karna aur usse ek naye array mein return karna hai, bina original array ko modify kiye.

or&#x20;



`slice` method ka primary purpose yahi hai ki aap original array ke kuch elements ko lekar ek naye array mein daal sakte hain.

`slice` method original array ko bilkul bhi change nahi karta. Ye ek naya array return karta hai, jiska matlab hai ki aap elements ko use kar sakte hain bina original data ko affect kiye.

#### Syntax

```javascript
array.slice(start, end);

```

* **start**: Wo index jaha se extraction shuru karna hai. Agar negative hai, to ye array ke end se offset indicate karta hai.
* **end** (optional): Wo index jaha pe extraction khatam karna hai. Is index ka element include nahi hota. Agar omit kiya, to extraction array ke end tak chalta hai. Agar negative hai, to ye array ke end se offset indicate karta hai.
*

    #### Examples

    1.  **Basic Usage**:

        ```javascript
        const fruits = ['apple', 'banana', 'cherry', 'date', 'elderberry'];
        const citrus = fruits.slice(1, 3);
        console.log(citrus); // Output: ['banana', 'cherry']
        ```
    2.  **End Index Omit Karna**:

        ```javascript
        const fruits = ['apple', 'banana', 'cherry', 'date', 'elderberry'];
        const endToEnd = fruits.slice(2);
        console.log(endToEnd); // Output: ['cherry', 'date', 'elderberry']
        ```
    3.  **Negative Indices Use Karna**:

        ```javascript
        const fruits = ['apple', 'banana', 'cherry', 'date', 'elderberry'];
        const lastTwo = fruits.slice(-2);
        console.log(lastTwo); // Output: ['date', 'elderberry']
        ```
    4.  **Pure Array Ko Copy Karna**:

        ```javascript
        const fruits = ['apple', 'banana', 'cherry', 'date', 'elderberry'];
        const copyOfFruits = fruits.slice();
        console.log(copyOfFruits); // Output: ['apple', 'banana', 'cherry', 'date', 'elderberry']
        ```
