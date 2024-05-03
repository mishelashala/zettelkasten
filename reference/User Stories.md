## What user stories represent

"Rache Davies has said that cards 'represent customer requirements rather than document them'."

Mike Cohn, User Stories Applied, p4

### Alternate Definition

"Each user story represents a discrete piece of functionality; that is, something a user would be likely to do in a single setting."

Mike Cohn, User Stories Applied, p14

## What user stories aren't

"[...] stories are descriptions of user -or customer- valued functionality; they are not to-do lists for developers."

Mike Cohn, User Stories Applied, p111

## User stories are better than documentation

"Because user stories shift emphasis toward talking and away from writing, important decisions are not captured in documents that are unlikely to be read."

Mike Cohn, User Stories Applied, p14

## User Story Composition

"User stories are composed of three aspects:
- a written description of the story used for planning and as a reminder
- conversations about the story that serve to flesh out the details of the story
- tests that convey and document details and that can be used to determine when a story is complete"

Mike Cohn, User Stories Applied, p4

### User Story Template Format

"I as a (role) want (function) so that (business value)"

Mike Cohn, User Stories Applied, p81

### 3Cs model

"Ron Jeffries has named these three aspects with the wonderful alliteration of Card, Conversation, and Confirmation."

Mike Cohn, User Stories Applied, p4

## User Story content

"[...] it is useful to think of the story card as containing:
- a phrase or two that act as reminders to hold the conversation
- notes about issues to be resolved during the conversation"

Mike Cohn, User Stories Applied, p18

##  User stories should not include technical details

"[...] the users of this system do not care about the technical details of how the application connects to the database."

Mike Cohn, User Stories Applied, p4

### User stories should be tech agnostic

"In exactly the same way it is worth attempting to keep user interfaces assumptions out of stories, it also worth keeping technology assumptions out of stories."

Mike Cohn, User Stories Applied, p22

## Elements of a good user story: Invest Acronym

"A good story is:
- Independent
- Negotiable
- Valuable to users or costumers
- Estimable
- Small
- Testable"

Mike Cohn, User Stories Applied, p17

### Independent

"Dependencies between stories to prioritization and planning problems."

Mike Cohn, User Stories Applied, p17

### Negotiable

"They are not written contracts or requirements that the software must implement. Story cards are short descriptions of functionality, the details of which are to be negotiated in a conversation between the customer and the development team."

Mike Cohn, User Stories Applied, p18

### Valuable

"What you want to avoid are stories that are only valued by developers."

Mike Cohn, User Stories Applied, p21

#### How to ensure stories are valuable

"The best way to ensure that each story is valuable to the customer or users is to have the customer write the stories."

Mike Cohn, User Stories Applied, p22

### Estimable

"It is important for developers to be able to estimate (or at least take a guess at) the size of a story or the amount of time it will take to turn a story into working code."

Mike Cohn, User Stories Applied, p22

### Small

"Story size does matter because if stories are too large or too small you cannot use them in planning."

Mike Cohn, User Stories Applied, p23

#### Too small

"A story that is too small is typically one that the developer syas she doesn't want to write down or estimate because doing that may take longer than making the change."

Mike Cohn, User Stories Applied, p26

#### Dealing with tiny stories

"A good approach for tiny stories, common among [[Extreme Programming]] teams, is to combine them into larger stories that represent from about a half-day to several days of work."

Mike Cohn, User Stories Applied, p26

### Testable

"If the story cannot be tested, how can the developers know when they have finished coding?"

Mike Cohn, User Stories Applied, p27

#### Untestable User Stories

"Untestable stories commonly show up for nonfunctional requirements, which are requirements about the software but not directly about its functionality."

Mike Cohn, User Stories Applied, p27

## Closed Stories

"A closed story is one that finishes with the achievement of a meaningful goal and that allows the user to feel she has accomplished something."

Mike Cohn, User Stories Applied, p76

## User Stories should be like slices of a cake

"A far better approach is to write the replacement stories such that each provides some level of end-to-end functionality. Bill Wake [...] refers to this as 'slicing the cake.' Each story must have a little from each layer."

Mike Cohn, User Stories Applied, p76

### Why slices

"[...] an application could conceivably be released for use with only partial functionality as long as the functionality that is included in the release slices all the way through the system."

Mike Cohn, User Stories Applied, p76

## Grouping Users in Roles

"While each user comes to your software with a different background and with different goals, it is still possible to aggregate individual users and think of them in terms of user roles."

Mike Cohn, User Stories Applied, p32

## User Roles

"When we talk about user stories, who is the user we're talking about?"

Mike Cohn, User Stories Applied, p31

