# Hooks API

  - *Hooks* are a new addition in React 16.8.
  - is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.
  - are backwards-compatible
  - React hooks allow to to easily create and manage state in a `functional component`.

  - Hooks are JavaScript functions.

  - **Rules of Hooks**
    - 1. Hooks must be named with a use prefix (i.e. useFishingPole)
    - 2. Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions.
    - 3. Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions. (There is just one other valid place to call Hooks — your own custom Hooks. We’ll learn about them in a moment.)

  - **Built In Hooks**
    - Returns a stateVariable and setterFunction for you to use to manage state in a functional component

  - **When would I use a Hook?**
    - If you write a function component and realize you need to add some state to it, previously you had to convert it to a class. Now you can use a Hook inside the existing function component.

  - **Basic Hooks**
     - useState
     - useEffect
     - useContext
  - **Additional Hooks**
     - useReducer
     - useCallback
     - useMemo
     - useRef
     - useImperativeHandle
     - useLayoutEffect
     - useDebugValue

  - **When exactly does React clean up an effect?**
     - React performs the cleanup when the component unmounts. However, as we learned earlier, effects run for every render and not just once. 

  