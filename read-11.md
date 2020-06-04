#  Authentication


## User Modeling
  - **have sensitive data that should NEVER be sent to client applications.**
  - Modern web applications need to model sensitive information about their users.
  - users password, should be encrypted using a hashing algorithm before it is ever stored.
  - hash password can be stored when the user signs up. When the user needs to login


## Cryptography
  - is the science which studies methods for encoding messages so that they can be read only by a person who knows the secret information required for decoding, called the `key`; it includes `cryptanalysis`, the science of decoding encrypted messages without possessing the proper key, and has several other branches.


## Cryptographic Hash Algorithm
  -  takes a piece of data and produces a hash that is deliberately difficult to reverse.


## Cryptographic Cypher Algorithm
   - takes a piece of data and a key and produces encrypted data. Later the encrypted data can be reversed into the original data by decrypting it using the same key.


## Basic Authorization
   - is a common method used to send a username and password in an HTTP request. The username and password are joined with a `‘:’ ` then ` “base64 encoded” `and placed after the string `‘Basic ‘.` The resulting string is set to the value of an Authorization header.
   - A Server can decode the Basic Authorization header to retrieve the username and password. 

  - **NOTE: base64 encoding is not a form of encryption. The client and server must use HTTPS to protect the username and password as it travels across the network.**