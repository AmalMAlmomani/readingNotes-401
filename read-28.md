# Props and State

## Forms and Inputs
  - `form` elements maintain internal state.
  - Each `input` has an *onChange* event that we can handle and use to update our form-container’s state each time the user interacts with an input.

# Props

  - Components accept arbitrary inputs called props.
  -  In JSX, props are passed into a component with a syntax that looks like HTML attributes. These are the equivalent of function params.
  - `props` is the name of the object passed into a component constructor and any prop added to a component in the JSX will be accessible as a property on props.
  - **Props can be data or functions**

- `setState()` is the only legitimate way to update state after the initial state setup. 

## Handling Events 
  - is very similar to handling events on DOM elements.
  - **There are some syntax differences:** 
    - 1. React events are named using camelCase, rather than lowercase.
    - 2. With JSX you pass a function as the event handler, rather than a string.

## Forms
  - work a little bit differently from other DOM elements in React, because form elements naturally keep some internal state. 

## State and Lifecycle
   - **Converting a Function to a Class**
      - 1. Create an ES6 class, with the same name, that extends React.Component.
      - 2. Add a single empty method to it called render().
      - 3. Move the body of the function into the render() method.
      - 4. Replace props with this.props in the render() body.
      - 5. Delete the remaining empty function declaration.



- `Components` let you split the UI into independent, reusable pieces, and think about each piece in isolation. 

 
