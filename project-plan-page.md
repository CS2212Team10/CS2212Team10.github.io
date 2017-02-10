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









