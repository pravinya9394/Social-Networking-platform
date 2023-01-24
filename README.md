# Social-networking-platform
Goal:
A social networking platform for users to discover events and connect with people who share similar interests

Overview:

Define a list of interests and events by direct DB write [MUST]

A user can add interests to his profile [MUST]

A user can see a list of events happening in the city for the added interests [MUST]

A user can see events listed from Eventbrite public API [MUST]

A user can see a list of events they have registered for [MUST]

A user can register for the event [GOOD]

A user can see other participants of an event [MUST]

A user can add other participants as their friends [GOOD]

A user can explore activities of friends [EXTRA MILE]

Non-Functional requirements

Logging

Unit tests

UI Interfaces:

Home: List of events - Filters (City)

On click of an event: Event page

Register for the event - Send an email - GOOD

Event Brite plugin to display public events

Profile: Add interests 

Explore: User with same interests ka list

	On click of user in interest list, show all interests of the user


----------------------------------------------------------------------------------------------------------------------------------




Appendix

Coverage:


Day 1

HLD + few APIs working

Day 2

30% UI and all working APIs

Day 3

Final integration + Demo



APIs:

Add user ( Post)

POST /api/user

Add interest to an existing user. (Put)

PUT /api/user/:id/interest

Get user by user id and display user information. (Get)

Get interests of a particular user. (Get)

Remove the interest of the user. (Put)

Get events happening for a particular interest. (Get)

Add events for a particular interest. (Post)

Delete a user ( Delete)

Schema:

User


Variable Name

Data Type

Constraints

UserId

Long

PK

FirstName

String



LastName

String



Email

String

Unique



Interest


Variable Name

Data Type

Constraints

InterestId

Long

PK

InterestName

String

Unique



User-Interest


Variable Name

Data Type

Constraints

UserId

Long

FK (User), PK

InterestId

Long

FK (Interest), PK



Event

Event Details

Event Registration

Event City-Pincode Mapping



