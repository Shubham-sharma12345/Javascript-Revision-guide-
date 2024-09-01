# Q1- what are the Diff ways to write the Objects in js

JavaScript mein functions ko alag-alag tarikon se categorize kiya ja sakta hai. Yahan par hum kuch main types ke functions ke baare mein baat karenge:

1. **Function Declaration (Function Statements)**:
   * **Hindi**: Yeh woh functions hain jo directly declare kiye jaate hain.
   *   **Example**:

       ```javascript
        function greet() {
           console.log("Hello!");
       }
       ```
   * **Explanation**: Function declarations ka use tab hota hai jab aapko ek function ko define karna ho jo baad mein kahi bhi call kiya ja sakta hai.
2. **Function Expression**:
   * **Hindi**: Yeh woh functions hain jo expressions ke roop mein define kiye jaate hain.
   *   **Example**:

       ```javascript
        const greet = function() {
           console.log("Hello!");
       };
       ```
   * **Explanation**: Function expressions ko kisi variable ya object ke saath assign kiya ja sakta hai aur yeh tab execute hote hain jab unhe call kiya jaata hai.
3. **Arrow Functions**:
   * **Hindi**: Yeh ES6 mein introduce hue functions hain jo concise syntax provide karte hain.
   *   **Example**:

       ```javascript
        const greet = () => {
           console.log("Hello!");
       };
       ```
   * **Explanation**: Arrow functions ek compact syntax ke saath aate hain aur 'this' keyword ko lexical scope mein bind karte hain.
4. **Anonymous Functions**:
   * **Hindi**: Yeh woh functions hain jin ka naam nahi hota.
   *   **Example**:

       ```javascript
        setTimeout(function() {
           console.log("Hello!");
       }, 1000);
       ```
   * **Explanation**: Anonymous functions ko generally callbacks ke roop mein use kiya jaata hai.
