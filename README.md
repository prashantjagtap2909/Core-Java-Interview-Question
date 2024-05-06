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
 
 ### Static

1.  ####   What is static?
   - In Java, static refers to a member (field, method, or nested class) that belongs to the class itself, rather than to an instance of the class. There is only one copy of a static member shared by all objects of the class.

2.  ####   Can we make local variables static? Why or why not?
   - No, we cannot declare local variables as static in Java. Local variables are specific to a particular method invocation and go out of scope when the method finishes executing. Static members, on the other hand, are associated with the class itself and exist throughout the lifetime of the program.

3.  ####   Can we call non-static functions from a static function? Why or why not?
   - Yes, we can call non-static methods from a static method in Java. Even though a static method cannot access non-static members directly, it can create an object of the class and call the non-static method on that object.

4.  ####   Why is the main method static?
   - The main method is declared as static in Java because it is the entry point of the program. The JVM looks for the main method to start executing the program. Since the main method is static, it can be called without creating an instance of the class that contains it.

5.  ####   When do we use static variables? Can you explain with an example?
   - Static variables are used to store data that is shared by all instances of a class. For example, you might use a static variable to count the number of objects that have been created from a class. Here's an example:

    public class Counter {
      private static int count = 0;
    
      public Counter() {
        count++;
      }
    
      public static int getCount() {
        return count;
      }
    }

In this example, the count variable is static. Every time a new Counter object is created, the count variable is incremented. The getCount method can be used to retrieve the current value of the count.

 **[⬆ Back to Top](#table-of-contents)**  
 
5. ### Constructor

1.  ####   What is a constructor?
   - In Java, a constructor is a special method that is called when an object of a class is created. It is used to initialize the object's state (set the values of its fields).

2.  ####   Can we make our constructor private? Why or why not?
   - Yes, we can make a constructor private in Java. This means that the constructor can only be called from within the class itself. This can be useful for ensuring that objects are always created in a valid state. However, it also means that you cannot create objects of the class from other classes.

3.  ####   Can we make our constructor static? Why or why not?
   - No, we cannot make a constructor static in Java. Constructors are used to initialize objects, and static methods cannot access non-static members of the class. Additionally, static methods are called without creating an instance of the class, and constructors are used to create instances of the class.

4.  ####   What is the use of a constructor?
   - Constructors have several uses, including:
Initializing object fields with default values
Performing validation checks on input parameters
Allocating resources for the object
Chaining constructors together (calling one constructor from another

5.  ####   Why does a constructor not inherit?
   - Constructors are not inherited by subclasses in Java. This is because constructors are used to initialize objects of a specific class, and the initialization requirements for a subclass may be different from those of its superclass.

6.  ####   What is constructor overloading? Explain with an example.
   - Constructor overloading is a technique of creating multiple constructors in a class that have different parameter lists. This allows you to create objects of the class in different ways, depending on the data you have available.
For example, here is a class Person with two overloaded constructors:


         public class Person {
           private String name;
           private int age;
         
           public Person(String name) {
             this.name = name;
           }
         
           public Person(String name, int age) {
             this.name = name;
             this.age = age;
           }
         }

In this example, the first constructor takes a single parameter for the name, and the second constructor takes two parameters for the name and age. You can use either constructor to create a Person object, depending on whether you have the person's age or not.

 **[⬆ Back to Top](#table-of-contents)**  

6. ### Encapsulation

1.  ####   What is Encapsulation?
   - Encapsulation is a fundamental concept in object-oriented programming (OOP) that refers to the bundling of data (fields) and methods that operate on that data together within a single unit, typically a class in Java.

2.  ####   How to Achieve Encapsulation?

   - Encapsulation is achieved by declaring the class's variables as private. This means that they can only be accessed directly by the methods within the class. To access or modify the private variables, you can use public getter and setter methods.

3.  ####   What is the Role of Private in Encapsulation?

   - The private keyword is a key mechanism to achieve encapsulation in Java. By declaring class members (fields, methods) as private, you restrict their direct access from outside the class. This promotes data hiding and prevents external code from accidentally modifying the data in an unexpected way.

4.  ####   Why is Encapsulation Required?

   - Encapsulation offers several benefits, including:
Data hiding: Protects data from unauthorized access and modification.
Data integrity: Ensures that data is only modified through well-defined methods, reducing the risk of errors.
Modular design: Promotes modularity by keeping the internal implementation details of a class hidden from external code.
Improved maintainability: Makes code easier to maintain by allowing you to change the implementation details of a class without affecting other parts of your program.

5.  ####   Have you done encapsulation in your project?
   - Encapsulation is a best practice in object-oriented programming, and we have used it in projects where the code involves classes.

 **[⬆ Back to Top](#table-of-contents)**  

7. ### Polymorphism
8. ### Abstraction
9. ### Inheritance
10. ### Multithreading
11. ### Exception Handling
