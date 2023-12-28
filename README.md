# Unit-1: introduction to C++

C++ is a statically-typed, free-form, (usually) compiled, multi-paradigm, intermediate-level general-purpose middle-level programming language.”

In simple terms, C++ is a sophisticated, efficient and a general-purpose programming language based on C. It was developed by BjarneStroustrup in 1979.


## FEATURES OF C++

1.C++ is fast
2. C++  is statically typed
3 .C++ is a multi-paradigm programming language
4.Object oriented programming with C++
5.Power of standard library (Standard template library – STL)

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

Overloading ( a + b = 'hello world')
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

## DIFFERENCE BETWEEN C AND C++
- C Programming Language

        1. C language was developed in 1972 by Dennis Ritchie.

        2.  C is a Procedural Oriented Programming language.

        3. C has Top Down programming approach.

        4. In c programming language, a big problem divides into small pieces known as functions; this approach of programming is known as Modular programming.

        5. Structure in C does not have function declaration features i.e. we cannot declare a function as member function of structure in C.

- C++ Programming Language
        1. C++ language was developed in 1980 by BjarneStrostroup.

        2. C++ is an Object Oriented Programming language.

        3.  C++ has Bottom Up programming approach.

        4. In c++ programming language, a big problem divides into Classes and Objects.

        5. Structure in C++ provide the feature of declare a function as member function of structure.

### New and delete operator
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


Here are examples of each type of operator in C++:

1. Assignment Operator (=)

Assigns a value to a variable.
Example: x = 10; assigns the value 10 to the variable x.
2. Mathematical Operators

Perform arithmetic operations.
Examples:
Addition: + (e.g., result = 5 + 3)
Subtraction: - (e.g., difference = 10 - 4)
Multiplication: * (e.g., product = 2 * 6)
Division: / (e.g., quotient = 12 / 3)
Modulus (remainder): % (e.g., remainder = 17 % 4)
3. Relational Operators

Compare values and return a boolean result (true or false).
Examples:
Equal to: == (e.g., if (x == y) { ... })
Not equal to: != (e.g., if (a != b) { ... })
Greater than: > (e.g., while (count > 0) { ... })
Less than: < (e.g., if (temp < 25) { ... })
Greater than or equal to: >=
Less than or equal to: <=
4. Logical Operators

Combine boolean expressions.
Examples:
AND: && (e.g., if (isMember && hasPaid) { ... })
OR: || (e.g., if (age >= 18 || hasGuardian) { ... })
NOT: ! (e.g., if (!isValid) { ... })
5. Bitwise Operators

Perform operations on individual bits of integer values.
Examples:
AND: &
OR: |
XOR: ^
NOT: ~
Left shift: <<
Right shift: >>
6. Shift Operators

Shift bits of an integer value to the left or right.
Examples:
Left shift: << (e.g., result = value << 2)
Right shift: >> (e.g., result = value >> 3)
7. Unary Operators

Operate on a single operand.
Examples:
Increment: ++ (e.g., x++;, ++x;)
Decrement: -- (e.g., y--;, --y;)
Negation: - (e.g., -value)
Logical NOT: ! (e.g., !isAvailable)
Address-of: & (e.g., &x)
Dereference: * (e.g., *ptr)
8. Ternary Operator (?:)

A conditional expression that takes three operands.
Example: result = (condition) ? valueIfTrue : valueIfFalse;
9. Comma Operator (,)

Evaluates multiple expressions sequentially, returning the value of the last expression.
Example: x = (y = 3, y + 2); assigns 5 to x and 3 to y.


# Unit-2: Classes and objects

Encapsulation
Encapsulation is a process of combining data members and functions in a single unit called class. This is to prevent the access to the data directly, the access to them is provided through the functions of the class. It is one of the popular feature of Object Oriented Programming(OOPs) that helps in data hiding.

How Encapsulation is achieved in a class
To do this:
1) Make all the data members private.
2) Create public setter and getter functions for each data member in such a way that the set function set the value of data member and get function get the value of data member

information hiding
Information hiding or data hiding in programming is about protecting data or information from any inadvertent change throughout the program. Information hiding is a powerful OOP feature. Information hiding is closely associated with encapsulation.


Key Differences Between Data Hiding and Encapsulation
Encapsulation deals with hiding the complexity of a program. On the other hand, data hiding deals with the security of data in a program.
Encapsulation focuses on wrapping (encapsulating) the complex data in order to present a simpler view for the user. On the other hand, data hiding focuses on restricting the use of data, intending to assure the data security.
In encapsulation data can be public or private but, in data hiding, data must be private only.
Data hiding is a process as well as a technique whereas, encapsulation is subprocess in data hiding.


Abstract data types
An abstract data type (or ADT) is a class that has a defined set of operations and values. In other words, you can create the starter motor as an entire abstract data type, protecting all of the inner code from the user. When the user wants to start the car, they can just execute the start() function.

 In programming, an ADT has the following features:

