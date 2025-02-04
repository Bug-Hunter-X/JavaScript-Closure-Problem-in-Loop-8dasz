# JavaScript Closure Problem in Loop

This repository demonstrates a common closure problem in JavaScript that occurs when using `setTimeout` or `setInterval` inside a loop.  The problem arises because the callback functions created within the loop share the same `i` variable, leading to unexpected behavior.

The `bug.js` file contains code illustrating the problem.  The `bugSolution.js` file provides a solution using `let` to create a new variable scope for each iteration of the loop, ensuring the correct value is captured for each `setTimeout` call.  This is a subtle but common issue that can cause headaches for JavaScript developers.

This example highlights the importance of understanding JavaScript closures and how they impact the use of asynchronous functions like `setTimeout` within loops.