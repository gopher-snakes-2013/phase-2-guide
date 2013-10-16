##Testing JavaScript in Your Web Apps

See [sample-jasmine-application]() for code.

### Add Jasmine

* Add to your gemfile and require it:  
```gem jasmine```  
 ```require 'jasmine'```

* In the console, type: ```jasmine init```
* Then follow instructions on the console to set up a default jasmine project with lots of default files and folders. 

* Add files to ```public/javascripts``` files and they will be loaded when you run jasmine

* Add files to ```spec/javascripts``` named file_name_spec.js and they will be run when you type: ```rake jasmine```

* Add a ```javascript/vendor``` folder for any js libraries (like jquery).  Edit the ```jasmine.yml``` file to include all files in the vendor file before your local js files. 

### Add jasmine-jquery and jasmine-fixture
* Read the docs: [jasmine-jquery](https://github.com/velesin/jasmine-jquery) , [jasmine-fixture](https://github.com/searls/jasmine-fixture)
* Save these and any other libraries to the ```spec/helpers``` directory.
* Jasmine-Jquery makes it easy to test against the DOM using jQuery. It comes
with dozens of matchers like 'toHaveClass' or 'toHandleWith' which allow you to
express your desired behavior with very little work
* Jasmine-fixture makes it a snap to insert stuff into the DOM without doing a
ton of work. Your JavaScript is often going to be coupled to the DOM; so you'll
be doing a lot of tests which have to deal with your HTML structure.

#### Maybe add jasmine Given
* Read the docs: [jasmine-given](https://github.com/searls/jasmine-given)
* Watch the video by Justin Searls on [javascript testing tactics](https://speakerdeck.com/searls/javascript-testing-tactics)

### Wire it all together
* Update the ```jasmine.yml``` file to link to your public files and spec files. 