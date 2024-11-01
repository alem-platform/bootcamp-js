# The Key Finder

| Expected file |
| ------------- |
| has-key.js    |

Write a function called `hasKey` that takes an object and a key name, and checks if the key is present, using the `in` operator. The presence of the key must be true, even if its value is `falsy`.

### Resources:

- [in](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/in)
- [falsy](https://developer.mozilla.org/en-US/docs/Glossary/Falsy)

### Example:

```js
hasKey({ name: "Alice", age: 0 }, "age");
// Output: true

hasKey({ job: null }, "job");
// Output: true

hasKey({ country: "USA" }, "city");
// Output: false
```
