# A Very Simple Software Requirements Specification

### 1. Introduction
##### 1.1 Purpose
This file outlines the plan for version 1 (MVP) of `gumshoe`. `gumshoe` will be a full-stack application for creating and managing tickets (similar to Jira, Asana, etc. but on a much smaller scale).

`gumshoe` is meant to be a fun side-project for gaining experiencing in building such a project. It isn't meant to be used as a serious replacement for other issue tracking options out there.

Development on `gumshoe` may continue on past version 1, but at that point this SRS will not longer be applicable.
##### 1.2 Intended Audience
John will be the primary user for this application, and of course anyone else that happens to be interested.
##### 1.3 Intended Use
`gumshoe` will be added to John's portfolio, and will also be used to track the development progress of `gumshoe` itself, once it reaches such level of usability prior to the release of version 1.
##### 1.4 Scope
This will be a deployed application that can be used by anyone anywhere. Users will be able to create accounts and sign in, and there will be different user roles available such as admin, standard, and guest (least privileged).

Users will be able to create and manage tickets (managing involves viewing, modifying, and deleting tickets at a minimum). Tickets will have various data such as title and description.

The data of tickets and users should be kept in persistent storage.

The website should be mobile friendly, and effort will be made to make the app's UI look nice, but of course it won't be done by a UI/UX professional.
##### 1.5 Definitions and Acronyms
- gumshoe - A detective! See the [dictionary.com definition](https://www.dictionary.com/browse/gumshoe)
- ticket - A task to be done, which is shown in the form of a title, description, who the task is assigned to, and more.
- admin - The role with the highest privileges
- standard - The default role when creating an account
- guest - The role with least privileges
### 2. Overall Description
##### 2.1 User Needs
Users need a way to access `gumshoe` from any device and anywhere in the world.

Users need to have a way to create an account, log in, or demo the app without creating an account or logging in.

Users need to create tickets, as well as modify existing tickets and delete them if necessary.

Users need a page to view all tickets assigned to them.

User progress and data should be persisted, such that ticket information should be saved and viewable no matter where they are or what device they are using.

A dashboard would be a nice-to-have.
##### 2.2 Assumptions and Dependencies
Usage of `gumshoe` is dependent on internet access and a modern web browser.
### 3. Requirements
##### 3.1 Functional Requirements
Tickets
- Attributes (possibilities): title, description (rich text), size (L, M, S, etc.), type (Bug, Research, Feature New, Feature Modify, etc.), status (not started, doing, complete, etc.), due date, assignee, comments, comment history, activity history

Users

User Interface

Accessibility
##### 3.3 Nonfunctional Requirements
- A Node server will be hosted on Firebase and will use GraphQL for the api.
- The batabase will be a document database and will be hosted on Firestore.
- The frontend will be hosted on Netlify or Digital Ocean.
- The frontend will be built with React.
- All code will be written in Typescript (as opposed to Javascript) when possible

\
\
*This SRS outline is partially based on [this article](https://www.perforce.com/blog/alm/how-write-software-requirements-specification-srs-document)*
