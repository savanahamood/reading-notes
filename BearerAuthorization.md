# Bearer Authorization

### Intro to JWT
1. What is a JSON Web Token (JWT)?
JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. 

2. When should we use JSON Web Tokens?
* Authorization
* Information Exchange

3. Claims are expected in which structural component of a JWT?
JSON Web Tokens consist of three parts separated by dots (.), which are:
* Header
* Payload
* Signature
Therefore, a JWT typically looks like
xxxxx.yyyyy.zzzzz



### Are JWTs Secure?
1. If I get a JWT and I can decode the payload, how can we call that secure?
the security of JWTs lies in the token's integrity, authenticity, and the server's ability to verify the token's signature. While the payload can be decoded by anyone, the digital signature ensures that the token hasn't been tampered with, providing a level of security in the authentication and authorization process.

2. If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.
Both the sender and the receiver must have access to the same secret key. The sender uses the secret key to sign the token, and the receiver uses the same secret key to verify the signature. If the secret key used by the sender and receiver does not match, the signature verification will fail

3. Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.
sending concatenated content and a secret securely involves encrypting the information in a way that only the intended recipient can decrypt and understand. This ensures that the information remains confidential and protected from unauthorized access.




### JWTs Explained
1. Why use JWT?
JWTs provide a lightweight and flexible solution for authentication and authorization, offering simplicity, security, and compatibility across different platforms and technologies.

2. JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.
JWTs being compact and self-contained means that they are easy to transmit, efficient in terms of size, and contain all the necessary information for verification. This makes them a practical and convenient choice for secure communication and authentication in various applications and systems

3. What are the three components (the structure) of a JWT signature?
* Header
* Payload
* Secret Key