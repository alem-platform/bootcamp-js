# Has Own IT?

### Prototype Inheritance – Own vs Inherited Properties

You're givem an object `child` that inherits from another given object `parent`. Create function `hasOwnIt` that checks if a property belongs directly to the child or the prototype.

### Starting Code:

```js
const parent = { inheritedProp: "I am inherited" };
const child = Object.create(parent);
child.ownProp = "I am own property";

// you're code here

hasOwnIt(child, "ownProp"); // Output: true
hasOwnIt(child, "inheritedProp"); // Output: false
```
