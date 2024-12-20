# Animate points

| Expected file       |
| ------------------- |
| `animate-points.js` |

Create a function called `animatePoints` that animates a value from start to end over time.

### Instructions

Write a function that accepts an object with these properties:

- `start` (number): Starting value
- `end` (number): Ending value
- `steps` (number): Number of steps to take
- `duration` (number): Total animation time in milliseconds
- `onStep` (function): Callback for each step, receives:
  - `currentValue` (number): The current value
  - `stepNumber` (number): Current step number (0-based)
  - `timestamp` (number): Time elapsed since start

The function should:

- Animate from start to end in equal steps
- Call `onStep` at each step with current progress
- Space callbacks evenly over the duration
- Complete exactly after the specified duration
- Returns a cleanup function that when called:
  - Stops any pending animations
  - Clears all timers

Rules:

- Must use `setTimeout` or `setInterval`
- Must clean up any timers if animation is interrupted
- Must handle edge cases (steps < 2, duration <= 0, etc.)

### Resources

- [setTimeout](https://developer.mozilla.org/en-US/docs/Web/API/Window/setTimeout)
- [setInterval](https://developer.mozilla.org/en-US/docs/Web/API/Window/setInterval)
- [throw](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/throw)

### Example

```js
animatePoints({
  start: 0,
  end: 100,
  steps: 5,
  duration: 1000, // 1 second
  onStep: (value, step, time) => console.log(value),
});
// 0    // at 0ms
// 25   // at 200ms
// 50   // at 400ms
// 75   // at 600ms
// 100  // at 800ms (approx.)

try {
  animatePoints({
    start: 0,
    end: 10,
    steps: 0, // invalid steps
    duration: 1000,
    onStep: console.log,
  });
} catch (e) {
  console.log("Error caught successfully");
}

const cleanup = animatePoints({
  start: 0,
  end: 100,
  steps: 5,
  duration: 1000,
  onStep: (value) => console.log(value),
});

// After 300ms, we decide to stop the animation early
setTimeout(() => {
  cleanup(); // This should cancel all remaining steps
}, 300);

// Expected behavior:
// 0    (at 0ms)     - prints
// 25   (at 250ms)   - prints
```
