# Count-Masters

### Instructions:

Write a function called `countMaster` that returns another function (an inner function). This inner function will maintain its own count, even after multiple invocations. Each time the inner function is called, it should increment the counter and return the updated value.

- Write a function `countMaster` that initializes a count variable at 0.
- The function returns an inner function that increments count and returns the current value.
- Ensure that the count value persists across multiple invocations of the inner function.

### Example:

```js
const counter = countMaster();
counter(); // Output: 1
counter(); // Output: 2
counter(); // Output: 3
```

```js
const firstCounter = countMaster();
const secondCounter = countMaster();

firstCounter(); // Output: 1
firstCounter(); // Output: 2
secondCounter(); // Output: 1
```