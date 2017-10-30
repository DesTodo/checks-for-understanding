## Week Four - Module 4 Recap

1. What's your favorite project management tool?

I like Waffle for its Git integration and its less busy compared to Pivotal Tracker, especially for individual or pair projects. I've recently been introduced to Jira, and would be interested in using it for its Git and CI integration.  

2. Why do we create staging environments?

To test how the software works with the code changes made but in an environment that is the same as the production environment instead of the local dev invironement/s. Ultimately, to prevent introducing bugs and breaking functionality upon deployment.

3. What are the characteristics of a good README (in your opinion)?

It should describe the project and its purpose. It should include instructions for set up and dependencies. Also potentially instructions for how to contribute in the project and pictures/snippets for ease of use. 

4. What's one main improvement you're going to make to your code regarding accessibility issues?

Practice use of appropriate HTML elements
Make forms accessible by including descriptive tags
Minimize changing fonts and beware of distracting color themes
Learn to use ARIA roles and alerts for dynamically updated content

5. What are some basic security concerns to be aware of when building applications?

In Rails, use has_secure_password method with password_digest attribute to authenticate user login against bcrypt password 
Don't share sensitive information on GitHub (production keys and authentication tokens)
Don't pass information from URL params and forms into query without sanitizing || AR ORM layer is safe against SQL injection
Make methods private whenever possible to expose only necessary app functionality

6. Why is continuous integration helpful/important?

CI is an automated tool to help in tracking how changes to the code base may introduce bugs and in doing so, to reduce potential debugging time for code built on top of code that wasn't working as anticipated. Like staging, it tests the code in production ENV. CI can't work without thorough unit and integration testing.

7. What are some continuous integration tools?

Travis, Jenkins, GitLab, Bamboo CI

#### Review  

8. What are some characteristics of "good" git workflow?

agree on gitflow with team
checkout and appropriately designate branches for each feature
commit often with informative messages
tag team members, request reviews and review code in PR before merging

9. What are the four fundamental concepts of object oriented programming?

Abstraction: follow single responsibility principles to write code that is easy to read, maintain, reuse, and change
Encapsulation: group abstracted functions which work together to solve a problem programatically 
Polymorphism: understand and account for how functionality may change across different objects and datatypes
Inheritance: implement how objects can inherit behavior from superclasses and abstract constants into modules

10. What's a module in Ruby and what's the difference between a class and a module?

Modules can be implemented to abstract constants and generic behavior that can be shared between classes; the functions/behavior in modules are inherited by objects in a class via namespacing or as mixins. Modules do not have instances and therefore cannot preserve state. Classes can be instantiated and can store state; they can inherit behaviour and be inherited by other classes. 
