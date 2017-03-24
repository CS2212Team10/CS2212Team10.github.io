# Stage 3 Features
## User Accounts

**Description:**  Users create a profile based on their name, email, and password, which then adds them to the default group. User accounts can be added and deleted. 

**Feasibility:** The feature facilitates the social media aspect of this application. Creating a profile identifies users.

**Dependency:** Failure to implement this feature will affect the team’s ability to implement other features, as this identifies who is commenting, rating and liking.

## Notes

**Description:**  Users can post notes to any circle or course that they are a part of. Posts can be added and deleted. 

**Feasibility:** This feature gives users the ability to post and share notes. It requires the creation of a profile, since the notes need to be identified by the users who create them.

**Dependency:** Failure to implement this feature will not affect the team’s ability to further implement other features but it will be a major hole in our project. 

## User Groups (Courses and Circles)

**Description:**  Users can create courses, which represent a course at Western, as well as circles which are aggregations of users who are all in a course. Users can also join courses and circles created by others. Circles are subgroups within courses which have the requirement that users be registered in the related course to join the circle. Users post notes to a course or circle. 

**Feasibility:** This feature is the defining aspect of the app, as it organizes the notes so users can find them and tailor their experience of the app. The only requirements of this feature are maintaining lists of users and posts, allowing users to join and drop courses/circles (adding/removing themselves from the lists), and adding/removing posts from a circle. It relies on users being implemented.

**Dependency:** The posting feature depends on courses being implemented, as users can only post to courses they have joined. The newsfeed depends on circles to be functional as well, as a user’s list of circles determines what shows up on their newsfeed.

## Stars

**Description:**  Stars can be added to and removed from posts (similar to “likes” on Facebook). Only one star can be added to a post per user. 

**Feasibility:** This feature is non-essential and just adds an extra element to the social aspect of the app.

**Dependency:** This feature depends on Users and Posts being implemented, but no current features depend on it. 

## Security

**Description:** Anyone can create an account, but they must be logged in to post, comment, star or view content in their groups. Users cannot contribute to or see content from groups they are not a part of, and they cannot delete content (stars, comments, posts, groups) that they did not create. 

**Feasibility:** This feature modifies how all other features are implemented (ie. how content is accessed and created/deleted). It will be implemented using Spring Security Service. 

**Dependency:** This feature is a modification of existing features in order to make them more secure. It requires Users to be implemented.

---

# Stage 2 Features
## User Accounts

**Description:**  Users create a profile based on their name, email, and password, which then adds them to the default group. User accounts can be added and deleted (but not yet modified). 

**Feasibility:** The feature gives purpose to the social media aspect of this application. Creating a profile gives identity to who posts and stars notes.

**Dependency:** Failure to implement this feature will affect the team’s ability to future implement other features, since this will show who is commenting, rating and liking.

## Notes

**Description:**  Users can post notes to the default circle. Posts can be added and deleted (but not yet modified). 

**Feasibility:** This feature gives users the ability to post and share notes. This feature requires the creation of a profile, since the notes need to be identified from who its coming from.

**Dependency:** Failure to implement this feature will not affect the team’s ability to further implement other features but it will be a major hole in our project. 

## Default Group

**Description:**  As a precursor to the circles and courses organization, we have a single group that all users are added to and to which notes can be posted.  

**Feasibility:** When completed with courses and circles, this feature will be the defining aspect of the app, as it organizes the notes so users can find them and tailor their experience of the app. The only requirements of this feature are maintaining lists of users and posts, allowing users to join and drop courses/circles (adding/removing themselves from the lists), and adding/removing posts from a circle. It relies on users being implemented.

**Dependency:** The posting feature depends on courses being implemented, as users can only post to courses they have joined. The newsfeed depends on circles to be functional as well, as a user’s list of circles determines what shows up on their newsfeed.

## Stars

**Description:**  Stars can be added to and removed from posts (similar to “likes” on Facebook). Only one star can be added to a post per user. Existing stars are displayed, although at present users cannot star posts through the UI.

