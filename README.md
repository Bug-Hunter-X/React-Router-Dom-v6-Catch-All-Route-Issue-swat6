# React Router Dom v6 Catch All Route Issue

This repository demonstrates a common issue encountered when using the catch-all route (`*`) in React Router v6.  The issue is that the catch-all route doesn't function correctly, and the 404 component is always displayed, even when other routes should be matched. This is often due to incorrect route ordering or other conflicts within the route configuration.

## The Problem
The provided `App.js` file contains a simple React Router v6 setup. Despite having defined routes for `/` and `/about`, the catch-all route (`*`) always gets matched, leading to the 404 page being rendered. 

## Solution
The solution involves ensuring that the catch-all route is always placed last within the `Routes` component.  If other routes are placed after the catch-all, they will never be matched. This is demonstrated in `AppSolution.js`

## How to Run
1. Clone this repo.
2. Navigate to the project directory.
3. Run `npm install`.
4. Run `npm start`. 