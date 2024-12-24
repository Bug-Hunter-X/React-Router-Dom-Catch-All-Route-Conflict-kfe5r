# React Router Dom Catch-All Route Conflict

This repository demonstrates a common issue in React Router v6 where a catch-all route (`/*`) interferes with other defined routes. The problem arises when the catch-all route is placed before more specific routes, causing the catch-all route to always match, even when other routes should be selected.

## Problem
The provided `App.js` demonstrates this: a catch-all route (`/*`) is defined to show a 404 page. However, no matter which route is visited in the browser, the 404 page is always displayed. This is because the catch-all route is declared before the other routes, thus always matching first. 

## Solution
The solution, provided in `AppSolution.js`, demonstrates how to correct this by ordering the routes correctly. The more specific routes are now defined before the catch-all route, allowing the correct components to render. 

## How to run
1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install` to install the dependencies.
4. Run `npm start` to start the development server.