**Feasibility:** This feature is non-essential and just adds an extra element to the social aspect of the app.

**Dependency:** This feature depends on Users and Posts being implemented, but no current features depend on it. 




---


# Essential Features

## Post Notes

**Description:**  Each user can post notes and comment, rate and like on other peoples’ notes within the circles they have added themselves to. Notes can be posted as pictures, pdfs, word documents etc

**Feasibility:** This feature serves purpose to the application since it gives the users the ability to post and share notes. This feature requires a creation of a profile, since the notes need to be identified from who its coming from.

**Dependency:** Failure to implement this feature will not affect the team’s ability to further implement other features but it will be a major hole in our project. This features gives purpose to our project.

## Creating a profile

**Description:** Each user will be asked to create a profile, in which will have information about them and the circles they are part of

**Feasibility:** The feature gives purpose to the social media aspect of this application. Creating a profile gives identity to who likes, rates, comments on the posted notes.

*Dependency:** Failure to implement this feature will affect the team’s ability to future implement other features, since this will show who is commenting, rating and liking.

## Courses and Circles

**Description:** Courses are aggregations of users and are the app’s representation of a class at Western. Circles are subgroups within courses which have the requirement that users be registered in the course to join the circle. Users post notes to a course or circle.

**Feasibility:** This feature is the defining aspect of the app, as it organizes the notes so users can find them and tailor their experience of the app. The only requirements of this feature are maintaining lists of users and posts, allowing users to join and drop courses/circles (adding/removing themselves from the lists), and adding/removing posts from a circle. It relies on users being implemented.

**Dependency:** The posting feature depends on courses being implemented, as users can only post to courses they have joined. The newsfeed depends on circles to be functional as well, as a user’s list of circles determines what shows up on their newsfeed.

## Newsfeed

**Description:** A user’s newsfeed displays clickable icons linking to the most recent 20 posts made to any circle they have joined, in chronological order. It is similar to a Facebook timeline in that the most recent comments on a post are displayed beneath it, as well as its rating. The newsfeed is the home page when a user logs in.

**Feasibility:** This feature only requires that courses are implemented, so that a user’s courses can determine their newsfeed content. When a user logs in, their newsfeed is produced by checking each of their courses for the 20 most recent posts, which should be fairly simple to implement.

**Dependency:** Nothing builds on this feature or depends on it.

# Extended Features

## Professor Ratings

**Description:** This extended feature build on user ratings by separating user and professor rating sections. A course has a single verified professor account attached to it which can rate notes or flag them to be removed.

**Feasibility:** This feature requires that the user ratings and professor accounts features be working and then they will be simple to set up. The professors being verified can occur outside the app in the prototype (with administrators giving them permission to create professor accounts). The flag option will automatically notify administrators of problematic posts.

**Dependency:** Nothing builds on this feature or depends on it.

## Authenticating user email

**Description:** The email will be authenticated to check if it is a valid uwo email. This will help reduce plagiarism since it exposes one’s student identity

**Feasibility:** This feature is an extended feature that reduce plagiarism, since the users’ identities are linked with their university emails.

**Dependency:** This is an extended feature, so poor/no implementation of this feature will not cause the project to fail

# Optional Features

## Text to Speech

**Description:** It is a helpful study tool where a PDF/word document uploaded will be read out loud by an automated voice This can help to study through verbally reading notes, textbooks etc.

**Feasibility:** This feature is an optional feature that is a study tool. Notes uploaded as PDFs can be read out loud. APIs are available that can be used to make this feature functional.

**Dependency:** This is an additional feature; the project will not be affected if this feature is not implemented

## Search Engine

**Description:** This is a feature to allow users to search for keywords in all of the notes in a circle.

**Feasibility:** Notes can only be posted as pdfs, so we will need to be able to search a collection of pdfs for keywords. There are some APIs we can use to do this, including PDFBox and Lucene.

**Dependency:** Nothing builds on this feature or depends on it.
