# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications involving the `useEffect` hook.  The example shows an infinite loop caused by an improperly configured dependency array.  The solution provides the correct implementation to resolve the issue.

## Bug
The `bug.js` file contains a React component that increments a counter. The `useEffect` hook logs the current count to the console after every render. However, the dependency array is missing the `count` variable, causing the effect to run on every render and trigger an infinite loop.

## Solution
The `bugSolution.js` file corrects the bug by including `count` in the dependency array.  This ensures the effect runs only when the `count` variable changes, resolving the infinite loop.

This is a common mistake when using useEffect, so paying attention to the dependency array is crucial for avoiding performance issues and unexpected behavior.