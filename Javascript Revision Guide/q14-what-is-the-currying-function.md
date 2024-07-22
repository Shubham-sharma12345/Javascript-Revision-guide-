# Q14-What is the currying function

Currying is the process of taking a function with multiple arguments and turning it into a sequence of functions each with only a single argument. Currying is named after a mathematician **Haskell Curry.**

**in Hindi**

**Currying** ek functional programming technique hai jisme ek function ko aise transform kiya jata hai ki wo multiple arguments ko ek ek karke leta hai. Iska matlab hai ki hum ek function ko multiple arguments ki jagah ek ek argument pass karke call kar sakte hain.

Example:

**`function sendemail(to)`**

**`{  return function(subject)`**

**`{  return function(body)`**

**`{ console.log(hi there ${to} here is something ${subject} for you ${body});`**&#x20;

&#x20;**`}`**&#x20;

**`}`**&#x20;

&#x20;**`}`**

**`let step1= sendemail("shubham sharma");`**&#x20;

**`let step2 =step1("new order is ready");`**&#x20;

**`step2("hello");`**

**`or`**&#x20;

**`(arrow function)`**

**`const sendemail=(to)=>(subject)=>(body)=>`**&#x20;

**`console.log(hi there ${to} here is something ${subject} for you ${body});`**

**`let step1= sendemail("shubham sharma");`**&#x20;

**`let step2 =step1("new order is ready");`**&#x20;

**`step2("hello");`**

`or`

**`function add(a){`**&#x20;

**`return function(b){`**&#x20;

**`return a+b;`**

&#x20;**`}`**&#x20;

**`}`**&#x20;

**`console.log(add(5)(4));`**
