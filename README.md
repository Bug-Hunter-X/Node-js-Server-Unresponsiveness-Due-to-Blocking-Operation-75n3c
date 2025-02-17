# Node.js Server Unresponsiveness

This repository demonstrates a common Node.js issue: server unresponsiveness caused by a long-running synchronous operation that blocks the event loop.  The `server.js` file contains the buggy code. The solution is provided in `serverSolution.js`.

## Problem

The server uses a `while` loop to simulate a long-running task. This blocks the event loop, preventing the server from responding to new requests or handling existing ones until the loop finishes.  This results in the server hanging and becoming unresponsive.