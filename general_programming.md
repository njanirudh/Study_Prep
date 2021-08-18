### General Programming

* Static vs Dynamic programming languages?
    * Static programming language
      * Before running the data type of each variable is checked.
      * Done by a compiler.
      * Invalid assignments give compile-error.
      * eg. C++

    * Dynamic programming languages
      * Data types are known only after running the programme.
      * Runtime errors.
      * eg. Python

* Duck typing
    * Dynamic languages 

<details>
  <summary> Language Processors: Assembler, Compiler and Interpreter </summary> 
 
 [(src)](https://www.geeksforgeeks.org/language-processors-assembler-compiler-and-interpreter/)
 * Assembler
 * Compiler
 * Interpreter
</details>


#### Analysis
* Big O
* What is Amortized Analysis?

* What are different types of problem complexities?
  * Dimensional Complexity (2D, 3D ...ND data)
  * Analytic Complexity (polynomial degree 1, 2 ...N)
  * Combinatorial Complexity (O(nlogn)...)

#### Memory 

* Where are the stack and a heap memory stored?
   * RAM 

* Stack vs Heap vs Data Segment
 [(src)](https://stackoverflow.com/questions/79923/what-and-where-are-the-stack-and-heap)

   * Stack 
      * Small contiguous blocks of memory.
      * Each thread has its own stack.
      * Local variables are stored.
      * Scope: function start to end.
      * Error: Stack overflow.

   * Heap
      * Large fragmented memory. 
      * All threads have access to common heap memory.
      * Scope: application start to end.
      * Error: Out of memory.
   
   * Data Segment
      * Static objects and global objects are placed in data segment.
      * Dosn't change at run time.
      * Size depending on the total variables. 


### References
1. https://stackoverflow.com/questions/20563433/difference-between-static-and-dynamic-programming-languages#:~:text=A%20static%20language%20is%20a,compare%20to%20a%20dynamic%20language.
2. http://www.programmerinterview.com/data-structures/difference-between-stack-and-heap/
3. https://pages.mtu.edu/~shene/COURSES/cs3621/NOTES/overview/complexity.html
