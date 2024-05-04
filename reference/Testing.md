# Tests as reliable documentation

"Tests provide the only reliable documentation of design. The story they tell remains true long after paper documents become obsolete and human memory fails."

Sandi Metz, Practical Object-Oriented Design, p195

# Testing incoming vs outgoing messages

"Incoming messages should be tested for the state they return. Outgoing command messages should be tested to ensure they get sent. Outgoing query messages should not be tested."

Sandi Metz, Practical Object-Oriented Design, p198

# Well designed code and tests

"Costly tests do not necessarily mean that the application is poorly designed. It is quite technically possible to write bad tests for well-designed code. Therefore, for tests to lower your costs, both the underlying application _and_ the tests must be well-designed."

Sandi Metz, Practical Object-Oriented Design, p196

# Testing is not only for QA

"Everyone on the team should be able to execute any and all automated and manual test cases."

Chris Sterling, Managing Software Debt, p59

# The goal of developers when writing tests

"Our goal as developers is to write specs that maximize the values we've listed here-guiding the design, building confidence, and so on-while minimizing the time lost to writing, running, and fixing them."

Effective Testing with RSpec 3, p39

# Unit Specs

"[...] unit focus on individual units of code--often as small as a single object or method."

Effective Testing with RSpec 3, p39

# Integration Specs

"Code that interacts with an external service--such as a database or third-party REST API--should have an integration spec."

Effective Testing with RSpec 3, p40

# Tests of state

"Tests that make assertions about the values that messages return are tests of _state_. Such tests commonly assert that the results returned by a message equal an expected value."

Sandi Metz, Practical Object-Oriented Design, p198

# Acceptance Specs

"Acceptance specs describe a feature in an end-to-end, back-box style that exercises the entire system."

Effective Testing with RSpec 3, p39