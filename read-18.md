# Socket.io
  - It is a library which enables real-time and full duplex communication between the Client and the Web servers.
  - It uses the WebSocket protocol to provide the interface.
    - Client Side: it is the library that runs inside the browser
    - Server Side: It is the library for Node.js

## Web Sockets
  - remains open all the time so they allow the real-time data transfer.

  - **Key features of WebSocket:**
    - WebSocket helps in real-time communication between the Client and the web server.
    - This protocol helps in transforming to cross-platform in a real time world between the server and the client.
    - This also enables the business around the world for real-time web application to enhance and to increase the feasibility.
    - The major advantage it stands over an HTTP connection that it provides full duplex communication.


    - ![](./img/WebSocket-protocol-schema.png)

## Messaging
  - Standard node events are sent with `emit()` and received with `on()` … Socket.io uses the same methodology/terminology.

  
  - **Not every client will have a listener for every event.**
  - **The server may not have a listener for every event a client sends.**