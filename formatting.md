#Formatting

* Helps with readability and maintainability of the code

## File Size and contents

* The size of the files should be **not more than 200 lines generally**. Upper limit ~ 500
* The name should be simple and should explain about the purpose of the file
* Top part of the file should provide most high level details about the data. As we go down, in-depth details are obtained
* Two blank lines between classes. One blank line between functions
* Lines of code that are closely related should appear dense. Otherwise, u got to use too much of eye plus head movement to make sense out of the code
* Concepts that are related should be kept as close as possible to each other. You dont want to be jumping too much to make sense out ot it
    * Ofcourse this does not apply when related code is in different files but then closely related code should not be kept in separate files
* **Variables** should be declared as **close to the usage** as possible
* **Instance Variables** should be declared at the top of the class
* **When a function calls other function** the one which calls should be above the one which is called. For example, if *a* calls *b*, then *a* should be declared first and then *b*
* **Functions that are similar in nature like getuser, getcustomer** etc should be placed close to each other
* **Length of each line** should generally be **not more than 80 chars**


## Separation in a line
* **Assignment should have whitespace**. example: a = 5
* **No space between function definition and paranthesis open**. example: myFunc()
* **Arguments should be separated by a comma**. example: myFunc(a, b, c)
* Equation
    * **Equation** -- a*b + c*d -e*f **No space between * since its higher in precedence. There is space for + and - since its lower in precedence**


## Indentation
* **Statements** at the level of file
* **Classes** mostly to the level of file
* **Method** one level to the right of class
* **Method Implementation** should be one level right of Method declaration

