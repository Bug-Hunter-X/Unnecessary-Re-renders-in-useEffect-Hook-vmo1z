# Unnecessary Re-renders in React useEffect Hook

This repository demonstrates a common issue with the React `useEffect` hook: unnecessary re-renders due to an improperly defined dependency array.

The `bug.js` file shows the initial code with the issue, where the `useEffect` hook runs on every render because it has no dependency array, causing it to log every render.

The `bugSolution.js` file shows the corrected code where the `useEffect` hook only runs when the `count` variable changes, fixing the unnecessary renders.

## How to reproduce

1. Clone this repository
2. Run `npm install`
3. Run `npm start`
4. Observe the console logs in the `bug.js` example and note the frequent logging.
5. Observe the console logs in the `bugSolution.js` example and note that logging happens only when the button is clicked.