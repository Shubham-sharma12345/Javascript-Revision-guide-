# Q3-What is the difference between Call, Apply and Bind

Firstly call() method - Call method invoke the function with **this** value and pass the argument one by one

```javascript
let student1={
      name:"rahul",
      age:23
    }
    let fulldetails=function(){
     console.log(this.name+ "" +this.age);
    }
      fulldetails.call(student1)

    let student2={
      name:"anuj",
      age:26,

    }
    
    fulldetails.call(student2)
```

Apply() - Apply is also somewhat same like call but the only diff is it pass an argument as an array list

```javascript
const stu1={
      name: "sami",
      age:29,
    }
    let user=function(state,country){
      console.log(this.name + "" + state );
    }
  
      user.call(stu1,["delhi","rajastan","kashmir"]);
    const stu2={
      name: "amii",
      age:29,
    }
        //  user.call(stu2);
         user.call(stu2,["punjab","india"]);

```

Bind()-returns a new function, allowing you to pass any number of arguments

```javascript
let stud1={
          name:"rahul",
          age:23,
        
          userdetail:function(){
                  console.log(this.name);
          }
        }
        stud1.userdetail();
    
        let stud2={
          name:"anuj",
          age:26,
    
        }
        
           let output1=stud1.userdetail.apply(stud2)
         console.log(output1)

```
