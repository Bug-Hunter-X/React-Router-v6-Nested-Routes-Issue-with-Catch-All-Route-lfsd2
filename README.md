# React Router v6 Nested Routes Issue
This repository demonstrates a common issue encountered when using nested routes with React Router v6 and a top-level catch-all route (`*`). The catch-all route unintentionally intercepts all requests, preventing nested routes from being matched.

## Problem
The provided `App.js` demonstrates the problem. Nested routes within a parent route will not render because the `*` route in the `Routes` will always match first. 

## Solution
The solution is provided in `AppSolution.js` and involves re-ordering the routes to place the catch-all route as the last route in the `Routes` component.
