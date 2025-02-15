# Unexpected Behavior with Null Values and Strict Equality in JavaScript

This repository demonstrates a common JavaScript bug related to handling null values with the strict equality operator (`===`).  The provided `foo` function aims to return 0 if either input `a` or `b` is null. However,  loose comparison using `==` leads to unexpected behavior when comparing null and other data types like numbers or strings.

## Bug Description:
The function's `if` statement uses strict equality (`===`), which correctly identifies `null` only. It might not behave as expected if 'a' and 'b' are of different types that evaluate to 'falsy' but are not strictly equal to null.

## Solution:
The solution employs more robust null checks using the loose comparison operator (`==`) to handle null values more accurately. This approach ensures better behavior in various scenarios. 
