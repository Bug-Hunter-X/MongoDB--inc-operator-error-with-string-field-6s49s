# MongoDB $inc Operator Error with String Field

This repository demonstrates an uncommon error in MongoDB when using the `$inc` operator with a string field.  The `$inc` operator is designed to increment numeric fields, and attempting to use it on a string field will lead to an error.

## Bug

The `bug.js` file contains code that attempts to increment a string field using `$inc`. This will result in a MongoDB error, indicating that the field is not a number.

## Solution

The `bugSolution.js` file shows the correct approach.  Before incrementing, you either need to ensure the field is a number, or use a different approach such as updating the field by concatenating a number or other string value.