# what are Promises

Promise asynchronous operations ke results ko handle karne ke liye use hota hai, jaise API calls, file reading, ya kisi bhi task jo time le sakta hai.

`Promise` in JavaScript is an object that represents the eventual completion (or failure) of an asynchronous operation and its resulting value. It provides a way to handle asynchronous operations more effectively than traditional callback functions.

#### Promise Ke Methods

**`then(onFulfilled, onRejected)`**: Jab promise fulfilled hota hai, `onFulfilled` function call hota hai. Agar promise rejected hota hai, to `onRejected` function call hota hai.

```javascript
myPromise.then((result) => {
  console.log(result); // Success message
}).catch((error) => {
  console.log(error); // Error message
});
```

1.  **`catch(onRejected)`**: Rejected promise ko handle karne ke liye use hota hai. Ye `then` ke `onRejected` function ka shorthand hai.

    ```javascript
     myPromise.catch((error) => {
      console.log(error); // Error message
    });
    ```
2.  **`finally(onFinally)`**: Ye method chahe promise fulfilled ho ya rejected, hamesha execute hota hai. Ye cleanup code ke liye useful hota hai.

    ```javascript
    myPromise.finally(() => {
      console.log("Promise complete");
    });


    ```

```javascript
// Some code
function fetchData() {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      const success = true; // Imagine this is the result of some async operation
      if (success) {
        resolve("Data fetched successfully");
      } else {
        reject("Failed to fetch data");
      }
    }, 2000);
  });
}

fetchData()
  .then(data => {
    console.log(data); // Data fetched successfully
  })
  .catch(error => {
    console.log(error); // Failed to fetch data
  })
  .finally(() => {
    console.log("Operation complete");
  });

```
