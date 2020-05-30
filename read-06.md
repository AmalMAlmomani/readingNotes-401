# HTTP and REST

## HTTP(Hyper Text Transfer Protocol):
  - stateless request-response application layer protocol. 
  - used to build distributed, collaborative, hypermedia information systems. 
  - the foundation for the world wide web.
  -  In the client-server computing model a host designed to provide a service is called a `server`
  - defines how requests and responses should be formatted, but not what a service should represent.
  - associated with serving `.html` files but is also used to transfer `images`, `videos`, `.json`, `.xml`, `binary executables`, and much more.

  - ![](http1-url-structure.png) 

### HTTP Requests
  - HTTP/1.1 request is formatted in text and transferred using TCP.
  - The first line of the request contains the `METHOD`, `URL`, and `HTTP VERSION`.
  - `Safe` methods should only be used for information retrieval and should not change the server state.
  - `Idempotent` methods means if two identical requests are made they should get an identical response. 
  - `Cacheable` means the client should be able to cache the response.

### HTTP Response
  - HTTP/1.1 response is also formatted in text and transferred using TCP. 
  - The first line of the response contains the `HTTP VERSION`, `STATUS CODE`, and `STATUS MESSAGE`.
 

## REST(REpresentational State Transfer):
  - is a means by which we can reference, manipulate, and transfer state.
  - uses a common set of methods (called `verbs`) to operate on the state of a resource (`noun`), generally using *HTTP as the transfer protocol*.
  - **RESTful Endpoint:** URI that identifies the resource. When addressed with a proper method, you are able to effect state.
  - RESTful Endpoint: *http://api.server.com/api/v1/people*
    - http:// - Protocol/Scheme
    - api.server.com - Domain or Server
    - /api/v1 - API Endpoint
    - /people - The resource (This identifies a collection: all people)
    - /people/12345 - A more specific resource: The person with id 12345
  - Generally speaking, RESTful endpoints deliver data in JSON format. 
  - **The best practice is to supply a header with metadata and a collection of results**
 
  - ![](http1-req-res-details.png)

### REST Documentation (Swagger):
  - standard for documenting REST APIs is with a “live” documentation system: Open API (formerly “Swagger”).
  - allows for live requests from with it.