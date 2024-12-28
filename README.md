# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common error in Node.js server applications: improper handling of exceptions within the request handler.  The `server.js` file showcases the problem, where an unhandled exception causes the server to crash.

The solution, found in `serverSolution.js`, utilizes a try-catch block to handle the exception gracefully and prevents the server from crashing.

## How to Reproduce

1. Clone the repository.
2. Navigate to the directory.
3. Run `node server.js`.
4. Access `http://localhost:3000/error` in your browser (or use a tool like curl).  Observe that the server crashes.
5. Run `node serverSolution.js` and repeat step 4.  Observe that the server handles the error without crashing.

## Lessons Learned

Always use try-catch blocks within your request handlers to catch and handle potential exceptions.  Logging the errors appropriately is crucial for debugging and monitoring.