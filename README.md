# Frontend Code Review


- Why code review
	- IMprove code quality
	- Collective learning internally
	- Catch issue before QA team

- The whole flow
	- Correct -> Readable -> Good quality

- How to conduct code review at frontend side

	- **Correct**: Run application locally and read PR's coressponding ticket to makre sure function works as expected
		- Does it satisfy the ticket requirements? (Read coressponding ticket description)
			- Business logic
			- UI effect
		- Does it change code behavior(old codebase、enhancement ticket)
		- Does it bring changes that out of scope
			- break other parts
			- purely out of scope
		- Dose it break tests
			- unit test
			- integration test
			- e2e test
	- **Readbility**
		- Is the code easy to read and comprehend?
		- Does it make clear what the business requirements are?
			- Logic flow is clear
			- Or with needed code comment
		- Are tests concise enough?
		- Does it use consistent coding convention
			- Are variables, functions, classes are named approperiately
			- Does the code work/organized in the same way how current/organization code convention work?
	- Basic
		- No ts warning?
		- No React warning at browser side?
	- Quality
		- Consitency
			- Good name to functions, variables, components?
			- Organized code in the same way with oragnaization or current codebase
		- KISS & maintainbility
			-  Do the codebase have duplication
			-  Does a function do too much work and need separation of concerns
			-  Does the code use variable constructure/deconstructure?
			-  Does a function use object as the way to pass parameters if the function more than two variables
			-  Store global used variables at single place or using Object
		- Test cases
			- One assert per test.
			- Readable.
			- Fast.
			- Independent.
			- Repeatable.
	- Performance
		- Event unregister
		- Rederning (React / Vue)
		- API request
		- Application performance


- References
	- [clean code summary](https://gist.github.com/wojteklu/73c6914cc446146b8b533c0988cf8d29)
	- [Maslow's pyramid of code review](https://www.dein.fr/posts/2015-02-18-maslows-pyramid-of-code-review)
	- [The code review](https://www.morling.dev/blog/the-code-review-pyramid/)



