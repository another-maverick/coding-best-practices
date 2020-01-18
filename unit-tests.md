# Unit Tests
* Important part of **Test Driven Development**. Idea is to write tests that are meaningful. Use mock tests whereever possible. Also, **make sure the tests are easy for others to execute**
##  Three laws of TDD
    * Dont write Production code until you have written one Unit Test that fails
    * Dont write more of a unit test than is sufficient to fail. Not compiling is failing
    * Dont write more Prod code than what is sufficient to pass the currently failing test

## Clean Tests
* Clean tests are important. "Quick and dirty" tests are equivalent to no tests. 
* Tests must change as the prod code evolves. If the tests are dirty, it will hard to keep up. This has a direct impact on how frequent you can make Prod code changes and how confident are you with those changes
* What makes a code clean? **Readability**. Less duplication.
* Use BUILD-OPERATE_CHECK design pattern
    * Build the test data
    * Operate on the data
    * Check if operation yielded right results
* One thing you de-prioritize, is the efficiency. The testb code does not have to be as *efficient* as prod code
* Duplication can be reduced by using *TEMPLATE PATTERN*. Separate "Given" in the template and  "then" + "when" in the derived code" 
* Try to have one assert per test
* Try to have "single concept" per test

