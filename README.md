# Null Value Handling in JavaScript Addition Function

This repository demonstrates a common error in JavaScript related to handling null values in functions.

## The Bug
The `foo` function adds two numbers together. However, it does not correctly handle cases where one or both of the input parameters are null.  This leads to unexpected results, as shown in the provided test cases. Specifically, the expectation is that when null is passed as a parameter, the function should return a 0. This does not happen because javascript does not implement the expected type checking needed in this example, as a result the function will return NaN which will cause a runtime error in the case of the use of null parameters.

## The Solution
The solution involves explicitly checking for null values and handling them appropriately. The fixed function returns 0 if either parameter is null, ensuring consistent and expected behavior.

## How to Run
1. Clone this repository.
2. Open `bug.js` to see the buggy code.
3. Open `bugSolution.js` to see the corrected code.
4. Run `node bug.js` and `node bugSolution.js` to see the difference in output.