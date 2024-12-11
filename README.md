# React Router v6 useParams Issue

This repository demonstrates a common issue encountered when using the `useParams` hook in React Router v6.  The problem occurs when attempting to access route parameters from a component that is not directly nested within a route defined using the `<Route>` component. This leads to `useParams` returning an empty object, causing errors in accessing parameter values.

The `brokenCode.js` file showcases the problematic code.  `fixedCode.js` provides the corrected implementation.

## Solution

The solution involves ensuring that the component using `useParams` is either directly within a route or is passed the necessary parameters via props from an ancestor component that is within a route.