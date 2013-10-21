## By Snapkins

### Hex Codes for Color
* The `#000000` code is separated into RED, GREEN, BLUE elements with two hex digits for each.  

### Save
* When posting the `canvas.toDataUrl()` string via ajax as string data, the `+` are replaced with a space so you must put it into a json object.  
```
var canvas_data = canvas.toDataUrl();  

$.ajax({  
  type: 'post',  
  url: '/canvas',    
  data : {"canvas_key": canvas_data}  
  }); 

```