## Week Three - Module 4 Recap

1. At a high level, what is Node?

It's a server side runtime environment for javascript. 

2. What is Express? What is Express similar to in the Ruby world?

Express is a node web app framework; Express is to JS as Sinatra is to Ruby in terms of provided functionality. 

3. How do we setup a route when creating an API with Node and Express? Please provide a code snippet.
// HTTP verb + URL + controller + action
app.get('/api/v1/foods', FoodsController.indexFood)
app.post('/api/v1/foods', FoodsController.createFood)
app.put('/api/v1/foods/:id', FoodsController.editFood)
app.delete('/api/v1/foods/:id', FoodsController.deleteFood)

*if a controller and model objects not created yet, the second argument would be a function(request, response){} to handle the request and response data

4. What do we use Knex for?

It is the ORM for node/js. It allows us to connect to and communicate with a databbase by making queries. 

5. How could you organize your code to follow the MVC design pattern in your Quantified Self project?

By abstracting the code for setting up an API endpoint into separate files with separate responsibilities: 

A: model level functions for SQL queries; layer between JS server and datababse server

B: controller layer: layer between model objects and router; responsible to perform different actions on POJOs by handling the 
request and response data

C: routes: specify HTTP verb and pass URL and controller object function as arguments

Example: app.get('/api/v1/foods', FoodsController.indexFood) demosntrates Rails like routing pattern where a verb and URL are routed to a controller and a specific action within that controller

6. How do you execute raw SQL in node?

A: capture database variable with knex and current dev env, B: call .raw() method, and C: pass it raw sequal query 
(database.raw("SELECT * FROM foods") => returns a promise which should be handled with .then .catch chain)

7. What are some advantages to having your front end and back end code live in separate applications? What are some disadvantages?

Advantage: different languages can be used and connected via API endpoints and they can run independent of each other; 
Disadvantage: need to setup and host separate apps on separate servers and to maintain two code bases;

#### Review  

8. Describe DNS.

Domain Name Servers: keep a domain name directory and translate URLs into their respective Internet Protocol(IP) address numeric value. 

9. What does writing clean code mean to you?

A: avoid repetition
B: abstract code into reusible methods
C: code is easy to read and to modify

10. If you were building an application that models hotels, what classes would you need? What classes would be responsible for what functionality?

class Building wraps most other classes; responsible for security and access from other applications/hotels
class Floor responsible for separating relevant operations in the running of the hotel
class Room responsible for storing furtinute and guests
class Personnel responsible for the handling of hotel operations
class Guest responsible for triggering hotel events

