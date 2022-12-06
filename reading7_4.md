# Reading

## Intro to JWT

1. What is a JSON Web Token (JWT)?

- SON Web Token is a proposed Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims. The tokens are signed either using a private secret or a public/private key.

2. When should we use JSON Web Tokens?

- is as an API authentication mechanism. JWT technology is so popular and widely used that Google uses it to let you authenticate to its APIs. On the client side, you create the token (there are many libraries for this) using the secret token to sign it.

3. Claims are expected in which structural component of a JWT?

- Claims are expected in the payload of the JWT.

## Are JWTs Secure?

1. If I get a JWT and I can decode the payload, how can we call that secure?

- JWT doesn't concern itself with encryption. It cares about validation.

2. If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.

- JWS signature​​ The signature is used to verify that the sender of the JWT is who it says it is and to ensure that the message wasn't changed along the way.

3. Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.

- The concatenation of the 88-bit and 40-bit values makes a 128-bit key, which encrypts the message with it using AES in Counter 

## JWTs Explained

1. Why use JWT?

- JWTs are a good way of securely transmitting information between parties because they can be signed, which means you can be sure that the senders are who they say they are. Additionally, the structure of a JWT allows you to verify that the content hasn't been tampered with.


2. JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

- JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

3. What are the three components (the structure) of a JWT signature?


- They are lightweight and easy to use by client applications: for example, mobile applications.
They are self-contained, which means that the Liberty JVM server can consume the token directly and use a claim from the token as the identity for running the request.
They can be symmetrically signed by a shared secret by using the HMAC algorithm, or asymmetrically by using a private key.