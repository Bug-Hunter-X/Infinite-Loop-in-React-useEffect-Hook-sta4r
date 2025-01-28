# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications: an infinite loop caused by a missing dependency in the `useEffect` hook's dependency array.

## Bug Description
The `MyComponent` function uses the `useEffect` hook to log the current value of the `count` state variable to the console.  However, the dependency array is missing `count`, causing the effect to re-run after every render, leading to an infinite loop and potentially crashing the application. 

## Bug Solution
The solution involves correctly specifying the `count` variable in the dependency array. This ensures that the effect only runs when the `count` variable changes.

## How to Reproduce
1. Clone this repository.
2. Run `npm install` to install the dependencies.
3. Run `npm start` to start the development server.
4. Open your browser and observe the infinite loop in the console.
