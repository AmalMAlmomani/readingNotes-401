# React Testing and Deployment

## React Testing 
  - `Snapshots` - Make assertions on the exact rendered markup (with content) at any state of the application.
  - `Render Testing` - Similar to snapshots, but allows for jQuery-like inspection of the virtual DOM tree
  - `Shallow Testing` - Executes and renders the called/container component, but does not compose children.
  - `Mounting` - Executes the full component and children. Allows for inspection of rendered Virtual DOM as well as the current state


## Deployment
  - React in development mode uses a node service to create a live website that refreshes as you write code.

## Snapshot Testing
  - are a very useful tool whenever you want to make sure your UI does not change unexpectedly.

## Static Rendering API
  - Use enzyme's `render` function to generate HTML from your React tree, and analyze the resulting HTML structure.

## Full Rendering API (mount(...))
  - Full DOM rendering is ideal for use cases where you have components that may interact with DOM APIs or need to test components that are wrapped in higher order components.