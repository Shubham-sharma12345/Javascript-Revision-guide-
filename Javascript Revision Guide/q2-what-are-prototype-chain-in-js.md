# Q2- what are prototype Chain in Js

**Prototype  chain**-   jab ham ek object ko create karte hai to uske sath a hidden property create hoti **(\_**_**proto\_)**_ jisko ham protoype kehte hai. in english(it is type of mechanism that allows objects to inherit properties and methods from other objects.

example of prototype chain

class animal={

jumps:true;

}

class rabbit={

eats:true;

}

rabbit.\__proto_\_ = animal; // we use this **\_**_**proto\_**_ to inherit the other object.

console.log(rabbit.eats);
