# Express.js Route Handler Missing Error Handling

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid input.  Specifically, the `/users/:id` route fails to handle cases where the `id` parameter is not a valid number or when no user is found.

## Bug

The `bug.js` file contains the buggy code.  It attempts to find a user by ID, but doesn't handle cases where the ID is invalid or the user is not found. This can lead to unexpected behavior or crashes.

## Solution

The `bugSolution.js` file provides a corrected version. It includes explicit error handling for invalid user IDs and returns a more informative 404 response.