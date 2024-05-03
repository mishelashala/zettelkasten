# Tests as reliable documentation

"Tests provide the only reliable documentation of design. The story they tell remains true long after paper documents become obsolete and human memory fails."

Sandi Metz, Practical Object-Oriented Design, p195

# Testing incoming vs outgoing messages

"Incoming messages should be tested for the state they return. Outgoing command messages should be tested to ensure they get sent. Outgoing query messages should not be tested."

Sandi Metz, Practical Object-Oriented Design, p198

# Well designed code and tests

"Costly tests do not necessarily mean that the application is poorly designed. It is quite technically possible to write bad tests for well-designed code. Therefore, for tests to lower your costs, both the underlying application _and_ the tests must be well-designed."

Sandi Metz, Practical Object-Oriented Design, p196

# Tests of state

"Tests that make assertions about the values that messages return are tests of _state_. Such tests commonly assert that the results returned by a message equal an expected value."

Sandi Metz, Practical Object-Oriented Design, p198