# Control Flow
---
### Terminology
- Expression
- Statement
- Block

1. **Expression**
	something that produce a some value. It can made up of variables, operators and methods invocations.
	
	e.g
	```java
	name = "Piyush" // --> "Piyush"
	"My name is " + name // --> "My name is Piyush"
	a == b // --> true or false
	```
	
2. **Statement**
	A _statement_ forms a complete unit of execution.
	It is terminated by semicolon `;`.
	
	Types
	- Expression statements e.g. `str = "Hello"` etc.
	- Declaration statements e.g. `String name = "Piyush"` etc.
	- Control flow statements

3. **Block**
	zero or more statements between curly braces (`{` and `}`).

---

### Control Flow Statements
> The statements inside your source files are generally executed from top to bottom, in the order that they appear. _Control flow statements_, however, break up the flow of execution by employing **decision making**, **looping**, and **branching**, enabling your program to _conditionally_ execute particular blocks of code. - [Source](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/flow.html)

#### Decision Making
- `if`
- `if-else`
- `switch-case`
- `jump`
