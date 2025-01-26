# Unhandled Server Errors in Node.js

This repository demonstrates a common error in Node.js server development: inadequate error handling. The `bug.js` file showcases a server vulnerable to crashes due to unhandled errors.  The `bugSolution.js` provides a more robust solution.

## Bug

The `bug.js` server lacks proper error handling.  If an error occurs (e.g., port in use), the server might crash without providing informative logs or gracefully shutting down.

## Solution

The `bugSolution.js` demonstrates improved error handling by:

1.  Using a `try...catch` block to handle potential errors during server initialization.
2.  Implementing comprehensive `'error'` event listeners for the server to catch and log errors appropriately.
3.  Gracefully shutting down the server on error, minimizing the impact of the unexpected failure.

This improved error handling prevents unexpected server crashes and provides better debugging information.