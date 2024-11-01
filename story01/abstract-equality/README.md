# The Abstract Equality

| Expected file        |
| -------------------- |
| abstract-equality.js |

Create a function called `abstractEquality` that compares two values and determine if they are abstractly equal, even if the types differ.

### Resources:

- [Data structures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)
- [Type Coercion](https://developer.mozilla.org/en-US/docs/Glossary/Type_coercion)
- [Equality comparisons](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness)

### Example:

```js
abstractEquality(2, "2"); // Output: true
abstractEquality(0, false); // Output: true
abstractEquality(null, undefined); // Output: true
```
