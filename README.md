# React Native useEffect Async Operation Error Handling

This repository demonstrates a common error in React Native when using the `useEffect` hook with asynchronous operations and provides a solution to prevent it.

## Problem

When performing asynchronous operations within the `useEffect` hook, there's a risk that the component might unmount before the asynchronous operation completes. This can lead to errors, particularly if you're trying to update state after the component has been unmounted.

## Solution

The solution involves using a cleanup function within `useEffect` to abort the asynchronous operation if the component unmounts.  This prevents errors and ensures a cleaner unmounting process.

## How to Run

1. Clone the repository.
2. Navigate to the project directory: `cd react-native-useeffect-async`
3. Install dependencies: `npm install`
4. Run the app: `npx react-native run-android` (or `npx react-native run-ios`)

## License

MIT