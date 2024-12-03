# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers:  the lack of proper error handling when dealing with user input.  Specifically, the example code attempts to parse a user ID from the request parameters as an integer without checking for non-numeric input, which can lead to application crashes or unexpected behavior.  The solution shows how to add robust error handling to prevent these issues.

## Bug

The `bug.js` file contains the erroneous code. It defines a route that fetches user data based on the ID passed in the request parameters.  However, it fails to handle cases where the `userId` is not a valid number.

## Solution

The `bugSolution.js` file demonstrates a corrected version of the code.  It includes explicit checks to ensure the `userId` is a number before attempting to parse it, thereby preventing potential errors.