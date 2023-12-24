# Unit-1: introduction to C++

C++ is a statically-typed, free-form, (usually) compiled, multi-paradigm, intermediate-level general-purpose middle-level programming language.”

In simple terms, C++ is a sophisticated, efficient and a general-purpose programming language based on C. It was developed by BjarneStroustrup in 1979.


## FEATURES OF C++

- C++ is fast
- C++  is statically typed
- C++ is a multi-paradigm programming language
- Object oriented programming with C++
- Power of standard library (Standard template library – STL)

### Object
This is the basic unit of object oriented programming. That is both data and function that operate on data are bundled as a unit called as object.

### Class
When you define a class, you define a blueprint for an object. This doesn’t actually define any data, but it does define what the class name means, that is, what an object of the class will consist of and what operations can be performed on such an object.

### Abstraction
Data abstraction refers to, providing only essential information to the outside world and hiding their background details, i.e., to represent the needed information in program without presenting the details.

For example, a database system hides certain details of how data is stored and created and maintained. Similar way, C++ classes provides different methods to the outside world without giving internal detail about those methods and data.

### Encapsulation
Encapsulation is placing the data and the functions that work on that data in the same place. While working with procedural languages, it is not always clear which functions work on which variables but object-oriented programming provides you framework to place the data and the relevant functions together in the same object.

### Inheritance
One of the most useful aspects of object-oriented programming is code reusability. As the name suggests Inheritance is the process of forming a new class from an existing class that is from the existing class called as base class, new class is formed called as derived class.

This is a very important concept of object-oriented programming since this feature helps to reduce the code size.


### Polymorphism  (same function acts diff with diff params)
The ability to use an operator or function in different ways in other words giving different meaning or functions to the operators or functions is called polymorphism. Poly refers to many. That is a single function or an operator functioning in many ways different upon the usage is called polymorphism.

### Overloading ( a + b = 'hello world')
The concept of overloading is also a branch of polymorphism. When the exiting operator or function is made to operate on new data type, it is said to be overloaded.



Here's a concise explanation of bottom-up and top-down approaches in programming:

### Bottom-up approach:

Starts with the smallest, most basic components.
Builds up to more complex solutions by combining those components.
Often iterative, using loops and data structures to build solutions step by step.
Common in dynamic programming, where smaller subproblems are solved first to solve larger problems.
Example:

Calculating Fibonacci numbers: Start with base cases (F0 = 0, F1 = 1), then iteratively compute larger numbers using the formula Fn = Fn-1 + Fn-2.
Top-down approach:

Starts with the overall problem and breaks it down into smaller subproblems.
Solves subproblems recursively or iteratively, then combines solutions to solve the larger problem.
Often involves function calls or recursion to break down problems into smaller parts.
Can be less efficient in terms of memory usage due to potential recursion overhead.
Example:

Merge sort algorithm: Divides the array into halves repeatedly until subarrays are single elements, then merges them back in sorted order.

### DIFFERENCE BETWEEN C AND C++
C Programming Language

- C language was developed in 1972 by Dennis Ritchie.

- C is a Procedural Oriented Programming language.

- C has Top Down programming approach.

- In c programming language, a big problem divides into small pieces known as functions; this approach of programming is known as Modular programming.

- Structure in C does not have function declaration features i.e. we cannot declare a function as member function of structure in C.

### C++ Programming Language
- C++ language was developed in 1980 by BjarneStrostroup.

- C++ is an Object Oriented Programming language.

- C++ has Bottom Up programming approach.

- In c++ programming language, a big problem divides into Classes and Objects.

- Structure in C++ provide the feature of declare a function as member function of structure.

New and delete operator
The new operator
The new operator requests for the memory allocation in heap. If the sufficient memory is available, it initializes the memory to the pointer variable and returns its address.

Here is the syntax of new operator in C++ language,

pointer_variable = new datatype;
Here is the syntax to initialize the memory,

pointer_variable = new datatype(value);
Here is the syntax to allocate a block of memory,

pointer_variable = new datatype[size];

The delete operator
The delete operator is used to deallocate the memory. User has privilege to deallocate the created pointer variable by this delete operator.

Here is the syntax of delete operator in C++ language,

delete pointer_variable;
Here is the syntax to delete the block of allocated memory,

delete[ ] pointer_variable;


### Here are examples of each type of operator in C++:

## Assignment Operator (=)

Assigns a value to a variable.
Example: x = 10; assigns the value 10 to the variable x.

# Mathematical Operators

Perform arithmetic operations.
Examples:
Addition: + (e.g., result = 5 + 3)
Subtraction: - (e.g., difference = 10 - 4)
Multiplication: * (e.g., product = 2 * 6)
Division: / (e.g., quotient = 12 / 3)
Modulus (remainder): % (e.g., remainder = 17 % 4)

## Relational Operators

Compare values and return a boolean result (true or false).
Examples:
Equal to: == (e.g., if (x == y) { ... })
Not equal to: != (e.g., if (a != b) { ... })
Greater than: > (e.g., while (count > 0) { ... })
Less than: < (e.g., if (temp < 25) { ... })
Greater than or equal to: >=
Less than or equal to: <=

## Logical Operators

Combine boolean expressions.
Examples:
AND: && (e.g., if (isMember && hasPaid) { ... })
OR: || (e.g., if (age >= 18 || hasGuardian) { ... })
NOT: ! (e.g., if (!isValid) { ... })

## Bitwise Operators

Perform operations on individual bits of integer values.
Examples:
AND: &
OR: |
XOR: ^
NOT: ~
Left shift: <<
Right shift: >>

## Shift Operators

Shift bits of an integer value to the left or right.
Examples:
Left shift: << (e.g., result = value << 2)
Right shift: >> (e.g., result = value >> 3)

## Unary Operators

Operate on a single operand.
Examples:
Increment: ++ (e.g., x++;, ++x;)
Decrement: -- (e.g., y--;, --y;)
Negation: - (e.g., -value)
Logical NOT: ! (e.g., !isAvailable)
Address-of: & (e.g., &x)
Dereference: * (e.g., *ptr)

## Ternary Operator (?:)

A conditional expression that takes three operands.
Example: result = (condition) ? valueIfTrue : valueIfFalse;

## Comma Operator (,)

Evaluates multiple expressions sequentially, returning the value of the last expression.
Example: x = (y = 3, y + 2); assigns 5 to x and 3 to y.
