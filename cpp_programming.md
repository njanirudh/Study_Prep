### C++ Programming 

<details>
  <summary>  </summary> 
 
 [(src)]()
   
</details>

--------------
#### Philosophy
    
<details>
  <summary> General rules </summary> 
 
 [(src)]()
*  Don't postpone to run time what can be done to compile time.
*  Dont use raw pointers (new, delete).
*  Express ideas directly in code not by comments (const, naming).
*  Use stdlibs whenever possible.
</details>

--------------
#### STL 

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
  <summary> std::vector, std::set, std::map, std::pair </summary> 
 
 [(src)](https://stackoverflow.com/questions/3389648/what-is-the-difference-between-stdliststdpair-and-stdmap-in-c-stl)
 [(src)]()
* std::vector
  * 
* std::set
  * 
* std::pair
  * stores two heterogeneous objects. 
* std::map
  * Associative container.
  * <key, value>
  * offers indexing , map[key]
  * logarithmic time
</details>

  
<details>
  <summary> std::array vs std::vector vs std::list </summary> 
 
 [(src)](https://stackoverflow.com/questions/1905417/array-vs-vector-vs-list)
 [(src)]( https://stackoverflow.com/questions/4424579/stdvector-versus-stdarray-in-c)
   
</details>


<details>
  <summary> noexcept </summary> 
 
 [(src)](https://en.cppreference.com/w/cpp/language/noexcept_spec)
 * Specifies that the function dosn't throw any exception. 
   
</details>

--------------
#### Design 

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
  *
* Compile-time   
  *   
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
<summary> The rule of three/five/zero </summary> 
 
[(src)](https://en.cppreference.com/w/cpp/language/rule_of_three)
*  Rule of 3
  * If a class requires a user-defined destructor, a user-defined copy constructor, or a user-defined copy assignment operator, it almost certainly requires all three.
*  Rule of 5
  * 
* Rule of 0
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

  
<details>
  <summary> Improvements of modern C++ over previous versions </summary> 
 
 [(src)]()
* Type safety
* Prevent accidents
* Auto destruction and memory freeing
</details>
  

<details>
  <summary> Common violations </summary> 
 
 [(src)]()
* Type violation
* Bounds violation
* Lifetime violation
  
</details>

<details>
  <summary> RTTI : Run-time type information </summary> 
 
 [(src)]()
* C++ function to determine type information at runtime.
* Can be used for same type casts (dynamic, static).
  
</details>


<details>
  <summary> static_cast vs dynamic_cast vs regular_cast vs reinterpret_cast </summary> 
 
 [(src)]()
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
</details>
  

<details>
  <summary> RAII : Resource Acquisition is Initialization </summary> 
 
 [(src)]()
* The idiom of having constructors acquire resources and destructors release them is called RAII.
  
</details>
  

<details>
  <summary> volatile </summary> 
 
 [(src)]()
* Prevents over optimization from the compiler.     
</details>


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
 
 [(src)](https://stackoverflow.com/questions/49002/prefer-composition-over-inheritance)

 * Composition
  * 
 * Inheritance
  *  
  
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

--------------
#### General
<details>
  <summary> X && </summary> 
 
 [(src)](https://www.modernescpp.com/index.php/c-core-guidelines-how-to-pass-function-parameters)
  * r-value reference
  * std::move() should be used to pass variables.
</details>

  
<details>
  <summary> 'const int* ptr'  vs  'int * const ptr' </summary> 
 
 [(src)](https://stackoverflow.com/questions/21476869/constant-pointer-vs-pointer-to-constant)
  
 * 'int * const ptr'
    * These type of pointers are the one which cannot change address they are pointing to.
    * You cant increment or decrement pointers.
 * 'const int* ptr'
    * These type of pointers are the one which cannot change the value they are pointing to.

</details>

<details>
  <summary> Linked List vs std::vector </summary> 
 
 [(src)](https://stackoverflow.com/questions/4700052/are-vector-a-special-case-of-linked-lists)
 *
  
</details>

<details>
  <summary> V-Tables in C++ </summary> 
 
 [(src)](https://www.learncpp.com/cpp-tutorial/the-virtual-table/)
 * Lookup table to resolve function calls in a dynamic/late binding.
 * Used to implement virtual functions.
</details>

<details>
<summary> move constructor, move-assignment, copy constructor, copy-assignment </summary> 
 
 [(src)]()
* move constructor
  * 
* move assignment
  * 
* copy constructor
  * 
* copy assignment
  * 
</details>

<details>
<summary> Value categories (lvalue, rvalue)</summary> 
 
[(src)](https://www.fluentcpp.com/2018/02/06/understanding-lvalues-rvalues-and-their-references/)
* If it’s got a name, it’s an lvalue, otherwise it’s an rvalue. `move` and `forward` convert lvalues (even ones to rvalues!) into rvalues
  
</details>
  
<details>
  <summary> </summary> 
 
 [(src)]()
   
</details>
  
#### Concurrency

<details>
  <summary> Disadvantages of Locking </summary> 
 
 [(src)](https://www.cs.cmu.edu/~410-s05/lectures/L31_LockFree.pdf)
 [(src)](https://stackoverflow.com/questions/3601602/what-are-rvalues-lvalues-xvalues-glvalues-and-prvalues)

* Deadlock : Waiting for resource to be freed. 
* Priority Inversion : Low-priority processes hold a lock required by a higherpriority process.
  
</details>


<details>
  <summary> std::atomic </summary> 
 
 [(src)]()
   
</details>


--------------
#### References:
2. https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines#S-introduction
