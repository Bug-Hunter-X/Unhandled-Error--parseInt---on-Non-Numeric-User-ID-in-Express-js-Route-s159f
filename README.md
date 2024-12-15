# Unhandled parseInt Error in Express.js Route

This repository demonstrates a common error in Express.js route handlers:  failure to handle potential errors when parsing user input. Specifically, the code attempts to parse a user ID as an integer without checking if the input is actually numeric.  This can lead to unexpected crashes or incorrect behavior.

## Bug

The `bug.js` file contains the buggy code.  It lacks error handling for the case where the `:id` parameter in the route is not a valid integer.

## Solution

The `bugSolution.js` file provides a corrected version of the code. It includes checks to ensure the user ID is a number before attempting to parse it, preventing the potential error.