# The Hybrid Creature

Create a factory function named `createHybridObject` that returns objects created by a given constructor function. The factory function should accept parameters and pass them to the constructor.

### Requirements:

- The factory function `createHybridObject` should accept any parameters needed to create an object.
- The constructor function should define properties and methods for the objects being created.
- The factory function should return an instance of the object created by the constructor function.

### Starting Code:

```js
// Constructor function
function Gadget(type, brand) {
  this.type = type;
  this.brand = brand;
  this.getInfo = function () {
    return `${this.brand} makes the best ${this.type}!`;
  };
}

// Your factory function

const phone = createHybridObject("smartphone", "TechCo");
console.log(phone.getInfo()); // Output: 'TechCo makes the best smartphone!'
console.log(phone instanceof Gadget); // Output: true
```
