# Incorrect console.log usage in useEffect hook
This example demonstrates an uncommon error in React where incorrect usage of `console.log` inside the useEffect hook can lead to unexpected behavior.  Specifically, using simple string concatenation when logging variables might not produce the expected output, especially with non-string values.

The `bug.js` file showcases the problem, while `bugSolution.js` provides the corrected code.

## Problem
The issue arises from the way we try to log the `count` variable. Instead of using template literals for string interpolation, we are using simple string concatenation. This can be problematic when logging values that aren't strings, leading to unexpected outputs or even errors.

## Solution
The solution involves using template literals (backticks) to properly embed the `count` variable within the log message. This ensures the correct output, regardless of the type of variable being logged.