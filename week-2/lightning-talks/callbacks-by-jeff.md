## Callbacks

* Passing a function as an argument to a callback function. 

``` function doStuff(a,b, callback){  
    c=a+b;  
    return callback(c);  
}```

``` function loud(speech){  
  return speech.toUpperCase
}```

``` function soft)(speech){  
  return speech.toLowerCase  
}```

Now you can send either `loud` or `soft`

