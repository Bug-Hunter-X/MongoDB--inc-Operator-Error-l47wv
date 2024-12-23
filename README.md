# MongoDB $inc Operator Error

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment or decrement a numeric field.  However, passing a non-numeric value as an argument will lead to unexpected results.

**The bug:** The provided code attempts to increment the `count` field with the string value '1'.  MongoDB expects a numeric value in this context. 

**Solution:** The solution is to provide a numeric value to the `$inc` operator. 