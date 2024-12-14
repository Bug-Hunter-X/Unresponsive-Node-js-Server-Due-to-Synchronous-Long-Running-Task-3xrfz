# Unresponsive Node.js Server Due to Synchronous Long-Running Task

This repository demonstrates a common Node.js issue where a long-running synchronous operation in the request handler can make the server unresponsive.  The `bug.js` file contains the problematic code. The server simulates a 5-second delay, blocking the event loop and preventing it from handling other requests during this time. This leads to unresponsive behavior and poor performance.

The solution in `bugSolution.js` demonstrates how to use asynchronous operations or worker threads to prevent this blocking behavior and maintain responsiveness.