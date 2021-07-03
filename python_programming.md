### Python Programming

* How is random implemented in python?   
  * Mersenne Twister pseudo-random number generator.
  * System random generator.

* Datastructure implementations:
  * set 
  * map
  * list 
 
 * What are context managers in python?
  * 

* Are there pointers in python?  


* PyObject   
  * Most basic object in python.
  * Eveything is a PyObject.
  * It has Type, Reference Count, value 

* Immutable vs Mutable datastructures?
  * Immutable objects cannot be changed in program. eg. 
  * Mutable objects can be changed. eg. list()   

* Sort implementations in python?
  * An hybrid sort called as Tim sort is used. ==>  O(n log n)
  * Insertion sort (~ 64 items) ==> O(n^2)
  * Merge sort (64<) ==> O(n log n)

* Memory allocation in python?  
  *  Reference counting
  *  Garbage collection

* What is a reference cycle?  
  * When an object refers to itself its called reference cycle.
  * eg. l = []; l.append(l);
  * Normal garbage collection has problems in detection referece cycles.
 
* Python magic methods?
  * Special methods in a python class.
  * __init__, __new__, __add__ etc.
  * Used for operator overloading.

* Global Interpreter Lock (GIL)  
  * It is a mutex (lock) used to prevent access to python objects from multiple threads.
  * Prevents proper mutithreading.

* Deep copy vs Shallow copy  
  * Deep copy
   * Makes a completely new copy of object.
  * Shallow copy
   * Makes only a reference to an object. 
  
* Type Introspection and Reflection
  * Type Introspection
    * Ability of the program to examine its type at runtime.
    * type()
  * Reflection
    * Uses type introspection.
    * Uses it to change properties of object at runtime.
    * Use cases :
      * As part of software testing, such as for the runtime creation/instantiation of mock objects.
      * Deserializing, serialization 
    * getattr() 

* What are generators?
  * Return a lazy iterator.
  * Unlike list the values are not stored in memory.
  * Uses : Reading large files in memory. 
  * next() can be used on generator object.
  
* What does yield expression do?
  * Used along with generators.
  * 
  
* Different ways to create a generator?
  * generator functions
  * generator statements  

### References
1. https://rszalski.github.io/magicmethods/#reflection
2. https://stackoverflow.com/questions/25198271/what-is-the-difference-between-introspection-and-reflectionf
3. https://docs.python.org/3/library/random.html
4. https://stackoverflow.com/questions/27683764/what-is-a-pyobject-in-python
5. https://nickmccullum.com/python-pointers/
6. https://www.geeksforgeeks.org/garbage-collection-python/
7. https://stackoverflow.com/questions/4828080/how-to-make-an-immutable-object-in-python
8. https://realpython.com/introduction-to-python-generators/
