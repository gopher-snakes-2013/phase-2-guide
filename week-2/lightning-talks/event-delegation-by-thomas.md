## Event Delegation

* Allows you to attach an event listener to a parent and delegate it to the children.
* Less events to bind.
* Allows you to bind to events that are dynamically added to a page after the script loads. 

```
document.getElement("ul")  
addEventListener("click", function(e){  
  if (e.target==='li'){  
    function(){  
      //do stuff  
    }  
  }  
});  
```

* Way easier in jQuery

``` 
$('ul').on('click', 'li' function(){
  
  //do stuff
})
```