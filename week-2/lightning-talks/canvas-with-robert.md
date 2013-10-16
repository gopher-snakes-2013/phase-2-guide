# Canvas

## Adding an event listener

```
var canvas = document.getElementById('myCanvas')
canvas.addEventListener('mouseover', function(e) {
  console.log(e);
  console.log(this);
  console.log(e.x, e.y);
});
```

## Removing an Event listener
The addEventListener and removeEventListener need to be the same, so you need
to name the function.

```
var canvas = document.getElementById('myCanvas')

function logAllTheThings(e) {
  console.log(e);
  console.log(this);
  console.log(e.x, e.y);
}


function addTheListener() {
  canvas.addEventListener('mouseover', logAllTheThings);
}

function stopTheListener() {
  canvas.removeEventListener('mouseover', logAllTheThings);
}
```
