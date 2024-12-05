# Silent Crash on Network Request Failure in React Native

This repository demonstrates a common yet subtle bug in React Native applications where network request failures result in silent crashes without providing any feedback to the user.  The issue stems from the lack of proper error handling within the asynchronous operation and the absence of a user-friendly error display mechanism.

## Bug Description

The provided `MyComponent` fetches data from a remote API.  While the `catch` block logs errors to the console,  it doesn't handle them in a way that prevents the app from crashing or informs the user about the failure.  This leads to a poor user experience and makes debugging more difficult.

## Solution

The solution involves enhancing the error handling to display a user-friendly message and potentially implement retry logic for transient network problems.
