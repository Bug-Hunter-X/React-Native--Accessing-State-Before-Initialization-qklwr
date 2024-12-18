# React Native: Accessing State Before Initialization

This repository demonstrates a common error in React Native: accessing a state variable before it has been initialized.  The `bug.js` file shows the problematic code, while `bugSolution.js` presents a solution using the useEffect hook.

## Problem

In functional components, using the `useState` hook, attempting to read the state variable before the component mounts results in an undefined value. This can cause unexpected behavior or crashes, especially if the value is used in calculations or displayed directly. 

## Solution

The solution uses the useEffect hook to ensure the state variable is accessed only after the component has mounted.  Alternatively, conditional rendering can prevent rendering elements that depend on this state until it's initialized.

## How to Run

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npx react-native run-android` (or `npx react-native run-ios`) to start the app.
