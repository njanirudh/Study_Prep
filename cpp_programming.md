### C++ Programming 

#### Design 

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

#### Concurrency

* 
