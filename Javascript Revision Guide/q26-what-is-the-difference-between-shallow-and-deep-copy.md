# Q26-What is the difference between Shallow and Deep copy

* Shallow copy ka matlab hai ki aap object ya array ka sirf top-level properties copy karte ho. Agar object ya array ke andar aur bhi nested objects (matlab objects ke andar objects) hain, to shallow copy unhe copy nahi karti, bas unka reference (pointer) copy karti hai.

```javascript
// Some code
let original = { name: "John", address: { city: "New York" } };
let shallowCopy = { ...original };

shallowCopy.address.city = "Los Angeles";

console.log(original.address.city);  // Output: Los Angeles

```

**Deep Copy:**

* **Explanation:**
  * Deep copy ka matlab hai ki aap object ya array ka ekdum naya aur complete copy banate ho, jisme nested objects ya arrays bhi included hote hain. Matlab, deep copy aur original object bilkul independent hote hain; agar aap ek mein change karoge to dusre mein koi farak nahi padega.

```javascript
// Some code
let original = { name: "John", address: { city: "New York" } };

// Deep copy create kar rahe hain using structured cloning (JSON)
let deepCopy = JSON.parse(JSON.stringify(original));

// Ab hum nested object ko deep copy mein modify kar rahe hain
deepCopy.address.city = "Los Angeles";

console.log(original.address.city);  // Output: New York
console.log(deepCopy.address.city);  // Output: Los Angeles
```
