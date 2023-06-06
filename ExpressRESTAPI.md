# Express REST API
## Readings
### Review: ES6 Classes

1.Classes are a template for creating objects.

2.Can a class declaration be hoisted?
class declarations are not hoisted you need to declare a class before you can use it in your code

3.How would you describe a constructor and contextual “this” to a non-technical friend?
we will suppose that we will using a class called "Person" that represents individuals the class has properties like "name" and "gender" to store the person's name and gender, and a method called "introduce" to introduce themselves When we use the constructor to create a person object, we pass in arguments for the name and gender, like "Savana" and "female" The constructor then assigns those values to the respective properties of the person object using "this.name = name" and "this.gender = gender".


### Using Express Routing

1.Within Express, what does routing refer to?
refers to how an application’s endpoints (URIs) respond to client requests.

2.What is the difference between a route path and a route method?
A route method is derived from one of the HTTP methods, and is attached to an instance of the express class, Express supports methods that correspond to all HTTP request methods: get, post, and so on but Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.

3.When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?
You can use this mechanism to impose pre-conditions on a route, then pass control to subsequent routes if there’s no reason to proceed with the current route. and what must you do if next has been passed to your middleware as a parameter? you must ensure next() is called appropriately to pass control to the next middleware function or route handler


### Express Routing

1.What is an Express Router?
It is a mini express application without all the bells and whistles of an express application, just the routing stuff. it's a framework that allows you to create modular and reusable sets of routes for handling HTTP requests

2.By what mean do we initialize express.Router() in an express server?
to create modular and reusable sets of routes within your Express server

3.What do we use route middleware for?
Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we’d like to do before we actually spit out information to our user.

