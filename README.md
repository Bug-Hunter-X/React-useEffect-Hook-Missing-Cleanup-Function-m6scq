# React useEffect Hook Missing Cleanup Function

This repository demonstrates a common error in React applications: forgetting to include a cleanup function in the `useEffect` hook when using event listeners or other side effects.  This can lead to memory leaks and unexpected behavior.

## The Bug

The `bug.js` file contains a component that uses the `useEffect` hook to add an event listener for key presses. However, it is missing a return statement within the `useEffect` which contains a function to remove the event listener when the component unmounts.

## The Solution

The `bugSolution.js` file demonstrates the correct implementation, including the cleanup function to remove the event listener when the component is no longer needed.  This prevents memory leaks and ensures the component behaves predictably.

## How to Run

1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install` to install the necessary dependencies.
4. Run `npm start` to start the development server.