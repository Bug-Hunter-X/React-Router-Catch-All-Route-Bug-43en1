# React Router Catch-All Route Bug

This repository demonstrates a common issue with React Router's catch-all route (`/*`).  The problem arises when the catch-all route is placed before other specific routes. This causes the catch-all route to always match, preventing other routes from being accessed. This example shows how to correctly order routes to solve the problem.

## Bug
The `App.js` file contains a React Router configuration with the catch-all route (`/*`) placed before other routes.  This causes all navigation requests to be intercepted by the `NotFound` component, regardless of the URL.