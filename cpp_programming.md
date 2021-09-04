### C++ Programming 

<details>
  <summary>  </summary> 
 
 [(src)]()
   
</details>

   
#### Philosophy
    
<details>
  <summary> General rules </summary> 
 
 [(src)]()
*  Don't postpone to run time what can be done to compile time.
*  Dont use raw pointers (new, delete).
*  Express ideas directly in code not by comments (const, naming).
*  Use stdlibs whenever possible.
</details>

#### std::

<details>
  <summary> std::span </summary> 
 
 [(src)](https://en.cppreference.com/w/cpp/container/span)
* Lightweight abstraction that describes a contiguous sequence of objects. 
</details>

<details>
  <summary> When should you use std::endl vs '/n' for new line? </summary> 
 
 [(src)]()
* std::endl causes the buffer to be flushed.   

</details>

<details>
  <summary> namespace </summary> 
 
 [(src)](https://docs.microsoft.com/en-us/cpp/cpp/namespaces-cpp?view=msvc-160#:~:text=A%20namespace%20is%20a%20declarative,code%20base%20includes%20multiple%20libraries.)
* declarative region that provides a scope to the identifiers 
* Prevents name collsions.   
</details>

<details>
  <summary> vector, set, map </summary> 
 
 [(src)](https://stackoverflow.com/questions/3389648/what-is-the-difference-between-stdliststdpair-and-stdmap-in-c-stl)
 [(src)]()
* vector
  * 
* set
  * 
* pair
  * stores two heterogeneous objects. 
* map
  * Associative container.
  * <key, value>
  * offers indexing , map[key]
  * logarithmic time
</details>

  
<details>
  <summary> array vs vector vs list </summary> 
 
 [(src)](https://stackoverflow.com/questions/1905417/array-vs-vector-vs-list, https://stackoverflow.com/questions/4424579/stdvector-versus-stdarray-in-c)
   
</details>


<details>
  <summary> noexcept </summary> 
 
 [(src)]()
 * Specifies that the function dosn't throw any exception. 
   
</details>

#### Design 

* C++ 11 Memory model

<details>
  <summary> Compilation steps in C++ </summary> 
 
 [(src)](https://stackoverflow.com/questions/6264249/how-does-the-compilation-linking-process-work)
 * The three major steps are:
    * Preprocesing
       * Replaces #includes, #defines and other preprocessing directives.
    * Compilation
      * Convert the C++ code into assembly code. 
    * Linking
      * Object files from compilers are converted into libraries or executables.
      * Links to external libraries. 
</details>


<details>
  <summary> Run-time vs Compile-time </summary> 
 
 [(src)](https://stackoverflow.com/questions/846103/runtime-vs-compile-time)
   * Run-time 
   
</details>


<details>
  <summary> Run-time vs Compile time errors </summary> 
 
 [(src)](https://stackoverflow.com/questions/846103/runtime-vs-compile-time)
  
 * Compile-time errors
      * Program should satisfy all variants (syntax, type)
      * eg. Syntax errors, Typecheck errors
 * Run-time errors
      * Run-time invariants require human + compiler help.
      * eg. Division by zero, Dereferencing a null pointer, Running out of memory
</details>

<details>
  <summary> Stack vs Heap initialization </summary> 
 [(src)](https://www.learncpp.com/cpp-tutorial/the-stack-and-the-heap/)

* Stack Initialization
  * Faster allocation and deallocation.
  * Small variables can be stored for fast access.
  * Pointer is created on the stack.
* Heap Initialization
  * Memory allocation is slow
  * Memory should be explicitly cleaned up if 'new' and 'delete' are used.
  * Heap is a large pool of memory, so big objects must be created on the heap.
</details>


* Improvements of C++ over previous versions
    * Type safety
    * Prevent accidents
    * Auto destruction and memory freeing 

* Common violations
    * Type violation
    * Bounds violation
    * Lifetime violation

* RTTI : Run-time type information
    * C++ function to determine type information at runtime.
    * Can be used for same type casts (dynamic, static).

* static_cast vs dynamic_cast vs regular_cast vs reinterpret_cast 
    * Dynamic_cast 
      * Run-time cast
      * Used for polymorphic classes.
      * Type checking is involved (RTTI)
      * Overhead due to type check
    * Static_cast
      * Compile time cast
      * Reverse an implicit conversion
      * No type checking involved
      * Less overhead

* RAII : Resource Acquisition is Initialization
    * The idiom of having constructors acquire resources and destructors release them is called RAII.

* 'volatile 'keyword
   * Prevents over optimization from the compiler.  

<details>
  <summary>  Header Only vs Compiled Libs </summary> 
 
 [(src)](https://stackoverflow.com/questions/12671383/benefits-of-header-only-libraries)
* Header Only
   * Easier to package and distribute.
   * Simplifies the build process.
   * No linking process.  
   * Longer compilation time.
* Compiled Libs
   * 
   * 
</details>




<details>
  <summary> Composition vs Inheritance </summary> 
 
 [(src)]()
   
</details>

#### Template Metaprogramming

<details>
  <summary>  Advantage and Disadvantage of using Templates </summary> 
[(src)](https://isocpp.org/wiki/faq/templates)
   
   * Advantages
      * Builds a family of classes or functions.
      * Reduces reundant code. 
   * Disadvantages 
      * Difficult in maintanence.
      * Slow to compile.
      * 
   
</details>


#### Concurrency
* Lock free
* std::atomic
* 



#### References:
2. https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines#S-introduction
