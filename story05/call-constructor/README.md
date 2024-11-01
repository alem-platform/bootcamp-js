# Using **call** in Constructor Functions

You're given a constructor function, you need to create another constructor function that use `call` to invoke it's own context with the given one.

### Resources:

[Function.prototype.call](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/call)

### Starting Code:

```js
function Animal(type) {
  this.type = type;
}

function Dog(name) {
  // your code here
}

const myDog = new Dog("Rex"); // Output: Dog { type: 'Dog', name: 'Rex' }
```
