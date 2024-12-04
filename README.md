# Node.js Server Crash Bug

This repository demonstrates a bug in a Node.js server that causes intermittent crashes under heavy load. The crashes are due to unhandled exceptions within asynchronous operations. The solution involves using a robust error handling mechanism to prevent crashes and provide better logging of exceptions.

## Bug Description

The server, implemented using the `http` module, appears to function correctly under normal conditions. However, when subjected to a high volume of requests, it intermittently crashes without any clear indication of the root cause.  This is due to the lack of proper exception handling in asynchronous code.