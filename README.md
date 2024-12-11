# JavaScript Closure Issue in setTimeout Loop
This repository demonstrates a common closure issue in JavaScript when using `setTimeout` within a loop.  The problem arises because of how JavaScript handles closures and variable scoping.  The solution shows how to properly capture the loop variable's value using an immediately invoked function expression (IIFE).

## Problem
The `bug.js` file contains a function that intends to log numbers 0 through 9 with a 1-second delay between each log.  Due to a closure issue, it logs '10' ten times.

## Solution
The `bugSolution.js` file demonstrates the correct approach using an IIFE to immediately capture the current value of 'i' for each iteration.

## How to Run
1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in your preferred JavaScript environment.
3. Execute the `myFunction` within each file and observe the difference in output.