# Julia Bug: Unexpected Exponentiation Behavior
This repository demonstrates a subtle bug in a Julia function related to exponentiation with negative numbers. The function `myfunction` aims to square the input, handling positive and negative numbers differently. However, the use of the `^` operator leads to unexpected results for negative numbers and non-integer exponents.

## Bug Description
The issue stems from the way Julia's `^` operator handles negative bases and non-integer exponents.  The expected behavior is to return always the square of a number, regardless of its sign. The solution provides a corrected version that explicitly handles the squaring operation to produce correct results for all inputs.

## How to Reproduce
1. Clone this repository.
2. Run `bug.jl`. Observe the unexpected output for negative input.
3. Run `bugSolution.jl` to see the corrected version's behavior. 

## Solution
The solution involves explicitly handling the squaring operation using multiplication instead of the `^` operator. This ensures that the function always returns the correct squared value regardless of the input's sign.