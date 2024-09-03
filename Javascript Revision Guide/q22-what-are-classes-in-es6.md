# Q22-What are classes in ES6

In ES6 (ECMAScript 2015), classes were introduced as a more elegant syntax for creating and working with objects and inheritance in JavaScript. They provide a cleaner and more intuitive way to handle object-oriented programming compared to the older prototype-based approach. Here's a detailed look at ES6 classes:

#### **Basic Syntax**

A class in ES6 is defined using the `class` keyword. It can have a constructor and methods. Here's the basic syntax:

**Syntax:**

```javascript
class ClassName {
  constructor(parameters) {
    // Initialization code
  }

  method1() {
    // Method code
  }

  method2() {
    // Method code
  }
}
```

**Example:**

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log(`Hello, my name is ${this.name} and I am ${this.age} years old.`);
  }
}

const person1 = new Person('Alice', 30);
person1.greet(); // Output: Hello, my name is Alice and I am 30 years old.
```

#### **Key Features**

1.  **Constructor:**

    * The `constructor` method is a special method that is called when an instance of the class is created. It is used for initializing object properties.

    ```javascript
    class Person {
      constructor(name, age) {
        this.name = name;
        this.age = age;
      }
    }
    ```
2.  **Methods:**

    * Methods defined inside a class are added to the prototype of the class. They are accessible to all instances of the class.

    ```javascript
    class Person {
      greet() {
        console.log('Hello!');
      }
    }
    ```
3.  **Inheritance:**

    * ES6 classes support inheritance using the `extends` keyword. You can create a subclass that inherits from a parent class.

    ```javascript
    class Animal {
      speak() {
        console.log('Animal makes a sound');
      }
    }

    class Dog extends Animal {
      speak() {
        console.log('Dog barks');
      }
    }

    const dog = new Dog();
    dog.speak(); // Output: Dog barks
    ```
4.  **Super:**

    * The `super` keyword is used to call methods from the parent class. This is especially useful in constructors and when overriding methods.

    ```javascript
    class Animal {
      constructor(name) {
        this.name = name;
      }

      speak() {
        console.log(`${this.name} makes a sound`);
      }
    }

    class Dog extends Animal {
      constructor(name, breed) {
        super(name); // Call parent constructor
        this.breed = breed;
      }

      speak() {
        super.speak(); // Call parent method
        console.log(`${this.name} barks`);
      }
    }

    const dog = new Dog('Rex', 'German Shepherd');
    dog.speak();
    // Output:
    // Rex makes a sound
    // Rex barks

    ```

```javascript
// Some code
 class student2 extends student1{
   
   constructor(name,name1){
     
     super(name);
     this.name1=name1;
   }
   namer(){
     super.namer();
     console.log(`${this.name} also known as ${this.name1}`);
   }
 }
 
 const person1= new student2('shubham','shubhi');
 person1.namer();
   
   
```

1.  **Getters and Setters:**

    * Classes in ES6 can have getter and setter methods that allow you to define how properties are accessed and modified.

    ```javascript
    class Rectangle {
      constructor(width, height) {
        this.width = width;
        this.height = height;
      }

      get area() {
        return this.width * this.height;
      }

      set dimensions({ width, height }) {
        this.width = width;
        this.height = height;
      }
    }

    const rect = new Rectangle(5, 10);
    console.log(rect.area); // Output: 50

    rect.dimensions = { width: 10, height: 20 };
    console.log(rect.area); // Output: 200
    ```