### What is an user role

"A user role is a collection of defining attributes that characterize a population of users and their intended interactions with the system."

Mike Cohn, User Stories Applied, p32

### Identifying user roles

"We will use the following steps to identify and select a useful set of user roles:
- brainstorm an initial set of user roles
- organize the initial set
- consolidate roles
- refine the roles"

Mike Cohn, User Stories Applied, p33

### Why Include User Roles in the stories

"Instead of thinking of bland, faceless, interchangeable users, the developer will begin thinking of real, tangible users whom she needs to satisfy with the software."

Mike Cohn, User Stories Applied, p80

## Personas

"A persona is an imaginary representation of a user role."

Mike Cohn, User Stories Applied, p38

## User Proxies

"When we cannot get as many users as we want to represent different perspectives of the product, we need to resort to user proxies, who may not be users themselves but are on a project to help represent users."

Mike Cohn, User Stories Applied, p55

## Epics

"When a story is too large it is sometimes referred to as an epic. Epics can be split into two or more stories of smaller size."

Mike Cohn, User Stories Applied, p6

### You don't need all the details all at once

"For a feature that you want eventually but that isn't important right now, you can first write a large story (an epic)."

Mike Cohn, User Stories Applied, p14

#### Extra detail does not equals extra precision

"Most readers of this type of story will mistakenly associate the extra detail with extra precision."

Mike Cohn, User Stories Applied, p18

#### Stories encourage deferring details

"It is this ability to iterate over a story set that allows stories to encourage the deferring of detail."

Mike Cohn, User Stories Applied, p14

#### Too much detail discourages discussion

"This can lead to the mistaken belief that the story cards reflect all the details and that there's no further need to discuss the story with the customer."

Mike Cohn, User Stories Applied, p20

#### Why Deferring is important

"Deferring detail is important because it allows us to not spend time thinking about a new feature until we are positive the feature is needed."

Mike Cohn, User Stories Applied, p14

### Epic categories

"Epics typically fall into one of two categories:
- The compound story
- The complex story"

Mike Cohn, User Stories Applied, p24

#### Compound story

"A compound story is an epic that comprises multiple shorter stories."

Mike Cohn, User Stories Applied, p24

#### Complex Story

"[...] the complex story is a user story that is inherently large and cannot easily be disaggregated into a set of constituent stories."

Mike Cohn, User Stories Applied, p25

##### Developers don't understand the story

"If the developers do not understand a story as it is written, they should discuss it with the customer who wrote the story."

Mike Cohn, User Stories Applied, p22

##### How to tackle complex stories

"If a story is complex because of uncertainty associated with it, you may want to split the story into two stories: one investigative and one developing the new feature."

Mike Cohn, User Stories Applied, p25

###### Spike

"The solution in this case is to send one or more developers on what Extreme Programming calls a spike, which is a brief experiment to learn about an area of the application."

Mike Cohn, User Stories Applied, p22

## Trawling

"Trawling for requirements leads to the mental image that requirements are captured in a fishing net being pulled behind a boat."

Mike Cohn, User Stories Applied, p43

### Analogy from fishing

"A first pass can be made over the requirements pon with a large mesh net to get all the big ones. You can get a feel for the needed software from the big requirements and then make a subsequent pass with a smaller mesh net and get the medium-sized requirements, still leaving the small ones for later. This metaphor works wether we think of size as business value, essentialness to the software, and so on."

Mike Cohn, User Stories Applied, p43

### Requirements grow and die

"[...] trawling for requirements expresses the idea that requirements, like fish, mature and possibly die."

Mike Cohn, User Stories Applied, p43

## Gathering requirements

### Finding requirements requires skill

"A skilled requirements trawler will know where to look for requirements, while the unskilled trawler will waste time with inefficient techniques or in the wrong locations."

Mike Cohn, User Stories Applied, p44

### Valuable Techniques

"Some of the most valuable techniques for creating a set of stories are:
- User interviews
- Questionnaires
- Observation
- Story-Writing workshops"

Mike Cohn, User Stories Applied, p45

### Domain experts are critical for gathering requirements

"Domain experts, sometimes called subject matter experts, are critical resources because of how well they understand the domain the software will be targeted at."

Mike Cohn, User Stories Applied, p58

## User Story Acceptance Testing

"Acceptance testing is the process of verifying that stories were developed such that each works exactly the way the customer team expected it to work."

Mike Cohn, User Stories Applied, p12

### Customers Specify The Acceptance Tests

"Because the software is being written to fulfill a vision held by the customer, the acceptance tests need to be specified by the customer."

Mike Cohn, User Stories Applied, p69