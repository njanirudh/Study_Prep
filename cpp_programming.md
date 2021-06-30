### C++ Programming 

#### Philosophy
* General rules:
    *  Don't postpone to run time what can be done to compile time.
    *  Dont use raw pointers (new, delete).
    *  Express ideas directly in code not by comments (const, naming).
    *  Use stdlibs whenever possible.
    *  

#### std::
* std::span
* 

#### Design 

* Run-time vs Compile time errors:
   * Compile-time
      * Program should satisfy all variants (syntax, type)
      * eg. Syntax errors, Typecheck errors
   * Run-time 
      * Run-time invariants require human + compiler help.
      * eg. Division by zero, Dereferencing a null pointer, Running out of memory
         

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

#### Template Metaprogramming
* 


#### Concurrency




#### References:
1. https://stackoverflow.com/questions/846103/runtime-vs-compile-time
2. https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines#S-introduction
