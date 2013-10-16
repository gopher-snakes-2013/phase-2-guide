# AJAX with Cricket

Asynchronous Javascript and XML

## XML

XML is a way to encode data that is both machine and human readable. In most of
our applications we will be passing HTML (or JSON).

## Asynchronous

Normally when you do web requests it goes to the server, downloads the full
HTML, and rerenders it in the browser.

With AJAX, we want this to happen in the background. We send out an HTTP
request using the XMLHTTP object, then when it gets done we apply just the
small bit of html that we needed.

This makes a very responsive, interactive web interface.

GMail does this by updating the DOM every time an email comes in.
