##Active record validation errors

* 'rack-flash3' gem - allows you to 'flash' a custom message on the form with any validation errors.

* In you appfile
```require 'rack-flash'```  
```use Rack::flash```  

* In your route

``` if model.save do #save returns true if no validation errors```  
```erb new_page```

``` else #error in saving```
