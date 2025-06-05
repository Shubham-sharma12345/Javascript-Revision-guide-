# Q36-Async/Await

```javascript
// Some code
// Step 1: Ticket book karna
function bookTicket() {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      console.log("✅ Ticket booked");
      resolve("Ticket #M123");
    }, 1000);
  });
}

// Step 2: Popcorn lena
function getPopcorn(ticket) {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      console.log("🍿 Popcorn ready for", ticket);
      resolve("Popcorn Combo");
    }, 1500);
  });
}

// Step 3: Movie dekhna
function watchMovie(popcorn) {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      console.log("🎥 Watching movie with", popcorn);
      resolve("Movie enjoyed!");
    }, 2000);
  });
}

// Final async function
async function enjoyMovie() {
  try {
    const ticket = await bookTicket();         // Step 1
    const popcorn = await getPopcorn(ticket);  // Step 2
    const result = await watchMovie(popcorn);  // Step 3
    console.log("😄 Experience:", result);
  } catch (err) {
    console.log("❌ Error:", err);
  }
}

// Run the function
enjoyMovie();

```
