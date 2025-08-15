### Programs
To make a program run, its source text has to be processed by a compiler, producing object files, these files are combined by a linker yielding an executable program.
(Put image here)

An executable program is created for a specific hardware,this means it is not portable. 

### Functions
A function cannot be called unless it has been declared. 
Function declaration (needs):
1. Type of returned value
2. Name of the function
3. Number and types of arguments that it takes
4. (optional) Name of the arguments it takes
#### Function overloading
When 2 functions are defined with the same name, but take different argument types, the compiler automatically chooses which one to call.
**careful** -> when 2 functions can be called but neither is better than the other, the compiler will give an error. 
Each function with the same name should implement the same functionality 
Example: printf(), each printf prints its argument. 

### Types, Variables and Arithmetic
The size of a type is implementation-defined (it can vary among different machines), if we want to use a specific type, we use values like **uint32_t** . 
#### Arithmetic
all the different types of ++,== ... and so on...

#### Initialization
Before and object can be used, it must be given a value.  There are different ways to do so:
```cpp
double d1 = 2.3;    //old c way of doing it
double d2 {2.3};    // cpp form
double d2 = {2.3};  // cpp form, the = is optional

complex<double> z = 1;
complex<double> z2 {d1,d2}
```
