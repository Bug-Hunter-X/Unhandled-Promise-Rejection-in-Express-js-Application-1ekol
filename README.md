# Unhandled Promise Rejection in Express.js Application
This repository demonstrates a common error in Express.js applications: unhandled promise rejections.  Asynchronous operations are frequently used in Express.js but neglecting proper error handling can lead to application crashes without helpful error messages.

## Bug Description
The `bug.js` file showcases an Express.js app with an asynchronous operation (`someAsyncOperation()`) that might throw an error.  The `catch` block for handling errors is missing, causing the promise rejection to be unhandled, resulting in a crash.

## Solution
The `bugSolution.js` file demonstrates the correct approach. The `catch` block handles the potential error, providing better error handling and preventing crashes.