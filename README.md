# Incorrect Object Comparison in useEffect Hook

This repository demonstrates a common error in React's `useEffect` hook: incorrectly comparing objects for changes.  The example uses a shallow comparison (`!==`), which only checks for reference equality. This means that if the object's properties change, the comparison might not detect it, leading to unexpected behavior or infinite loops.

The `bug.js` file shows the incorrect implementation. The `bugSolution.js` file provides the corrected version using a deep comparison library or custom comparison logic.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console logs and the component's behavior.

## Solution

The solution uses a deep comparison library like Lodash's `isEqual` to correctly detect changes in the object's properties.
