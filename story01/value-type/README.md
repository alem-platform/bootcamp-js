# Value Checker

| Expected file |
| ------------- |
| value-type.js |

Create a function that can tell the difference between `null`, `undefined`, and regular values.

### Instructions:

Create a function called `valueType` that takes a single value and returns a string indicating whether the value is:

- [null](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Operators/null)
- [undefined](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/undefined)
- or any other type (use [typeof](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Operators/typeof) operator for this part).

### Example:

```js
valueType(null);
// Output: 'null'

valueType(undefined);
// Output: 'undefined'

valueType(42);
// Output: 'number'
```
