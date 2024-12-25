# React Native FlatList: Non-Unique Keys Error

This repository demonstrates a common error encountered when using the `FlatList` component in React Native: providing non-unique keys to the `keyExtractor` prop.

The `bug.js` file shows the problematic code, where the `keyExtractor` function returns non-unique keys, leading to incorrect rendering.  The `bugSolution.js` file provides the corrected implementation.

## Reproducing the Error

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app. Observe the incorrect rendering of list items.

## Solution

The solution involves ensuring that the `keyExtractor` function returns a unique string or number for every item in the `data` array.  This is crucial for efficient and correct rendering in FlatList.