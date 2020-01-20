# Functions
* Functions should be **small**. How  long? Normally,  they should be less than 20 lines long
* More number of small functions is better than less number of large functions
* Functions should **do only one thing** and there should **not have un-desired side effects**. For example a function that is supposed to list customer names should not add/change anything
* Use consistent indentation
* Use **descriptive** names. Dont worry about the names being long. As long as they are descriptive, its okay
* There should be less number of  arguments. Ideally 0. 1, 2, or 3 (in the order of preference). More than 3 arguments is not good.
    * As we increase the number of arguments, tets become harder too. There would be higher number of combinations
* Passing **boolean** arguments is bad. For example "display(true)"  can get confusing
* If you are using more than 3 arguments, mostly instead of using the extra args, you can create a class of their own
* Function names should be **verbs**. For example "write(name)" is not very descriptive. Whatever the name is, is unknown. If we use "writeField(name)" gives an idea that name thats being written is a Field
* If the functions must chnage the state of  something, have it change the state of its owning object
* Throw an exception instead of an error code
* DRY(Dont Repeat Yourself). Object Oriented programming can come to the rescue. **Interfaces, abstract classes** can be used to reduce duplication
* Try not having multiple returns in the function

