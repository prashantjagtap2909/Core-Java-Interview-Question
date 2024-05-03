# Core-Java-Interview-Question  [![Views](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fprashantjagtap2909%2FBreadcrumbsCore-Java-Interview-Question&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Views&edge_flat=false)](https://hits.seeyoufarm.com)

### Table of Contents

| No. | Topics                                                                                                                             |
| --- | ---------------------------------------------------------------------------------------------------------------------------------- |
| 1   | [JDK, JRE and JIT](#JDK-JRE_JIT)                                                                                                   |
| 2   | [Basics of Java](#Basics-of-Java)                                                                                                  |
| 3   | [Package and Import](#Package-and-Import)                                                                                          |
| 4   | [Static](#Static)                                                                                                                  |
| 5   | [Constructor](#Constructor)                                                                                                        |
| 6   | [Encapsulation](#Encapsulation)                                                                                                    |
| 7   | [Polymorphism](#Polymorphism)                                                                                                      |
| 8   | [Abstraction](#Abstraction)                                                                                                        |
| 9   | [Inheritance](#Inheritance)                                                                                                        |
| 10  | [Multithreading](#Multithreading)                                                                                                  |
| 11  | [Exception Handling](#Exception-Handling)                                                                                          |



 ### JDK, JRE and JIT
  1.  ####  What's the difference between a JDK and a JRE?

   - JDK (Java Development Kit): Provides the tools for building Java applications, including the JRE, compilers, debuggers, and other development utilities.
    
   - JRE (Java Runtime Environment): Provides the basic environment to run Java programs. It includes the JVM and core Java class libraries.

  2.  ####  What is the role of JIT (Just-In-Time Compiler) in Java?

   - The JIT compiler is part of the JVM. It takes bytecode (the intermediate language Java programs are compiled into) and translates it into machine code specific to your computer's               processor for faster execution.

 3.  #### How is a compiler different from an interpreter?

   - Compiler: Translates source code (human-readable code like Java) into machine code all at once before the program runs. Machine code is specific to the processor and runs directly.
    
   - Interpreter: Translates source code into machine code line by line as the program executes. No need to generate all the code upfront, but it can be slower than a compiler.

 4.  ####  What does the JVM (Java Virtual Machine) do?

   - The JVM is a program that executes bytecode. Bytecode is not specific to any computer architecture, allowing Java programs to run on any machine with a JVM. The JVM translates bytecode into   machine code specific to your processor at runtime.

5.  ####  What's the difference between source code and bytecode?

   - Source code: Human-readable code written in a programming language like Java.
    
   - Bytecode: An intermediate language generated from source code by a Java compiler. Bytecode allows Java programs to run on any computer with a JVM because it's not specific to a particular architecture.


 **[⬆ Back to Top](#table-of-contents)**


 ### Basics of Java
 1.  ####  What is a class??
   - In Java, a class is a blueprint that defines the properties and methods of an object. We can use a class to create objects that share the same properties and behaviors.

 2.  ####  What are variables and the different types of variables?
   - In Java, a variable is a named storage location that holds data. There are different types of variables, such as primitive data types (int, float, char, etc.) and reference data types (objects, arrays, etc.).

3.  #### Why do we need custom variables and what are the benefits of using them?
   - Custom variables allow us to store data specific to our program's needs. They are beneficial because they can improve code readability, maintainability, and reusability.

4.  ####  How do you decide when to use a global variable and when to use a local variable?
   - Global variables are accessible throughout your entire program, while local variables are only accessible within the block of code where they are declared. You should use local variables whenever possible to avoid naming conflicts and unintended side effects. Use global variables sparingly, and only when data needs to be accessed by multiple parts of your program.

5.  ####  What is a method?
   - In Java, a method is a block of code that performs a specific task. Methods can take parameters and return values.

6.  ####  What is the purpose of the return statement in Java?
   - The return statement is used to return a value from a method. A method can optionally return a value using the return keyword followed by the value to be returned.

7.  ####  What is the use of the 'new' keyword in Java?
   - The new keyword is used to create a new object from a class. When you use the new keyword, memory is allocated for the object, and the object's constructor is called.

8.  ####  What is a runtime error? Can you explain with an example?
   - A runtime error is an error that occurs while a program is running. Runtime errors are typically caused by mistakes in the program's logic, such as trying to divide by zero or accessing an array element out of bounds.

9.  ####  How can you differentiate between a compile-time error and a runtime error?
   - Compile-time errors are errors that are detected by the compiler before the program can even run. Syntax errors and type mismatches are examples of compile-time errors. Runtime errors, on the other hand, occur while the program is running.

10.  ####  What is the difference between Heap and Stack memory?
   - The heap and stack are two different memory areas used in Java programs. The heap is used to store dynamically allocated objects, while the stack is used to store method calls and local variables.

11.  ####  What are the features of Java that you know?
   - Java has many features that make it a popular programming language, including object-oriented programming, platform independence, automatic memory management, and security.

 **[⬆ Back to Top](#table-of-contents)**     
 
 ### Package and Import
 
1.  ####  What is a package?
   - In Java, a package is a hierarchical namespace that groups related classes, interfaces, and sub-packages together. They help organize code, prevent naming conflicts, and improve code maintainability.

2.  ####  What are the benefits of using packages?
   - Packages provide several benefits, including:
Organization: Packages help to organize your code by grouping related classes together. This can make your code easier to understand and maintain.
Naming conflicts: Packages help to prevent naming conflicts between classes from different parts of your program.
Access protection: Packages can be used to control access to classes and interfaces. By default, classes in the same package can access each other's private and protected members, while classes in different packages cannot.
Reusability: Packages can be reused in other projects.

3.  ####  Why do we import classes or packages?
   - We import classes or packages to use them in our code. When you import a class, you can use the class name without having to specify its fully qualified name (including the package name).

4.  ####  Can we import an entire package? Why or why not?
   - Yes, you can import an entire package using the import packageName.* syntax. This will import all of the classes and interfaces in the package. However, it is generally not recommended to import entire packages because it can lead to naming conflicts. It is better to import only the classes that you need.

5.  ####  What are company standards for creating packages?
Company standards for creating packages can vary. Here are some general guidelines:
Use a reverse domain name structure for your package names (e.g., com.mycompany.myapp).
Keep your packages relatively small and focused.
Name your packages clearly and descriptively.

6.  ####  What package structure did you create in your project?
   - The specific package structure will vary depending on the project. Here are some common elements that you might find in a Java package structure:
A com.company.myapp package for your main application code.
A com.company.myapp.util package for utility classes.
A com.company.myapp.data package for data access classes.
A com.company.myapp.ui package for user interface classes.

 **[⬆ Back to Top](#table-of-contents)**  
 
4. ### Static
5. ### Constructor
6. ### Encapsulation
7. ### Polymorphism
8. ### Abstraction
9. ### Inheritance
10. ### Multithreading
11. ### Exception Handling
