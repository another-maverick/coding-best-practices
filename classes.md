# Classes
* **Classes shoud begin with a list of variables**. Public first and then private. (Having public variables is not a good practice)
* **Public Functions** should follow the list of variables
* Put private uitilities used by the public function right after the public function
## Classes should be small
* Same as functions, classes should be small
* Responsibility of each class should be as small as possible
* Name should be a **Noun** like "Manager", "Customer" etc and name should indicate what the class does
## Single Responsibility Principle (SRP)
* Class should have one responsibility. One reason to change. 
* There is nothing wrong with multiple small and single purpose classes
    * When we organize tools, its easier to search for a tool when they are organized in several small single purpose drawers than one giant drawer

## Moving on..
* classes should have small number of instance variables. A Method should not work on too many instances variables
## OPEN-CLOSED PRINCIPLE
* Classes should be open for extension(via sub classing etc) but closed for modification(just so existing clients dont break).
* Instead of writing concrete classes, **interfaces and abstract classes** can help here
## DEPENCENCY INVERSION PRINCIPLE
* Idea is to decouple similar classes as much as possible
* Classes should depend on abstractions and not on concrete implementation(related to OpenClosed principle)
* Instead of depending on a concrete base class, the child should be dependant on an abstract class or an interface



