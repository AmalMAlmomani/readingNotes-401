# OAuth

## OAUTH2.0
  -  is an open standard for access delegation, commonly used as a way for Internet users to grant websites or applications access to their information on other websites but without giving them the passwords.
  - an open standard for access delegation
  - OAuth serves as a way to give users the ability to grant application access to services, without giving the application their password.

## How does OAuth work?
  - Through a series of “handshakes”, an application such as an Express Web Server asks the user if it’s ok to login as them at some remote service, and then begins the process of authentication and access.

  - The token is the user

## Access Code
  - `<a>`
  - `response_type=code` indicates that your server wants to receive an authorization code
  - `client_id=<your client id>` tells the authorization server which app the user is granting access to
  - `redirect_uri=<your redirect uri>` tells the auth server which server endpoint to redirect to
  - `scope=<list of scopes>` tells the auth server what you want the user to give access to
  - `state=<anything you want>` a place where you can store info to pass to your server if you want


## Access Token
  - `POST`
  - `grant_type=authorization_code`
  - `code=<the code your received`
  - `redirect_uri=REDIRECT_URI `must be same as the redirect URI your client provided
  - `client_id=<your client id>` tells the authorization server which application is making the requests
  - `client_secret=<your client secret>` authenticates that the application making the request is the application registered with the `client_id`
  - Once you get an access token, you can use it to make API calls to the service on behalf of that user