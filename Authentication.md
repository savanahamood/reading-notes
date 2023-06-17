# Securing Passwords

1. Explain to a non-technical friend how you would safely hash and store a password.
hashing and storing passwords involves using a one-way function to transform the password into a unique hash. By storing only the hashes and adding additional security measures like salting and using strong hashing algorithms, we can ensure that passwords remain securely stored, protecting user accounts from unauthorized access.

2. What is Bcrypt?
Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor, which allows you to determine how expensive the hash function will be.

3. Why might you use something like Bcrypt?
using Bcrypt helps protect user passwords and reinforces the security of your application or system. It reduces the likelihood of successful password attacks, provides compliance with security standards, and gives users confidence that their passwords are stored securely.

# Basic Auth

1. What is Basic Authentication?
Basic Authentication is a simple authentication scheme used in web applications and APIs to authenticate and authorize users. It is an HTTP-based authentication protocol that requires the user to provide their credentials, typically a username and password, for authentication purposes.

2. What properties are necessary in the header of a Basic Auth request?
Authorization and Content-Type

3. How are username:password in Basic Auth encoded?
by Base64 Encoding: Convert the concatenated string into Base64 encoding. Base64 encoding converts binary or text data into ASCII characters. The resulting encoded string represents the username and password in a format that can be transmitted as part of the HTTP header.


# OWASP auth cheatsheet

1. Define the authentication process to a non-technical recruiter.
Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

2. How should your error messaging respond (both HTTP and HTML)? Why?
The reason for considering both HTTP-level responses and HTML error pages is to provide a comprehensive approach to error handling. HTTP-level responses are essential for communication between servers and clients, allowing for standardized error codes and additional information. On the other hand, user-facing HTML error pages focus on presenting errors in a user-friendly manner and guiding users through the problem resolution process. Together, they help ensure that users receive meaningful feedback and can take appropriate actions when encountering errors while using web applications.

3. Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.
https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html