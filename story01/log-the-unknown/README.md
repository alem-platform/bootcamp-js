# Log the Unknown

| Expected file      |
| ------------------ |
| log-the-unknown.js |

Design a function called `logTheUnknown` that examines any given input and logs a message describing its type.

### Instructions:

- Create a function called `logTheUnknown`. This function should be able to accept any value and log its type using `typeof` operator.
- If the type starts with a vowel sound, use "an" in the message (e.g., "an object"). Otherwise, use "a" in the message (e.g., "a number", "a string")

### Function Declaration:

```js
function logTheUnknown(n) {
  //
}
```

### Resources:

[typeof](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Operators/typeof)

### Example:

```js
logTheUnknown(42);
// will return "Scanning complete: This is a number!"

logTheUnknown("hello");
// will return "Scanning complete: This is a string!"

logTheUnknown({});
// will return "Scanning complete: This is an object!"
```
