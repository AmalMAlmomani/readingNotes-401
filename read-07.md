# Express

## Express Routing
  - Event driven system
    - `app.get('/thing', (req,res) => {})`
      - **The Request Object**
        - parameters `app.get('/api/:thing',...) = req.params.thing`
        - Query Strings `http://server/route?ball=round = req.query.ball`
      - **The Response Object**
        - Responsible for sending data back to the browser
        - Has methods like `send()` and `status()` that Express uses to format the output to the browser properly
          - Sends Headers
             - Cookies
             - Status Codes


## Express Middleware: 
   - series of functions that the request “goes through”
   - Each function receives request, response and next as parameters
   - Types of middleware: *Application* and *Route*
   - **Application Middleware**
      - Error Handling
      - Bringing in other routes
      - Applies Defaults
      - JSON, Body and Form Parsing
      - Runs on every request
    - **Route Middleware**
      - Dealing with specific things for a route
      - Generally, things many routes would participate in
        - Are you logged in?
        - What is your IP?
        - Have we seen you here before?

## CRUD Operations with REST and Express
  - CREATE
    - `app.post('/resource')`
  - READ
    - `app.get('/resource')`
  - UPDATE
    - `app.put('/resource/:id')`
  - DESTROY
    - `app.get('/resource/:id')`

## Server Testing
  - Then, you can use supertest to run your tests
    - *This will hit your routes as though your server was running, without actually starting it*
    - *That’s one less thing to go wrong (eliminate variables when testing!)*
  - you can wrap superagent in a module (the demo code created an agent.js module that does this)
  