An ADT doesn’t state how data is organized, and
It provides only what’s needed to execute its operations
An ADT is a prime example of how you can make full use of data abstraction and data hiding. This means that an abstract data type is a huge component of object-oriented programming methodologies: enforcing abstraction, allowing data hiding (protecting information from other parts of the program), and encapsulation (combining elements into a single unit, such as a class).

### state,identity,behaviour of an object
State: Represents data (value) of an object.

Behavior: Represents the behavior (functionality) of an object such as deposit, withdraw etc.

Identity: Object identity is typically implemented via a unique ID. The value of the ID is not visible to the external user. But,it is used internally by the JVM to identify each object uniquely.


# Unit 3 Inheritance and polymorphism

Inheritance
In C++, it is possible to inherit attributes and methods from one class to another. We group the “inheritance concept” into two categories:

derived class (child) – the class that inherits from another class
base class (parent) – the class being inherited from

class derived-class: access-specifier base-class

Access Control and Inheritance
A derived class can access all the non-private members of its base class. Thus base-class members that should not be accessible to the member functions of derived classes should be declared private in the base class.

We can summarize the different access types according to – who can access them in the following way −

![chart photo](https://bcastudyguide.files.wordpress.com/2020/07/img_20200730_092349.jpg)

A derived class inherits all base class methods with the following exceptions −

Constructors, destructors and copy constructors of the base class.
Overloaded operators of the base class.
The friend functions of the base class
We hardly use protected or privateinheritance, but public inheritance is commonly used. While using different type of inheritance, following rules are applied −

Public Inheritance − When deriving a class from a public base class, publicmembers of the base class become public members of the derived class and protected members of the base class become protected members of the derived class. A base class’s private members are never accessible directly from a derived class, but can be accessed through calls to the public and protectedmembers of the base class.
Protected Inheritance − When deriving from a protected base class, public and protected members of the base class become protectedmembers of the derived class.
Private Inheritance − When deriving from a private base class, public and protected members of the base class become private members of the derived class.

Types of Inheritance in C++
1) Single inheritance
2) Multilevel inheritance
3) Multiple inheritance
4) Hierarchical inheritance
5) Hybrid inheritance

1)Single inheritance
In Single inheritance one class inherits one class exactly.
For example: Lets say we have class A and B
- B inherits A

2) Multilevel Inheritance
In this type of inheritance one class inherits another child class.

3) Multiple Inheritance
In multiple inheritance, a class can inherit more than one class. This means that in this type of inheritance a single child class can have multiple parent classes.

C inherits A and B both

4)Hierarchical Inheritance
In this type of inheritance, one parent class has more than one child class. For example:

5) Hybrid Inheritance
Hybrid inheritance is a combination of more than one type of inheritance. For example, A child and parent class relationship that follows multiple and hierarchical inheritance both can be called hybrid inheritance.

Polymorphism in C++
Polymorphism is a feature of OOPSthat allows the object to behave differently in different conditions. In C++ we have two types of polymorphism:
1) Compile time Polymorphism – This is also known as static (or early) binding.
2) Runtime Polymorphism – This is also known as dynamic (or late) binding.

1) Compile time Polymorphism
Function overloading and Operator overloading are perfect example of Compile time polymorphism.

The easiest way to remember this rule is that the parameters should qualify any one or more of the following conditions, they should have different type, number or sequence of parameters.

int sum(int, int)
double sum(int, int)
	- This is not allowed as the parameter list is same. Even though they have different return types, its not valid.

Compile time Polymorphism Example
In this example, we have two functions with same name but different number of arguments. Based on how many parameters we pass during function call determines which function is to be called, this is why it is considered as an example of polymorphism because in different conditions the output is different. Since, the call is determined during compile time thats why it is called compile time polymorphism.

2) Runtime Polymorphism
Function overriding is an example of Runtime polymorphism.
Function Overriding: When child class declares a method, which is already present in the parent class then this is called function overriding, here child class overrides the parent class.

In case of function overriding we have two definitions of the same function, one is parent class and one in child class. The call to the function is determined at runtime to decide which definition of the function is to be called, thats the reason it is called runtime polymorphism.

Advantages of Function overloading
The main advantage of function overloading is to the improve the code readability and allows code reusability. In the example 1, we have seen how we were able to have more than one function for the same task(addition) with different parameters, this allowed us to add two integer numbers as well as three integer numbers, if we wanted we could have some more functions with same name and four or five arguments.
Imagine if we didn’t have function overloading, we either have the limitation to add only two integers or we had to write different name functions for the same task addition, this would reduce the code readability and reusability.

overloading and function overriding
Now that we understand what is function overloading and overriding in c++programming lets see the difference between them:

1) Function Overloading happens in the same class when we declare same functions with different arguments in the same class. Function Overriding is happens in the child class when child class overrides parent class function.
2) In function overloading function signature should be different for all the overloaded functions. In function overriding the signature of both the functions (overriding function and overridden function) should be same.
3) Overloading happens at the compile time thats why it is also known as compile time polymorphism while overriding happens at run time which is why it is known as run time polymorphism.
4) In function overloading we can have any number of overloaded functions. In function overriding we can have only one overriding function in the child class.

