## Week Two - Module 4 Recap

1. What's one difference between ES5 and ES6?

Syntax: A. Arrow functions in ES 6 versus (arguments) => {expressions}; unlike anonymous callback functions in ES 5, these do not define the context for this which can lend itself to OOP

Objects: ES 6 introduces the use of class Name { constructor() } to more closely emulate other OOP structure of code

String interpolation: `via ${backticks}` 
 
2. What's the difference between asynchronous and synchronous JavaScript? 

Synchronous JS runs code line-by-line and function-by-function -- JS is a single thread language just like Ruby. 

Asynchronous JS takes advantage of browser webAPIs to allow for multiple functions to run simultaneously; this process utilizes the stack (list of commands to be run), browser APIs, callback queue, and loop.  

3. What are the four pillars of Object Oriented programming?

A. Abstraction: what's being shown -- making code as readable and independent as possible
B. Encapsulation: how it works -- grouping and linking relevent funtionality together
C: Polymorphism: same function can have different behavior across different contexts (def walk in the context of class Human versus def walk in the context of class Dog)
D: Inheritance: the ability to inherit features and behaviour from predefined objects

4. What are some tools available in JavaScript to help you write object oriented code?
class object declarations,  JS {} objects, assert testing

5. What are some key concepts to be aware of when refactoring your JavaScript?

handling different objects with the appropriate available methods (e.g. handle a returned Promise object from an AJAX call function with a .then & || .catch method chain instead of callback/nested callback functions) 

6. What's a callback function and what are some reasons when we use/need callback functions?

Callback functions are passed as arguments and depend on another function to be involked. 

7. What's the scope of variables in Javascript?

Global variables are declared outside of and available within functions, but variables decralred inside of a function are local limited to the scope within that function. 

8. What's the difference between `==` and `===` in JavaScript?
'==' checks if objects are of the same class; '===' checks if objects evaluate to the same value

9. Why do front end frameworks exist?
As guidelines to building working features/applications that can successfully work in the browser. 

#### Review  

10. Why do people say "HTTP is stateless"?
Because it doesn't store the state of the resources being found in the server database and represented in the browser. 

11. Describe a RESTful API.
A restful APi follows conventions to make itself easily accessible, readable, and predictible to use; It consists of an HTTP request and a delete, post, edit, or create action; It is. cacheable because GET requests are idempotent; The client is not required to know anything about the server API -- this is why non-restful architecture is more appropriate for certain client needs, such as streaming. 

12. What are some main characteristics of a team following an agile workflow?

A: Iterative process that prioritizes small pieaces of working code to demo over large features
B: Constant client feedback
C: Frequent change implementation


13. What are some advantages **and** disadvantages to using OAuth to authenticate a user?

advantages: established secure protocols for user account verification exist; removes the need to create and remember multiple logins; removes the need to share and transmit sensitive account info; 

dissadvatage: limits the user by technology -- unless suing some other platform, a user may not be able to utilize an app that relies only on o.auth for account creation; less autonomy -- if external app/api is changed wihtout notice, not maintained or becomes unavailable, our apps would run into having to cope with that change. 
