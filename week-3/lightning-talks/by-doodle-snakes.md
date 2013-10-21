## By Doodle Snakes

### Event Handlers
* When working with canvas, separating the `ctx.beginpath()` and `ctx.endpath()` from the drawing allows better integration with mouse events.

### Storing the image
* use base64 encoding to get a string encoding of your image that can be stored in the database. Canvas does this with the `.toURL()` method.
* doesn't appear to be a canvas method to reverse the `.toURL()` method to get back an image to continue drawing. 

### Testing Canvas?
* Use faker to populate database and create rake tasks and a module to allow for quick testing. 

### Bcyrpt
* salted hash - get a different hash for the same unencrypted password for each entry in the database.  (if two users have the same password they will have different hashed passwords.)