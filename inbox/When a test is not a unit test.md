Michael Feather's definition can help teams figure out what should not be considered a unit test:

A test is not a unit test if:
  It talks to the database
  It communicates across the network
  It touches the file system
  It can't run at the same time as any of your other unit tests
  You have to do special things to your environment (such as editing [configuration] files) to run it

Chris Sterling, Managing Software Debt, p37