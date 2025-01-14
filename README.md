# MongoDB $inc Operator Unexpected Behavior
This repository demonstrates a common error when using the `$inc` operator in MongoDB updates. The `$inc` operator is used to increment a numerical field by a specified value.  However, if the field does not exist or is not of numerical type, unexpected behavior can occur.  The solution shows how to handle these scenarios appropriately, including using the `$setOnInsert` operator for new documents and checking for the presence of the field and its data type before attempting an increment.

## Bug
The bug is found in the way the `$inc` operator is utilized, not checking for the existence or data type of the field before incrementing it. This can lead to errors or incorrect updates.