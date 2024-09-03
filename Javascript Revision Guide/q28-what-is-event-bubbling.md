# Q28- what is Event Bubbling

**Event Bubbling** ka concept simple shabdon mein samajhte hain.

Jab aap kisi element (jaise button) pe click karte ho, toh us element ke saath-saath uske parent elements (jaise us button ka containing `div`) bhi jaante hain ki click hua hai. Yeh process **event bubbling** kehlata hai, jisme event sabse pehle us element pe trigger hota hai jisme aapne click kiya, aur phir yeh event uske parent elements tak bubble karta hai, matlab upar ki taraf move karta hai.

#### Simple Example:

Maan lo aapke paas yeh HTML structure hai:

```html
<div id="parent">
  <button id="child">Click Me</button>
</div>
```

Ab, agar aap `button` pe click karte ho, toh event bubbling kaise kaam karta hai, yeh samajhte hain:

1. Pehle, `button` (child element) pe `click` event trigger hota hai.
2. Uske baad, yeh `click` event bubble karta hai aur `div` (parent element) tak pahunchta hai.

Agar aap dono elements pe event listeners lagate ho:

```javascript
document.getElementById("child").addEventListener("click", function() {
  alert("Button clicked!");
});

document.getElementById("parent").addEventListener("click", function() {
  alert("Div clicked!");
});
```
