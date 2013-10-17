##This

* An example:

```var ryan = {  
  name: "Ry",  
  greet: function(){ alert("Hi" + this.name)}  
  ryan.greet(); //returns "Hi Ry"
```

* But ...
``` var Robot= {  
  name: "Bot",
  greet: ryan.greet()  
  }  
  Robot.greet(); // returns "Hi Bot"
  ```

* `this` is scoped to it's current object.

* use `call()` or `apply()` to send a context.



