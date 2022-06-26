### Python Programming

<details>
  <summary> Tuple/dict unpacking in Python </summary> 
 
 [(src)](https://treyhunner.com/2018/10/asterisks-in-python-what-they-are-and-how-to-use-them/#:~:text=The%20**%20operator%20allows%20us,arguments%20in%20a%20function%20call.&text=Functions%20in%20Python%20can't,an%20exception%20will%20be%20raised.)
 Unpacking can be done using ** operator in python.  
</details>

<details>
  <summary> How is random implemented in python? </summary> 
 
 [(src)](https://docs.python.org/3/library/random.html)
  * Mersenne Twister pseudo-random number generator.
  * System random generator.
</details>

<details>
  <summary> Datastructure implementations in python? </summary> 
 
 [(src)]()
  * set 
  * map
  * list 
</details>

<details>
  <summary> List vs Set? </summary> 
  * list
    * persistant 
    * keeps ordering
    * allows duplicates
  * set 
    * random ordering
    * dosn't allow duplicates 
</details>

<details>
  <summary> Difference between 'global' and 'nonlocal' keywords? </summary> 
   * global
     * global is that it only works for global variables. 
     * It cannot see variables in an enclosing, nonglobal scope 
   * nonlocal 
     * Define the total variable as non-local, causing it to bind to the nearest non-global variable.
</details>

<details>
  <summary> Different levels of variable scopes? </summary> 
    * global
   * local
   * nonlocal
</details>
 
<details>
  <summary> What are context managers in python? </summary> 
 </details>
 
<details>
  <summary> Are there pointers in python? </summary> 
 </details>
  
 <details>
  <summary> What are Closures? </summary> 
    * A closure is an inner function with an extended scope that encompasses nonlocal variables of the outer function. 
 </details>
 
 <details>
  <summary> PyObject </summary> 
  * Most basic object in python.
  * Eveything is a PyObject.
  * It has Type, Reference Count, value 
 </details>
 
 <details>
  <summary> Immutable vs Mutable datastructures? </summary> 
  * Immutable objects cannot be changed in program. eg. 
  * Mutable objects can be changed. eg. list()   
 </details>

 <details>
  <summary> Sort implementations in python? </summary> 
  * An hybrid sort called as Tim sort is used. ==>  O(n log n)
  * Insertion sort (~ 64 items) ==> O(n^2)
  * Merge sort (64<) ==> O(n log n)
 </details>
 
<details>
  <summary> Sort implementations in python? </summary> 
  * An hybrid sort called as Tim sort is used. ==>  O(n log n)
  * Insertion sort (~ 64 items) ==> O(n^2)
  * Merge sort (64<) ==> O(n log n)
 </details>

<details>
  <summary> Memory allocation in python? </summary>
  *  Reference counting
  *  Garbage collection
 </details>
  
<details>
  <summary> What is a reference cycle? </summary> 
  * When an object refers to itself its called reference cycle.
  * eg. l = []; l.append(l);
  * Normal garbage collection has problems in detection referece cycles.
 </details>

<details>
  <summary> Python magic methods? </summary> 
  * Special methods in a python class.
  * __init__, __new__, __add__ etc.
  * Used for operator overloading.
 </details>
   
   
<details>
  <summary> Global Interpreter Lock (GIL) </summary> 
  * It is a mutex (lock) used to prevent access to python objects from multiple threads.
  * Prevents proper mutithreading.
 </details>
   
<details>
  <summary> Deep copy vs Shallow copy   </summary> 
  * Deep copy
    * Makes a completely new copy of object.
  * Shallow copy
    * Makes only a reference to an object. 
</details>
 
<details>
  <summary> Type Introspection and Reflection </summary> 
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
</details>
 
<details>
  <summary> What are generators? </summary> 
  * Return a lazy iterator.
  * Unlike list the values are not stored in memory.
  * Data can be used only once.
  * Uses : Reading large files in memory. 
  * next() can be used on generator object.
</details>
  
<details>
  <summary> What does yield expression do? </summary> 
  * Used along with generators.
  * returns a value and runs till next yield statement or end of generator.
</details>

<details>
  <summary> Different ways to create a generator? </summary> 
   [(src)](https://realpython.com/introduction-to-python-generators/)
    * generator functions
  * generator statements  
</details>


### References
1. https://rszalski.github.io/magicmethods/#reflection
2. https://stackoverflow.com/questions/25198271/what-is-the-difference-between-introspection-and-reflectionf
4. https://stackoverflow.com/questions/27683764/what-is-a-pyobject-in-python
5. https://nickmccullum.com/python-pointers/
6. https://www.geeksforgeeks.org/garbage-collection-python/
7. https://stackoverflow.com/questions/4828080/how-to-make-an-immutable-object-in-python
