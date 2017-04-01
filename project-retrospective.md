# Project Retrospective

## Workflow

## MVC Design Patterns

The user interface (ie. the web application) is connected to the logic through a rest API. The logic (ie. the controllers) requests data from the model.
* The M in MVC is represented by the domain classes.
* The C in MVC is represented by the controller classes.
* The V in MVC is represented by the Web application.

For example when a the user creates a new account the Web application sends a HTTP request that includes the all relevant data to create a user, to the backend. Then the user controller creates a new instance of a user in the domain classes.

We could have improved are the section of the web app that retrieves and displays the circles and controllers to decrease code reuse. Integrating security earlier in the development process would have made a lot of the headaches surrounding security disappear.

## Refactor Retrospective

## Project Retrospective
