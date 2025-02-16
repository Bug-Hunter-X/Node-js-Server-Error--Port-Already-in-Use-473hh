# Node.js Server Error: Port Already in Use

This repository demonstrates a common error in Node.js when starting a server: the 'EADDRINUSE' error, which occurs when the specified port is already in use by another process.

The `bug.js` file contains code that attempts to start a server on port 8080.  If port 8080 is already occupied, the server will fail to start and throw the error.

The `bugSolution.js` file provides a solution to handle this gracefully.  It checks if the port is available before attempting to bind the server.

## How to reproduce the bug:
1. Clone the repository.
2. Run `node bug.js`.  If port 8080 is in use, you will encounter the error.
3. Run `node bugSolution.js`. This version should handle the port already in use scenario.