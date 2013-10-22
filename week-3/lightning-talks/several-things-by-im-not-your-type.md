## By I'm not your type

### JavaScript Incrementation
* Post Increment (num++), performs the operation before incrementation. 

  ``` 
  var num = 0
  num++ // returns  0 and then increments.
  ```

* Pre Increment

  ``` 
  var num = 0
  ++num // returns  0 and then increments.
  ```

### Event Listeners
* If you register a named function in your event listener, it is passed the `event` object even though you don't see an argument for it in the call. 

```
function bindEventListeners(){  
  document.getElementById('typing-zone').addEventListenter('keypress', gameLogic)  
  // other events can also be bound here  
}  


// elsewhere in the code

function gameLogic(event){  
  // key press code here  
}  
```

