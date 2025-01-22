# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating through arrays.  The error arises from incorrectly handling the loop termination condition.  The provided code and its corrected version illustrate the problem and its solution.

**Problem:**
The original `bug.java` file contains a `for` loop that iterates from `i = 0` to `i <= arr.length`.  In Java, arrays are zero-indexed, meaning the last valid index is `arr.length - 1`.  Therefore, the loop attempts to access an index that is out of bounds, causing an `ArrayIndexOutOfBoundsException`.

**Solution:**
The `bugSolution.java` file corrects the error by changing the loop condition to `i < arr.length`. This ensures that the loop iterates only up to the last valid index of the array.

This example highlights the importance of careful attention to array indices to avoid common runtime exceptions in Java.