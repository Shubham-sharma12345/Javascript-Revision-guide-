# Q 10 -What is a first class function

First class Function are also called as first class citizen and and it always treated as other values, string ,number and we can store in variable , pass as an argument ,return in  other function

Examples

**Store as variable**

`var a= function(){`

`console.log("hello ji);`

`}`

`a();`



**`Pass as an argument`**

`function a(){`&#x20;

`return 'This is a function';`

&#x20;`}`&#x20;

`function b(name)`

`{ console.log(name());`

&#x20;`}`&#x20;

`b(a);`

**Return into other function**

`function a(){`&#x20;

`return function b()`

`{ console.log("This is the function")`

&#x20;`}`

&#x20;`} a()();`
