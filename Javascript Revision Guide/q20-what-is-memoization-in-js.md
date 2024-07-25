---
description: (in simple term)
---

# Q20- what is memoization in js

Memoization is functional programming technique which attempts to increase a function’s performance by caching its previously computed results. Each time a memoized function is called.

If the data is present, then it can be returned, without executing the entire function. Otherwise the function is executed and then the result is added to the cache.

example

```javascript
 function memo(func){
       const cache= new Map();

       return function(args){
              let keys=JSON.stringify(args);
              if( cache.has(keys)){
                return cache.set(keys);
              }

              const result= func(args);
                 cache.set(keys,result);
                 return result;
       }
  }

  function fibbo(n){
       if(n<=1)
        return n;
         return fibbo(n-1)+fibbo(n-2);
       
  }

  const output= memo(fibbo);
  console.log(output(10));
```
