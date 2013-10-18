##AJAX and JSON

* The .to_json method allow you to change a ruby hash into JSON (JavaScript Object Notation).

* JSON can be returned to an AJAX call. 

* The html code 
```
<form method='post' action='/user'>  
  <input type='text' name='first_name'> 
  <button> Submit </button>  
</form>
```

* The route:
```  
post '\user' do  
  content_type :json  
  {name: "nat", cohort: "gopher snakes"}.to_json
end
