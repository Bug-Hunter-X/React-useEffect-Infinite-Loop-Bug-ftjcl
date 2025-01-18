# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug arises from an incorrect dependency array, leading to an infinite render loop.

## Bug Description
The provided `MyComponent` uses `useEffect` to log the current count. However, the `count` variable is not included in the dependency array, causing the effect to run after every render, regardless of whether the count actually changed. This creates an infinite loop.  The solution involves correctly specifying the dependency array to only trigger the effect when the `count` value changes.

## How to Reproduce
1. Clone this repository.
2. Run `npm install` to install the necessary packages.
3. Run `npm start` to start the development server.
4. Observe the infinite loop in your browser's console.