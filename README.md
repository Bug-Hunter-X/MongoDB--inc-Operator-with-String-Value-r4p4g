# MongoDB $inc Operator with String Value

This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries. The `$inc` operator is used to increment a numerical field by a specified value. However, if a string value is provided instead of a number, MongoDB will not behave as expected, potentially leading to data corruption or unexpected results.

## Bug Description
The provided code snippet attempts to increment the `count` field by 1 using the `$inc` operator, but instead provides '1' (string). This causes MongoDB to treat '1' as a string, leading to unexpected outcomes rather than an increment.

## Bug Solution
To correct this issue, provide a numerical value as the argument to the `$inc` operator.