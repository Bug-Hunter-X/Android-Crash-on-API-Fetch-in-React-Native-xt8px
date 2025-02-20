## React Native Android API Fetch Crash

This repository demonstrates a bug in a React Native application where fetching data from a remote API causes the app to crash on Android, but functions correctly on iOS. The issue stems from inconsistent error handling during the API request, leading to unhandled exceptions on the Android platform.

### Problem

The provided `MyComponent` attempts to fetch data from `https://api.example.com/data`. On Android, the app crashes under certain network conditions or API response errors, whereas iOS manages these scenarios gracefully.

### Solution

The solution includes more robust error handling within the `useEffect` hook, ensuring that errors are properly caught and displayed to the user, preventing crashes.  The solution also adds logging to help diagnose issues.

### Setup

1. Clone this repository.
2. `cd` into the project directory.
3. Run `npm install` to install project dependencies.
4. Run the application on Android and iOS emulators or devices to observe the difference and effectiveness of the fix.
