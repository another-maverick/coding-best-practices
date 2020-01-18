# Lines and Bounadries

* **Third party code challenges**: Interface provider wants the interface to be as generic as possible. Users of the interface on the other hand want the interface to be as specific to their need as possible
    * For example: If the interface has delete method that could be dangerous - You can enclose  the implementation with a custom class and create a "boundary". This results in code that is harder to misuse and still easier to understand
* **How to understand third party code well** - Write tests to explore the usage of third party code. Approach commmonly called as *Learning Tests*
    * Example: If you want to use logging third party code, run test code on logging libaries using ipython or jupyter(in case of python). Do trial and error. Get help from Google and understand the code better before using it in your "prod" code
    * When the third party code changes, you would want to run the learning tests again to ensure your prevoius understanding still holds true. In this case, the learning test also behaves as *boundary test*
* **Boundaries** are important to ensure our software is able to keep up with the changes without huge time and effort wasted in refactoring