# Unit-4: Generic Function
Generics in C++
Generics is the idea to allow type (Integer, String, … etc and user-defined types) to be a parameter to methods, classes and interfaces. For example, classes like an array, map, etc, which can be used using generics very efficiently. We can use them for any type.

The method of Generic Programming is implemented to increase the efficiency of the code. Generic Programming enables the programmer to write a general algorithm which will work with all data types. It eliminates the need to create different algorithms if the data type is an integer, string or a character.

The advantages of Generic Programming are

Code Reusability
Avoid Function Overloading
Once written it can be used for multiple times and cases

Templates
Templates are powerful features of C++ which allows you to write generic programs. In simple terms, you can create a single function or a class to work with different data types using templates.

Templates are often used in larger codebase for the purpose of code reusability and flexibility of the programs.

The concept of templates can be used in two different ways:

Function Templates
Class Templates

Function Templates
A function template works in a similar to a normal function, with one key difference.

A single function template can work with different data types at once but, a single normal function can only work with one set of data types.

Normally, if you need to perform identical operations on two or more types of data, you use function overloading to create two functions with the required function declaration.

However, a better approach would be to use function templates because you can perform the same task writing less and maintainable code.

template <class T>
T someFunction(T arg)
{
   ... .. ...
}

How to declare a class template?
template <class T>
class className
{
   ... .. ...
public:
   T var;
   T someOperation(T arg);
   ... .. ...
};

How to create a class template object?

className<dataType> classObject;
className<int> classObject;
className<float> classObject;
className<string> classObject;

# Unit-5:File and Exception Handling

## File Handling using File Streams in C++
File represents storage medium for storing data or information. Streams refer to sequence of bytes. In Files we store data i.e. text or binary data permanently and use these data to read or write in the form of input output operations by transferring bytes of data. So we use the term File Streams/File handling. We use the header file <fstream>

- ofstream: It represents output Stream and this is used for writing in files.
- ifstream: It represents input Stream and this is used for reading from files.
- fstream: It represents both output Stream and input Stream. So it can read from files and write to files.

## Operations in File Handling:

- Creating a file: open()
- Reading data: read()
- Writing new data: write()
- Closing a file: close()
- Creating/Opening a File
- We create/open a file by specifying new path of the file and mode of operation. - Operations can be reading, writing, appending and truncating.

Syntax for file creation: 

- FilePointer.open("Path",ios::mode);

Example of file opened for writing:  st.open("E:\studytonight.txt",ios::out);


Example of file opened for reading:

```cpp
st.open(“E:\studytonight.txt”,ios::in)
```

Example of file opened for appending:

```cpp
st.open(“E:\studytonight.txt”,ios::app)
```

Example of file opened for truncating:

```cpp
st.open(“E:\studytonight.txt”,ios::trunc)
```

```cpp
#include<iostream.h> 
#include<conio.h> 
#include <fstream.h> 
using namespace std; 
int main() {

    fstream st; st.open("E\studytonight.txt",ios::out)

    if(!st){ 
        cout<<"File creation failed";
        } 
    else{ 
        cout<<"New file created"; st.close();
        } getch(); 
    
    return 0;

    }
```
### Writing to a File
include <iostream> 
include<conio> 
include <fstream> 
using namespace std; 
int main() { fstream st; st.open("E\studytonight.txt",ios::out); if(!st) { cout<<"File creation failed"; }

else

{

cout<<"New file created";

st<<"Hello";

st.close();

Closing file

}

getch(); return 0;

}

Here we are sending output to a file. So, we use ios::out. As given in the program, information typed inside the quotes after “FilePointer <<“ will be passed to output file.

Reading from a File

#include <iostream> #include<conio> #include <fstream> using namespace std; int main() { fstream st;

st.open("E\studytonight.txt",ios::in)

if(!st)

{ cout<<"No such file";

} else

{ char ch; while (!st.eof()) { st >>ch;

cout << ch;

}

st.close();

}

getch();

return 0;

}

Here we are reading input from a file. So, we use ios::in. As given in the program, information from the output file is obtained with the help of following syntax “FilePointer >>variable”.

Close a File
It is done by FilePointer.close().

#include <iostream> #include<conio>

#include <fstream>

using namespace std;

int main()

{ fstream st;

st.open("E\studytonight.txt",ios::out)

st.close()

getch();

return 0;

}

Special operations in a File
There are few important functions to be used with file streams like:

tellp() – It tells the current position of the put pointer. Syntax: filepointer.tellp()
tellg() – It tells the current position of the get pointer. Syntax: filepointer.tellg()
seekp() – It moves the put pointer to mentioned location. Syntax: filepointer.seekp(no of bytes,reference mode)
seekg() – It moves get pointer(input) to a specified location. Syntax: filepointer.seekg((no of bytes,reference point)
put() – It writes a single character to file.
get() – It reads a single character from file.
Note: For seekp and seekg three reference points are passed:
ios::beg – beginning of the file
ios::cur – current position in the file
ios::end – end of the file
