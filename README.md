# Unexpected Behavior with Consecutive useState Updates in React

This repository demonstrates a subtle bug related to consecutive updates within a React component using the `useState` and `useEffect` hooks.  The core problem highlights how multiple calls to `setCount` in rapid succession can lead to unexpected behavior and potentially missed updates.

## Bug Description
The `bug.js` file contains a simple counter component. The `handleClick` function increments the count twice using `setCount`. Because of this, the useEffect hook might not update to the final value of the count.