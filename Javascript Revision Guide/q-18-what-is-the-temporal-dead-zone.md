# Q 18-What is the Temporal Dead Zone

The Temporal Dead Zone(TDZ) is a specific period or area of a block where a variable is inaccessible until it has been intialized with a value. In ECMAScript 6, accessing a `let` or `const` variable before its declaration (within its scope) causes a ReferenceError.

example

**`function somemethod()`**

&#x20;**`{`**&#x20;

**`console.log(counter1); // undefined`**&#x20;

**`console.log(counter2);// Reference Error`**

&#x20;**`var counter1 = 1;`**&#x20;

**`let counter2 = 2;`**

&#x20;**`}`**
