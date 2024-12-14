# React 19 useEffect Bug

This repository demonstrates a common bug encountered in React 19 where the `useEffect` hook runs more times than expected, causing performance issues and potential state update inconsistencies.

## Bug Description

The provided code contains a `useEffect` hook that logs the current count.  Without proper dependency array management, the `useEffect` runs every time the component renders, instead of only when the count changes.

## Solution

The solution involves correctly specifying the dependency array for the `useEffect` hook. Including `count` ensures the effect only runs when the `count` value changes.

## How to Reproduce

1. Clone the repository.
2. Run `npm install` to install the necessary dependencies.
3. Run `npm start` to start the development server.
4. Observe the console logs and how the `useEffect` function's log appears more often than expected.