# Q27- Diffrence between Map And Js Object

* O**bject:** JavaScript `Object` mein keys sirf strings ya symbols ho sakti hain. Agar aap kisi aur type ka key dene ki koshish karte ho (jaise number ya object), toh JavaScript usse automatically string mein convert kar deta hai.
  *   Example:

      ```javascript
      let obj = {};
      obj[1] = "one"; // 1 key ko "1" string bana diya jayega
      ```
* **Map:** `Map` mein keys kisi bhi type ki ho sakti hain—string, number, object, ya function—sab kuch as it is store hota hai.
  *   Example:

      ```javascript
      let map = new Map();
      map.set(1, "one"); // 1 key number type mein hi store hota hai
      ```

#### 2. **Order of Keys**

* **Object:** Keys ka order generally maintain nahi hota (although modern browsers mein kuch cases mein order maintain hota hai, lekin yeh reliable nahi hai).
* **Map:** `Map` mein keys insertion order mein hi store hoti hain, toh aapko pata hota hai ki kaunse key pehle insert hui thi.
