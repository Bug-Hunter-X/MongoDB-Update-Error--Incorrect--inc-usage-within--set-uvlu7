# MongoDB Update Error: Incorrect $inc usage within $set

This repository demonstrates a common error when using MongoDB's update operators. The error arises from attempting to use the `$inc` operator within a `$set` operation, which unexpectedly overwrites the field instead of incrementing it. The provided solution illustrates the correct way to achieve the intended behavior.

## Bug
The provided code tries to increment a counter field using `$inc` within a `$set` operation. This leads to the field being overwritten with an object instead of the incremented value.

## Solution
The solution provides the correct method using the `$inc` operator directly in the update operator, effectively incrementing the existing counter value without needing a `$set` operation.