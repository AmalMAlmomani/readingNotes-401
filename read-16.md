# Event-Driven Programming in Node.js
  - is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

## Event-Driven Programming makes use of the following concepts:
  - 1. An Event Handler is a `callback function` that will be called when an event is triggered.
  - 2. A `Main Loop` listens for event triggers and calls the associated event handler for that event.

## Removing Listeners
   - To remove event listeners in EventEmitter we can use the *removeListener* or *removeAllListeners* method.
   -  It’s important to note that in the EventEmitter that comes built-in with Node you must pass a reference to the exact function you wish to remove when using the removeListener method. 

## Most actions in JS are event driven
   - UI Events
   - Express Routes
   - (soon) Model Lifecycle Hooks
   - (later) React … everything
    
## Object Oriented Programming + Event-Driven Programming
   - These two make for a very valuable combination in a wide variety of situations and I think it can be beneficial to understand and conceptualize why.