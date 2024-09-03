# Q32-How do you call the constructor of a parent class

`super()` keyword ka use karke call kar sakte ho.

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


class person2 extends person{
    
    constructor(name,city){
        super(name)
       
        this.city=city;
        
    }
    sayHello(){
         console.log(`This is ${this.name}and his age is${this.age}`);
    }
}

const Person2= new person2('raja','rajasthan')
Person2.sayHello();

```
