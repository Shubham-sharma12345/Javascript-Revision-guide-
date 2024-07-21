---
description: >-
  Ans- Json is javascript object notation it is text based format used to
  transmit the data b/w servers or between diffrent parts of program.
---

# Q4 -What is JSON

example this **JSON.parse**(convert string to object)

```javascript
const user1='{"name":"shubham","age":30}'
const jsonobj=JSON.parse(user1);
console.log(jsonobj);

```

2-JSON.stringify(convert object to  string)

```javascript
const user1={name:"shubham",age:30}
const jsonstring=JSON.stringify(user1);
console.log(jsonstring);

```

3-dot notation&#x20;

```javascript
const user1={
  name:"shubham",
  age:30,
  courses:["maths","english"]
}

console.log(user1.name);
console.log(user1['courses']);
```
