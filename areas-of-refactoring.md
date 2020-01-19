# Refactoring

## Comments
### In appropriate Information
* Comments shuld only have tech notes about code. Authors, why the chnage is made, modified date etc. are better maintained  in GIT. Get rid of them
### Obsolete comment
* Get rid of old omments which are no longer valid. Get rid of them. Sometimes they stay for years.
### Redundant comments
* Anything that is already present in the code and is described by it, no need of comments here. Remove those
### Poorly Written Comments
* Comments should be well understood by all. If you cant understand some else's comment, thats an area of change
### Commented out code
* This should almost never be there. Just pollutes the file. Just remove it

## Environment
### Difficult Building process
* "Building" the code should be extremely simple, with not too many steps. If you have do a "lot" of work while building the code, thats an area for refactoring
### Difficult Testing Process
* Same rules as building. Should not be a difficult process

## Functions
### A lot of arguments
* In the oder of preference - Funtions should have no-args, 1, 2, 3. More than 3 is usually bad
### Output Args
* If the function is changing the state of something, its better to change the state on the object it is called on
### Flag Arguments
* Boolean arguments should not be used
### Dead Function
* Do not have methods that are never called. Remove those

## Generic
### Multiple languages in one source file
* Make effort to not have more than one language code in a file. Remove whereever possible
### NO surprises
* A fuction or a class should only do what it is advertising. No side effects. Try to remove if there are any
### Dont turn off safties
* For example turning off a test that fails is bad. Avoid this
### Duplication
* This should be avoided. DRY(Don't Repeat Yourself). Most of the times this presents an opportunity to create interfaces or abstract classes
* Modules that have similar algorithms and dont share the code
### Abstraction pitfalls
* You should only have the the "reuired" code in the base class. constants, variables, utility functions should not be present in the base class.
* base class should not depend on th child class
### Code  that is never used
* Functions that are never called, conditions that are never met etc. are not useful. Change these
### Separation
* Variables should be declared close to where they are used. Local variables shuld be declared right before their use
### Consistency
* There should be consistency in how variables are defined and named
### Selector Arguments
* Do not have boolena arguments. Not neat to pass true and false to the function in the arg list
### Placement of code
* Follow "least surprise" when making a decision as to where to place the code. Others should be able to make out whats going on by looking at the name of file, class or function
### Static methods in a class
* Think twice. Would this need to be static? When in doubt, make a method non-static
### Meaningful Names
* More variables with meaningful names is better than less variable with not-so-meaningful names. Refactor whenever needed. IDE's make it easy to refactor variable names
### Boolean Logic
* If you have multiple && or || in a "if" condition for example, try to have a function that checks the condition instead... like **if(eligibleForRaise())** instead of **if(<cond1> && <cond2>)** 

