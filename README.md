# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: creating an infinite loop by modifying the state within the dependency array.  The `bug.js` file contains the problematic code, while `bugSolution.js` provides the corrected version.

## Problem
The initial `useEffect` call in `bug.js` attempts to update the `count` state, triggering a re-render.  This re-render causes the `useEffect` hook to run again, leading to an infinite loop and potential application crashes. 

## Solution
The corrected code in `bugSolution.js` addresses the issue by using functional updates to the state, or by moving the state update to a different condition or effect.