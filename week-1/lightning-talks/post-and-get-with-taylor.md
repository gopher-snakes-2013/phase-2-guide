# What is the difference between POST and GET?

1. Think of it like a car. You can put a car in reverse and get wherever you
   want, but it's not a good idea.
1. POST is for when you're sending data that will make changes to the server
1. GET  is for when you're retrieving data from the server


## GET
1. GET sends data to the server in the request URL
1. GET requests are bookmarkable. It's not expected to change if you send the
   same requst over and over. The word is `idempotent`
1. Idempotent means multiple identical requests should have the same effect on
   the server

## POST
1. POST sends data to the server in the request body
1. POST is not bookmarkable. You expect multiple requests to change the server

## Sinatra

1. `get` and `post` are methods on sinatra
1. They handle the given request method to the given route with the passed in
   block
