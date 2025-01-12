# Unhandled JS Exception: Cannot read properties of undefined (reading '...state variable...')

This repository demonstrates a common error in React Native applications: attempting to access a state variable before it has been initialized.

## Problem
The error message "Unhandled JS Exception: Cannot read properties of undefined (reading '...state variable...')" appears when you render a component that uses a state variable before the component mounts and sets the initial state. This usually happens during the initial render or when using asynchronous operations.

## Solution
The solution is to use the optional chaining operator (`?.`) or the nullish coalescing operator (`??`) to safely access the state variable and handle the potential undefined state, or to only access the state after its initialization, such as inside useEffect with an empty dependency array or by using conditional rendering.