# Canvas with Salar

1. Canvas is an HTML element
1. You can create a canvas with a height and width. This gets added to the DOM
1. You can listen for events on the canvas

```
var canvas = document.querySelector('canvas');
function printEvent(event) {
  console.log(event);
  console.log(this);
}

canvas.addEventListener('mousedown', printEvent);
```

And that gives you [useful
data!](https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent?redirectlocale=en-US&redirectslug=DOM%2FMouseEvent)

Remember to P on everything.
