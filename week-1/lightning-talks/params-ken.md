#Params

* It's a hash

* A route that looks like
``` get '/:id' ``` is used to handle the url : ``` www.stuff.com/5``` and the key ```:id``` is associated with the value ```5``` yielding ```params={id: 5}```

* What about the ? in a url. 
The url ```www.stuff/?name=charles``` then the params from the route 
``` get '/' ``` would be ```params = {name: 'charles'}

* If you have an & in the url parameters it maps to another key value pair. 

* A post request also 