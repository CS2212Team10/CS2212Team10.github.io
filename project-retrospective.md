# Project Retrospective
[![Demo Video on YouTube](http://i.imgur.com/jwGjIur.png)](https://www.youtube.com/watch?v=PebcfiGmSSc "Demo Video on YouTube")
## Workflow
Branching Model and Process

* Each member in the group has his or her own dev branch that can be pushed and pulled anytime. 
* Any pull to the dev branch should be reviewed and approved by a peer member. 
* Any approved changes would be saved temporarily in the dev branch, and
* Master branch only contains code that are error-free and ready to be reviewed. 

Development tool: IntelliJ IDEA Ultimate

Framework: Grails, AngularJS, Spring Security and Spring Security REST API

Task Distribution Management
* Members were divided evenly between frontend and backend
* Basic tasks were distributed to reduce redundant code
* As build complexity increased, distribution of tasks was dependent on member’s coding capabilities.

## MVC Design Patterns

The user interface (ie. the web application) is connected to the logic through a rest API. The logic (ie. the controllers) requests data from the model.
* The M in MVC is represented by the domain classes.
* The C in MVC is represented by the controller classes.
* The V in MVC is represented by the Web application.

For example when a the user creates a new account the Web application sends a HTTP request that includes the all relevant data to create a user, to the backend. Then the user controller creates a new instance of a user in the domain classes.

We could have improved are the section of the web app that retrieves and displays the circles and controllers to decrease code reuse. Integrating security earlier in the development process would have made a lot of the headaches surrounding security disappear.

## Refactor Retrospective

## Project Retrospective
