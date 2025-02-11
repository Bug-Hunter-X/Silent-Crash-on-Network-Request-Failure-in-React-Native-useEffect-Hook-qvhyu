# Silent Crash on Network Request Failure in React Native useEffect Hook

This repository demonstrates a common but subtle bug in React Native applications involving network requests within the `useEffect` hook.  The application crashes silently without providing any feedback to the user when the network request fails. This is due to an improper handling of errors within the asynchronous operation.

## Bug Description

The provided code attempts to fetch data from a remote API.  If the fetch fails (due to network issues, server errors, or other reasons), the application crashes without displaying an error message to the user. This makes debugging and user experience problematic.

## Solution

The solution involves properly handling potential errors within the `try...catch` block and providing feedback to the user or implementing appropriate error handling mechanisms.