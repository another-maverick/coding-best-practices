# Concurrency
* Concurrency does not always improve performance. You need to understand if the wait time (say during I/O for example) can be used by other processes. It means differently in Python and GO. 
* Be mindful of **race** conditions when you are writing code that will make use of Concurrency
* If the problem requires code to run in a concurrent way, prefer using GO. Its support for conurrency is better.
* Use **Mutex**, **locks** and **semaphore**as required
* Study algorithms such as **Dining Philosophers** algorithm. This will help in avoiding deadlocks
* Keep synchorized sections as small as possible. Synchronized resources need a *lock*
* Test code with one and more processors. (you can do this in GO. NOt sure if it is convinient in other languages)
* Do not treat system failures as one-offs(especcially in concurrent applications)
