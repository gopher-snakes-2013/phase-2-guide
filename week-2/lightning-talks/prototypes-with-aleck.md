# Prototypes with Aleck

Prototype is a scary word. So I googled it.

```

function Tree() {
  this.height = 0;
  this.age = 0;
}

function OrangeTree() {
  this.orangeCount = 0;
}

OrangeTree.prototype = new Tree()
```

This looks like inheritance of some kind. OrangeTree is a kind of Tree

```
var orangeTree = new OrangeTree();
orangeTree.age; // 0
orangeTree.height; // 0; pulled from the tree that is the OrangeTree's prototype
orangeTree.orangeCount; // 0; pulled from orangeTree directly. 
```


[Difference between Orange.prototype and
Orange.__proto__](http://www.quora.com/JavaScript/What-is-the-difference-between-__proto__-and-prototype)

