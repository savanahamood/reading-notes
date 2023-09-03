# API Integration
### Review API Server Build
**1.Explain the different between a query string parameter and a path parameter.**

* Query String Parameter: A query string parameter is used to send additional data to a web server by appending it to the end of a URL. It typically consists of a key-value pair separated by an equal sign (key=value) and is preceded by a question mark (?) in the URL. Query string parameters are often used for filtering or sorting data.

* Path Parameter: A path parameter is a part of the URL path itself and is used to identify a specific resource or endpoint. Path parameters are typically enclosed in curly braces ({}) within the URL path and can hold values that are essential to the resource being accessed. They are used to route requests to the correct endpoint.

**2.What would our API URL with a path id parameter be given the following information:**
* Domain: http://our-site.com
* v3
* model name: stuff
* id: things

The API URL with a path id parameter would look like this: http://our-site.com/v3/stuff/things


**3.We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.**
An “interface” in the context of a dynamic API refers to a set of rules and functions that allow different software applications to communicate and interact with each other. It’s like a bridge that enables one program to understand and work with another program’s data and functionality, even if they were created by different developers.

Imagine you have a universal remote control that can be used to operate various electronic devices like TVs, DVD players, and stereo systems. This remote control has buttons and functions that are designed to work with different devices, making it easy for you to control them all using a single remote. In a similar way, an API interface provides a standardized way for different software programs to communicate and share information, making it possible for them to work together seamlessly.

### Review Auth Server Build

**1.Describe how you would use middleware to implement basic and bearer auth.**
* Basic Authentication: Middleware can be used to implement Basic Authentication by intercepting incoming requests to a server. It checks if the request includes a username and password, typically sent as a Base64-encoded string in the request headers. If the credentials are valid, the request is allowed to proceed; otherwise, access is denied.

* Bearer Authentication: Middleware for Bearer Authentication checks for a token (usually a JSON Web Token or JWT) in the request headers. If a valid token is present, the request is authorized; otherwise, access is denied.


**2.Describe the handshake necessary to implement OAuth.**
OAuth involves a handshake process between three parties: the user, the client application, and the OAuth server (usually maintained by a third-party service). Here’s a simplified overview of the process:

The user initiates the process by logging into a client application.
The client application requests authorization from the user to access specific resources on their behalf.
The client application sends this authorization request to the OAuth server.
If the user grants authorization, the OAuth server provides the client application with an access token.
The client application can then use the access token to access the user’s protected resources on the server.

**3.Describe how Role Based Access Control works to a non-technical friend.**
RBAC is like a bouncer at a club. It checks your badge (role) and only lets you into the areas you're allowed in. It helps keep data and systems safe by managing who can do what.

### Resources:
 [Review API Server Build](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/api-server/)

[Review Auth Server Build](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/auth-server/)


