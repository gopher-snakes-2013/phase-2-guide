## JavaScript Fun

* You don't need the `;` that often. It ends a statement but so does a newline.

* A `;` can be used to preference a file or the beginning of an anonymous function to prevent the anonymous function from being accidentally invoked.

* Working with anonymous functions: 
```
(function(){  
  var a = 5;  
  })()
```

  * Useful for defining scope and private vs public. 

###  Scope

* If you ever define a variable without `var` then it is global from there on. In both of the following examples, globalVar is global. 

```
globalVar = 5 
function(){ 
  var localVar = 3  
}  
```

```
var localVar = 2  
function(){
  globalVar =5  
}
```

### this
* `this` is the object that is invoking (calling) a function.
* A function is an invokable variable. 


### new

* If we use the `new` method to create an instance of a object then we gain access to the prototype and `this` is mapped to the instance.  Use to create multiple instances. 
```
function A(){  
  this.name="my name"  
  this.something = 3  
}  
  
b = new A()  
  
//  {name: "my name", something: 3}  

b.name = "hi"  

// b is now {name: "hi", name: "my name", something: 3}
b.name  
// returns "hi"  
  
```

* If you override a prototype value in the object instance, then the object instance definition will be used. 

