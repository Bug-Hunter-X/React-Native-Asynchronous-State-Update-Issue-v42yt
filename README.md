# React Native Asynchronous State Update Bug

This repository demonstrates a common bug in React Native applications involving asynchronous operations and state updates within the `useEffect` hook. The original code fails to properly update the component's state after fetching data asynchronously.

The solution provided correctly handles the asynchronous operation and updates the state, ensuring the component re-renders with the fetched data.

## Bug Description

The bug occurs when an asynchronous operation (in this case, a `fetch` call) is performed inside a `useEffect` hook. The component renders before the asynchronous operation completes, resulting in the state remaining unchanged.  The component displays 'Loading...' indefinitely.

## Solution

The solution addresses this issue by appropriately handling the asynchronous response and ensuring the component updates its state correctly after the data is fetched.