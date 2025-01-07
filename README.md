# F# Mutable Variable Swap Bug

This example demonstrates a common misconception when working with mutable variables in F#.  The `swap` function attempts to swap the values of two mutable variables, but it fails because F# passes arguments by value, not by reference. The function operates on copies of the variables, leaving the original variables unchanged.

The `bug.fs` file contains the buggy code. The `bugSolution.fs` file provides the corrected version.

## Bug
The `swap` function in `bug.fs` does not correctly swap the values of the mutable variables `x` and `y`.