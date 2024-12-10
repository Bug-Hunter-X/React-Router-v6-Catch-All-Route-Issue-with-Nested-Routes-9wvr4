This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router v6, specifically when dealing with nested routes. The problem arises because the catch-all route intercepts all unmatched routes, preventing nested routes from working as expected.

The `App.js` file shows the problematic code where a catch-all route is placed after other specific routes. This causes all navigation attempts to be caught by the `NotFound` component, even if a nested route was intended.

The solution, shown in `AppSolution.js`, involves reorganizing the routes.  The catch-all route should be placed last. In this specific scenario, no changes are necessary.  However, the problem occurs when other routes exist after the catch-all route.