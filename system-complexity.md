# System Complexity
* start up process when objects are constructed should be held separate from the run time logic
* We should have a common way of resolving dependencies suring object creation
* One way is to move construction to "main"
    * main builds the objects that are necessary for the application and passes them over to the app. App has no idea of how the objects are created. It just knows that it will have them avaialble.
* Sometimes application  needs to create objects. in those cases, try to use **Abstract Factory** pattern to givve application control of when/how objects are constructed but it does not know the internals how its done
    * example: factory implementataion is on the "main"  side of the code. Application calls it to create objects
## Dependency Injection
* A mechanism to separate "construction" from "use"
* An object should not take the job of instantiating dependencies itself. It should pass control to other objects
* A class doed not instantiate dependencies by itself. Instead it uses "setters" or "constructor arguments" to set dependencies
# Dont overthink about the future scale
* As an example: Small settlements grow into towns which grow into cities organically over time and then we have skyscrapers etc. There is no point of having a 6 lane freeway in small town just because it might make sense at some time
    * Similarly, dont worry about getting the scale "right" the very first time. Get the basics right. Work on Test Driven Development and follow DRY principle etc.
* Standards are "proven" guidelines. Sometimes "creation of standards" can be too long for the insustry to wait. Sometimes we need to adapt to the "real" needs at hand. When there is uncertainity, think about **the simplest thing that can work**
