# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook and its dependency array. The bug causes an infinite loop due to a missing dependency in the `useEffect`'s dependency array. The solution involves correctly specifying the dependency array to prevent the infinite loop.

## Bug
The `bug.js` file contains the buggy component. The `useEffect` hook's dependency array is missing `count`, leading to infinite re-renders. 

## Solution
The `bugSolution.js` file shows the corrected component.  The dependency array now includes `count`, ensuring the effect only runs when `count` changes.