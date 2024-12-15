# C++ Off-by-One Error Example

This repository demonstrates a common off-by-one error in C++ when iterating over a vector.  The error occurs because the loop condition is `i <= vec.size()`, which attempts to access an element beyond the valid range of the vector.  This leads to undefined behavior and potential crashes.

The `bug.cpp` file contains the erroneous code. The `bugSolution.cpp` file provides the corrected version.

## How to Reproduce

1. Compile `bug.cpp` using a C++ compiler (like g++).
2. Run the executable.  You'll likely see undefined behavior, a crash, or incorrect output.
3. Compile and run `bugSolution.cpp` to see the corrected behavior.

## Solution

The solution involves correcting the loop condition to `i < vec.size()`, which ensures that the loop iterates only through valid indices of the vector.