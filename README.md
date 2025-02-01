# React Native: Undefined is not an object (evaluating 'this.state.property')

This repository demonstrates a common React Native error: 'Undefined is not an object (evaluating 'this.state.property')'. This typically happens when trying to access a state variable or prop before it's been initialized.

## Bug Reproduction

The `bug.js` file shows the buggy code.  Running this will result in the error because `this.state.data` is accessed before the data is fetched and set in `componentDidMount`. 

## Solution

The `bugSolution.js` file provides a fix by using optional chaining or conditional rendering to handle the case where `this.state.data` might still be null.