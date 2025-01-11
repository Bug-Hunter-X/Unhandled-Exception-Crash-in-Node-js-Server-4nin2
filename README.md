# Node.js Unhandled Exception Handling

This repository demonstrates a common error in Node.js applications: unhandled exceptions that cause the server to crash without proper error handling.  The `server.js` file contains the problematic code, while `serverSolution.js` provides a corrected version with improved error handling.

## Problem

The original server lacks a mechanism to catch and handle exceptions that might occur during request processing. This leads to unexpected crashes and downtime.

## Solution

The solution involves using a `try...catch` block to wrap the request handling logic.  This allows the server to gracefully handle errors, log them for debugging, and potentially send a more informative response to the client.