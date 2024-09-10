---
description: >-
  A callback function is a function passed into another function as an argument.
  This function is invoked inside the outer function to complete an action.
---

# What is a callback function

```javascript
// Some code
function addwaterinPan(){
    console.log("Add Water in pan")
}
function Waterboils(callback){
    console.log("water boils")
    setTimeout(()=>{
        console.log("Water boiled")
        callback();
    },3000)
}
function addSugar(){
    console.log("Add Sugar")
    addGiner()
}
function addGiner(){
    console.log("Add Ginger")
    console.log("wait of 2 sec")
    setTimeout(()=>{
       PourItserve()
    },2000)
}
function PourItserve(){
    console.log("Serve to coustomer")
}

addwaterinPan()
Waterboils(addSugar)



```
