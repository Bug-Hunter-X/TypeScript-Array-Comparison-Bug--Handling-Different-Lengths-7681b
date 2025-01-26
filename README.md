# TypeScript Array Comparison Bug

This repository demonstrates a common error in TypeScript when comparing arrays: the failure to handle arrays of different lengths.

The `bug.ts` file contains a function `compareArrays` that incorrectly compares arrays. It only compares elements at the same index and returns `false` if they differ, without considering the possibility of different array lengths.

The `bugSolution.ts` file provides a corrected version of the `compareArrays` function which addresses the length mismatch issue.  This corrected version first checks the lengths of the arrays before proceeding to the element-wise comparison, leading to accurate results.

## How to Reproduce

1. Clone this repository.
2. Open `bug.ts` and observe the incorrect comparison logic.
3. Run the code using a TypeScript compiler (like tsc) and node.js.
4. Observe the incorrect output for arrays with differing lengths.
5. Open `bugSolution.ts` and see the corrected logic.
6. Run the corrected code to see the accurate output.
