# To Boolean

| Expected file |
| ------------- |
| to-boolean.js |

You must be able to convert any value to its Boolean equivalent.

### Instructions:

Create a function called `toBoolean` that takes any value (primitive or object) and returns its Boolean equivalent.

### Example:

```js
console.log(toBoolean(1)); // true
console.log(toBoolean(0)); // false
console.log(toBoolean("")); // false
console.log(toBoolean("hello")); // true
console.log(toBoolean([])); // true
console.log(toBoolean({})); // true
console.log(toBoolean(null)); // false
console.log(toBoolean(undefined)); // false
console.log(toBoolean(NaN)); // false
console.log(toBoolean(-42)); // true
```
