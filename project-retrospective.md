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


#####BACKEND STRENGTHS:

The authorization was checked for every level of code: post, star, user, course, and circle. We had a successful attempt at cascading security.
We had a “textbook” implementation of the REST API, which makes it easier to rewrite the code in any language and can be paired with any client-side.
The backend team also increased code reuse by extending the UserGroup domain in both the domains: Course and Circle. 


#####BACKEND WEAKNESSES:
It would have been nice if we had separated circle and course in the User. Currently, users have a UserGroup attribute where either circles or courses can be stored as ‘UserGroup’. It would’ve been nice to have them separate.

#####FRONTEND STRENGTHS:
The main strength of our front end code from an object-oriented perspective was its modularity of code that we were able to re-use across pages. Specifically, we used main.gsp and mainplain.gsp as the basic layouts of our pages. Main.gsp was used for pages that contained a navigation bar at the top and a footer at the bottom. This layout was used for all pages seen when the user is signed in, ie. main, class, document view, etc. Mainplain.gsp is identical to main.gsp except that it does not include the navigation bar or footer. This layout is used for all pages seen when no user has signed in yet, ie. home, sign in, and sign up. The navigation bar and footer are, in turn, encoded separately for reusability. Many of the effects triggered when the user moves the cursor over elements of the page are encoded separately in hover.css and hover-min.css, such that we did not need to re-implement functionality such as an element’s lighting up when the cursor is over it, in every page. A number of other types of commonly-used elements such as input boxes and title headers were encoded in a similar way and re-used over many pages.

#####FRONTEND WEAKNESSES:

Although we implemented extensive modularity and code-reusability, there were several features that we initially intended to implement on only one page, but ended up using on several or all, that we did not modularize to the extent that we could have. For example, the contents of each page are set with a blue box in the background that serves as a stylistic template for all of our pages. We did not modularize this blue box, and our code would have been simpler, cleaner, and perhaps enhanced the app’s performance if we were to have encoded this feature separately the way we did for the main page layouts and the hover effects, in particular because this box includes a number of CSS features such as shadows and hover effects. For ease of coding, if we were to have modularized this box to scale to fit whatever contents we inserted into it, we could have avoided having to manually adjust the dimensions of the box for each page.

## Project Retrospective

In this section, you will answer questions about the overall project, rather than the code design. Answers can include details about interpersonal communication, task and deadline management, UI design, frameworks/technologies, meeting management, etc. Be honest and professional in your answers.
#####What did your group do well?
The group worked very well together, with consistent communication, organization, and division of labour allowing for effective and efficient teamwork. The group was divided into frontend and backend teams, but occasionally worked all together to keep everyone up to date on what others were doing. We also produced API documentation to make communicating with the server through REST as straightforward as possible (for the frontend, as well as for backend testing). We had very thorough testing, especially of the backend of the project. The clear division of responsibilities made it so that all members understood what they needed to do and know (and what they didn’t need to bother researching), which made the work very efficient. 
#####What could your group have done better?
The timing of the project could have been improved, as much of the frontend development depended on the completion of the backend. We tried to combat this by setting earlier deadlines for the backend, but in Stage 2 and 3 the timelines didn’t give the frontend an ideal amount of time to complete their portions. This also meant the front end had less time to test all their features. We also could have communicated better between the frontend and backend earlier on, so that the frontend was fully aware of all of the features of the backend. The team also had some difficulty with planning meeting times due to conflicting schedules, however we combatted this issue by having more frequent meetings with fewer members in more specialized teams.
#####What did you like about the tools and frameworks you used?
IntelliJ was an effective tool, as it allowed us to work directly with GitHub and manage merge conflicts. The built in database included in Grails made it easy to work with data, which we could see from the DB console, and was useful because it has built in functions like cascading deletes. Creating, assigning, and tracking issues through GitHub was helpful in managing responsibilities.
#####What didn’t you like about the tools and frameworks you used?
The biggest issue was that the team struggled to find effective documentation of Grails. It was also difficult to manually produce API documentation, which in the future could be done better using the framework Swagger. The front end struggled with how Grails compiles CSS files, as styles were being overwritten. 