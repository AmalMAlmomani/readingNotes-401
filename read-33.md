# Context API

  - `Context` provides a means of passing state down the component tree through a Provider/Consumer relationship.

  - **When to Use Context**
    - Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. 

  - **Before You Use Context**
    - Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

  - **Updating Context from a Nested Component**
    - It is often necessary to update the context from a component that is nested somewhere deeply in the component tree.

  - **Consuming Multiple Contexts**
   - To keep context re-rendering fast, React needs to make each context consumer a separate node in the tree.

# Two ways to attach to context:
  - Wrap your component with, and use a function to “get” the context object itself.
Statically declare a connection to the context provider and then use.


# Context API in React (Hooks and Classes) React Context API 
  - is a way to essentially create global variables that can be passed around in a React app. This is the alternative to "prop drilling", or passing props from grandparent to parent to child, and so on.


- ![](./img/hooks.png)