## Erb Tags
Browsers speak 3 languages:

1. CSS - For making things look pretty/layout
1. HTML - For the text on the page
1. Javascript - to make things interactive

## HTML

1. `<head>` - Holds stylesheet references and javascript references, title, and metadata
1. `<body>` - Holds the actual text that is being displayed
1. `<div>` - An invisible placeholder that you can use to organize your text.
1. `<p>` - a container for paragraphs of text

HTML is static, so you can't dry it up.

## ERB

ERB (embedded ruby) allows you to inject dynamic content into the page.
1. `<%= variable %>` - executes the code inside and prints out the return value
1. `<% %> - executes the code inside but does not print out the return value
1. Looping:
```
<% [1,2,3].each do |n| %>
  <li><%= n %></li>
<% end %> 
```
