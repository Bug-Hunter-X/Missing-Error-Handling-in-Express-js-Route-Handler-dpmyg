# Express.js Route Handler Error

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input.  The example shows a route that fetches a user by ID.  If the ID is not a valid number, the application will crash or return an unexpected error.  The solution demonstrates how to add proper error handling to prevent this.

## Bug
The original code attempts to parse the user ID as an integer without checking for errors. If the ID is not a valid number, this will result in a runtime error.

## Solution
The solution adds input validation and proper error handling. It checks if the ID is a valid number before attempting to parse it and includes a robust error response for invalid input.