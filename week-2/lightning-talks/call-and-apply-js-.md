##Call and Apply Methods in JS

* JS is based on functions, not objects. 
  * this can cause some confusion on scope and the keyword 'this'

* The `call` and `apply` methods are called on another function to set the context for the calling function.

``` 
var person1 = {name: "laura"}
var update=function)(name, age){  
  this.name=name;  
  this.age=age;  
}  

update.call(person1, 'susan', 40)  
```

* The call method requires you to define all parameters, whereas the `apply` method can have an array that allows you to send some parameters. 




