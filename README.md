# React useEffect Hook Misuse

This repository demonstrates a common mistake when using the `useEffect` hook in React.  The provided code example shows an effect that runs on every render, leading to unnecessary re-renders and potential performance issues.

## The Problem

The `useEffect` hook in the `bug.js` file is missing the dependency array.  This means that the effect runs after every render, even if the `count` variable hasn't changed. This can lead to unintended consequences, such as excessive logging or unnecessary API calls. 

## The Solution

The `bugSolution.js` file demonstrates the correct usage. By including `[count]` as the dependency array, the effect now runs only when the value of `count` changes. This ensures that the effect executes efficiently and only when necessary.

## How to run

1. Clone this repository.
2. Navigate to the repository in your terminal.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.  You can then view both bug and solution version in your browser.