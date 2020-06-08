# Bearer Authorization

  - `Basic Authentication` (where your username and password are transmitted to a server) 
  - `OAuth` (where there is a cumbersome handshaking/authorization process)

## Bearer Tokens:
  - are encoded JSON objects that “bear” or “contain” enough information for the server to assert that any client request that presents a valid token must have originated from a client that has previously authenticated themselves using either Basic or OAuth.
    - Bearer Tokens are sent to the user/client after the initial `signin` process has completed.
    - Clients must make every subsequent request to the server with that token, in the header
       - *Authorization: Bearer encoded.jsonwebtoken.here*
    - The server opens the token, does the re-authentication, and then grants or denies access
    - In express servers, this can be done in middleware, in conjunction with a user model.

## JSON Web Tokens(JWT)
  - open standard that defines a compact and self-contained way for securely transmitting information between parties (servers, clients, etc) as a JSON object. 
  - can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.


### When should you use JSON Web Tokens? 
  - **Authorization**: 
    - Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token.
    -  Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.

    - ![](./img/client-credentials-grant.png)

  - **Information Exchange**:
   -  JSON Web Tokens are a good way of securely transmitting information between parties. 
   - Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are.

