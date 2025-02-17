# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug: an infinite loop caused by an incorrectly specified dependency array in the `useEffect` hook.

## Bug Description
The `MyComponent` component uses `useEffect` to log the current count. However, the dependency array is missing a key dependency, causing the effect to run on every render.

## How to Reproduce
1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console output and button behavior.

## Solution
The solution involves correctly specifying the `count` variable in the dependency array of useEffect.