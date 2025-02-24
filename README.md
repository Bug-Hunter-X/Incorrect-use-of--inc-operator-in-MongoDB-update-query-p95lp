# Incorrect use of $inc operator in MongoDB update query
This example demonstrates a common error when using the `$inc` operator in MongoDB update queries. The `$inc` operator is used to increment a numerical field by a specified value. However, this code provides a string value, which causes an error.

## Bug
The bug lies in the usage of the `$inc` operator.  The value being incremented should be a number, not a string.  Attempting to increment by a string will throw a MongoDB error.

## Solution
The solution is to provide a numerical value to the `$inc` operator.
