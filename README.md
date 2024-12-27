# React 19 useEffect Hook Bug

This repository demonstrates a common error when using the `useEffect` hook in React 19.  Directly modifying state variables inside `useEffect` does not trigger a re-render.  The solution shows the correct way to update state using the setter function.

## Bug
The `bug.js` file contains the buggy code where the state variable `count` is modified directly without using the `setCount` function, leading to an incorrect state update and no re-render.

## Solution
The `bugSolution.js` file demonstrates the correct solution.  The state is updated using the `setCount` function provided by the `useState` hook. This ensures that React correctly updates the component and triggers a re-render.