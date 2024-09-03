# Q31-What is Contructor method

The constructor method is a special method for creating and initializing an object created within a class. If you do not specify a constructor method, a default constructor is used. The example usage of constructor would be as below,

```javascript
class Employee {
  constructor() {
    this.name = "Rahul";
  }
}

var employeeObject = new Employee();

console.log(employeeObject.name); //Rahul
```
