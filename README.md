# React useEffect Dependency Array Error
This repository demonstrates a common error in React's `useEffect` hook: forgetting to include state variables in the dependency array.  Incorrectly omitting dependencies can lead to infinite render loops or unexpected behavior.

The `bug.js` file shows the problematic code. The `bugSolution.js` file provides the corrected version.

## How to reproduce
1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console logs and the behavior of the button.

## Solution
The solution involves adding the `count` variable to the dependency array of the `useEffect` hook.  This ensures that the effect only runs when the `count` value changes.