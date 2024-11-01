# Immutability Protector

| Expected file            |
| ------------------------ |
| with-updated-property.js |

In this task, you need to update a property of an object without mutating the original.

### Instructions

Write a function called `withUpdatedProperty` that returns a new object with one property updated. Keep the original object safe from any changes.

The function should take three parameters:

- obj: The original object to be updated.
- key: The key of the property you want to update.
- value: The new value to assign to the specified property.

Function should return a new object that has the updated property, without modifying the original obj.

```js
function withUpdatedProperty(obj, key, value) {
  // ...
}
```

### Example:

```js
const obj = { name: "Alice", age: 25 };
const updatedObj = withUpdatedProperty(obj, "age", 26);

console.log(updatedObj); // Output: { name: 'Alice', age: 26 }
console.log(obj); // Output: { name: 'Alice', age: 25 } (unchanged)
```
