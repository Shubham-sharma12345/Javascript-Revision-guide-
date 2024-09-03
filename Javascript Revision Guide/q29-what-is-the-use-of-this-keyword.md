# Q29- What is the use of this keyword

This keyword is used to access the current objects and classes

```javascript
// Some code
class person{
    constructor(name,age){
        this.name=name;
        this.age=age;
        
    }
    sayHello(){
        console.log(`This is ${this.name}and his age is${this.age}`);
    }
}
const Person= new person('john',34)
Person.sayHello();
```

If we wont' use use this keyword so how we diffrentiate which one is parameter and which one is property here

```javascript
// Some code
class Person {
  constructor(name) {
    this.name = name; // 'this' refers to the newly created object
  }
  
```
