# React Native Uninitialized State Bug

This repository demonstrates a common error in React Native applications: accessing component state before it has been fully mounted.  The `bug.js` file showcases the problematic code, where an attempt is made to access and initialize state within the `constructor` before the component has fully mounted. This results in `undefined` being returned for state values.

The `bugSolution.js` file provides a corrected version where state initialization and data fetching are moved to the `componentDidMount` lifecycle method, ensuring the component is fully mounted and state is properly initialized.