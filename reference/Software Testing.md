## What tests should focus on

"Tests should concentrate on the incoming or outgoing messages that cross an object's boundaries."

Sandi Metz, Practical Object-Oriented Design, p197

## What to do when we catch a bug

"For each production bug, we should ask the question, 'Why didn't our tests catch this bug?', document the answer, and then add a test that covers it."

Tom Hombergs, Get Your Hands Dirty on Clean 
Architecture, p82

## Automated Testing

### Benefits of automated tests

"Automation is essential to keeping the cost of regression test execution manageable over time."

Chris Sterling, Managing Software Debt, p11

## Functional tests

"[...] ensures that the application functions as expected."

Mike Cohn, User Stories Applied, p72

## Unit Tests

### When a test is not a unit test

Michael Feather's definition can help teams figure out what should not be considered a unit test:

A test is not a unit test if:
  It talks to the database
  It communicates across the network
  It touches the file system
  It can't run at the same time as any of your other unit tests
  You have to do special things to your environment (such as editing [configuration] files) to run it

Chris Sterling, Managing Software Debt, p37