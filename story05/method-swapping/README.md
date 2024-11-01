# Method Swapping

You're given two objects, each with a method that uses this. Swap their methods and verify if they log the correct values after the swap.

### Starting Code:

```js
const obj1 = {
  name: "Object 1",
  getName: function () {
    return this.name;
  },
};

const obj2 = {
  name: "Object 2",
  getName: function () {
    return this.name;
  },
};

// your code here

console.log(obj1.getName()); // Output: 'Object 2'
console.log(obj2.getName()); // Output: 'Object 1'
```
