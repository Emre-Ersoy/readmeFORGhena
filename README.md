1. **Comparing Paradigms**

   **Question**: Compare and contrast the imperative programming paradigm with the functional programming paradigm. Mention how variables and data structures are handled, and give examples of programming languages that primarily follow each paradigm.

   **Answer**: In the imperative programming paradigm, programs are made up of a series of statements that change a program's state. In this paradigm, variables are used to store data, and values in these variables can be changed over time. Common data structures in imperative programming include arrays, records, and loops, which are used to execute a sequence of statements repeatedly. Example languages include C, C++, and Java.
   
   On the other hand, in functional programming, programs are constructed by applying and composing functions. Variables in functional programming are often immutable, meaning that once a value is assigned, it cannot be changed. Instead of loops, functional programming often relies on recursion to repeat operations. Example data structures include lists and tuples. Example languages include Haskell, Lisp, and Erlang.

2. **Programming Language History**

   **Question**: Explain the historical significance of the FORTRAN programming language. How did it contribute to the development of modern programming languages?

   **Answer**: FORTRAN, which stands for Formula Translation, was developed in the 1950s and is considered one of the first high-level programming languages. It allowed scientists and engineers to write programs in a syntax that was more similar to mathematical notation than machine code, significantly reducing the effort required to write and maintain programs. Its development marked the beginning of high-level programming languages and it influenced many subsequent languages such as Algol, BASIC, and PL/I.

3. **Code Writing: Functional Programming**

   **Question**: Write a Haskell function that takes a list of integers and returns a list containing only the even numbers from the input list. For example, given `[1, 2, 3, 4, 5]`, the function should return `[2, 4]`.

   **Answer**:
   ```haskell
   filterEven :: [Int] -> [Int]
   filterEven xs = filter even xs
   ```

4. **Programming Paradigms: Logical**

   **Question**: Explain the basic concepts of logical programming. Name a programming language that is predominantly used for logical programming and give an example of its application.

   **Answer**: Logical programming is a programming paradigm in which programs are written as a set of logical rules and facts. These rules and facts are used by the language's inference engine to answer queries. Prolog is an example of a logical programming language. An application of logical programming is creating expert systems, where the system can make deductions and answer queries based on a knowledge base of facts and rules.

5. **Asynchronous Programming**

   **Question**: What is asynchronous programming, and why is it important? Give an example of a programming language that supports asynchronous programming and describe a use case.

   **Answer**: Asynchronous programming is a programming paradigm where the execution of certain operations can occur outside the main program flow, allowing the program to perform other tasks while waiting for asynchronous operations to complete. This is particularly useful in situations like making network requests, reading files, or any other operations that are time-consuming and don’t need the program to be stalled. JavaScript is an example of a language that supports asynchronous programming through callbacks, promises, and async/await. A common use case is in web development where you might need to fetch data from an API; using asynchronous programming allows the webpage to remain responsive while the data is being fetched.

6. **Language Feature: Python List Comprehension**

   **Question**: Explain the concept of list comprehensions in Python and provide an example code that

 utilizes this feature.

   **Answer**: List comprehension is a concise way to create lists in Python. It can be used to create a new list by performing an operation on each item in an existing list or other iterable. Syntax: `[expression for item in iterable if condition]`. 

   Example code that squares each item in a list:
   ```python
   original_list = [1, 2, 3, 4, 5]
   squared_list = [x ** 2 for x in original_list]
   print(squared_list)  # Output: [1, 4, 9, 16, 25]
   ```

7. **Comment on Kotlin's Null Safety**

   **Question**: What is Kotlin’s approach to null safety, and how does it differ from Java's approach? Explain the benefits of Kotlin's approach.

   **Answer**: Kotlin uses nullable types to handle null safety. In Kotlin, you must explicitly specify if a variable can be null by using the `?` operator. This makes null errors more predictable and easier to debug. In contrast, Java allows any variable to be null, which can lead to unexpected Null Pointer Exceptions. Kotlin’s approach benefits developers by enforcing null safety at compile time, reducing runtime errors and increasing code reliability. Additionally, Kotlin provides a set of operators like the Elvis operator `?:` and the safe call operator `?.` to handle null values gracefully.

8. **Concurrency vs. Parallelism**

   **Question**: Distinguish between concurrency and parallelism in programming. Provide an example where one might be more suitable than the other.

   **Answer**: Concurrency is a concept where several tasks are executed in overlapping time frames. It doesn’t necessarily mean that they’re executed at the exact same time; rather, it can be that the tasks are broken down into subtasks and executed in an interleaved manner. On the other hand, parallelism is when multiple tasks are executed at the same time, often by utilizing multiple processors or cores.

   For example, in a web server handling multiple incoming requests, concurrency might be more suitable as it can efficiently handle multiple clients by interleaving the processing of requests. However, for tasks like image processing where an image is broken into multiple segments and each segment is processed independently, parallelism would be more suitable as it would make use of multiple cores and do the processing faster.
9. **Programming Paradigms: Object-Oriented Programming**

   **Question**: What are the four fundamental principles of Object-Oriented Programming (OOP)? Describe each briefly and provide an example language that employs this paradigm.

   **Answer**: The four fundamental principles of Object-Oriented Programming are Encapsulation, Inheritance, Polymorphism, and Abstraction.
   
   - **Encapsulation**: It involves bundling the data (attributes) and the methods (functions) that operate on the data into a single unit called a class. An object is an instance of a class. Encapsulation also includes the concept of data hiding, meaning that the internal state of an object is protected from outside interference.
   
   - **Inheritance**: It is a mechanism where a new class can inherit properties and behavior (methods) of an existing class. This is used to represent a “is-a” relationship and promotes code reusability.
   
   - **Polymorphism**: This principle allows one interface to be used for different data types. For example, the ability to use the same method name for methods in different classes (through method overriding or overloading).
   
   - **Abstraction**: It involves hiding complex implementation details and showing only the essential features of the object. This helps in reducing complexity and allows the programmer to focus on interactions at a higher level.
   
   Example languages that employ the OOP paradigm include Java, C++, Python, and Ruby.

10. **Static vs. Dynamic Typing**

    **Question**: What is the difference between static typing and dynamic typing in programming languages? Provide an example of a statically-typed language and a dynamically-typed language.

    **Answer**: In static typing, the type of a variable is known at compile time. For some languages, this means that you have to explicitly specify the type of the variable at the time of declaration. Examples of statically-typed languages include Java, C, and C++.
   
    In dynamic typing, the type of a variable is determined at runtime. This means that you don't have to specify the type of the variable when you declare it, and you can assign different types to the same variable. Examples of dynamically-typed languages include Python, Ruby, and JavaScript.

11. **Code Writing: Recursion in Scheme**

    **Question**: Write a Scheme function that computes the factorial of a non-negative integer `n`. The factorial function can be defined as `factorial(n) = n * factorial(n-1)` for `n > 0`, and `factorial(0) = 1`.

    **Answer**:
    ```scheme
    (define (factorial n)
      (if (<= n 1)
          1
          (* n (factorial (- n 1)))))
    ```

12. **Functional Programming: Pure Functions**

    **Question**: What is a pure function in the context of functional programming? Describe its properties and explain how it contributes to the reliability and maintainability of the code.

    **Answer**: A pure function is a function that has the following properties:
    - Its return value is only determined by its input values, without observable side effects.
    - It always produces the same output for the same set of inputs.
    - It does not alter any external state or data.

    Pure functions contribute to the reliability and maintainability of the code by making it more predictable and easier to test. Since pure functions do not have side effects and only depend on their input, they can be more easily reasoned about and debugged.

13. **Dart and Asynchronous Programming**

    **Question**: Explain how Dart supports asynchronous programming. Provide an example use case where asynchronous programming in Dart would be beneficial.

    **Answer**: Dart supports asynchronous programming through

 the use of `Future`s, `async` and `await` keywords. A `Future` represents a computation that doesn't complete immediately. With the `async` keyword, you can define asynchronous functions, and you can use the `await` keyword within an `async` function to pause the execution of the function until an asynchronous operation completes.
    
    Example use case: In a mobile app developed with Flutter (which uses Dart), you might want to fetch data from an API and display it to the user. By using asynchronous programming, you can make the network request without freezing the UI, providing a better user experience.

14. **Metaprogramming in Ruby**

    **Question**: What is metaprogramming, and how is it supported in Ruby? Provide a brief example code snippet.

    **Answer**: Metaprogramming is a programming technique in which code can manipulate other code, such as methods or classes, at runtime. This allows for more dynamic and flexible code. Ruby supports metaprogramming through various features like dynamic method creation, method_missing, and class macros.
    
    Example code snippet in Ruby:
    ```ruby
    class Dog
      def initialize(name)
        @name = name
      end

      ["bark", "fetch", "wag_tail"].each do |action|
        define_method(action) do
          puts "#{@name} is #{action}ing!"
        end
      end
    end

    dog = Dog.new("Fido")
    dog.bark # Output: "Fido is barking!"
    dog.fetch # Output: "Fido is fetching!"
    ```

15. **Language Interoperability: C# and F#**

    **Question**: Explain what is meant by language interoperability and provide an example of how C# can interoperate with F# within the .NET framework.

    **Answer**: Language interoperability refers to the ability of code written in one programming language to interact with code written in another language. This is often facilitated by using a common runtime environment or standard.

    In the context of the .NET framework, both C# and F# are compiled to Common Intermediate Language (CIL), which allows them to interoperate. For example, you can define a class in F# and use it within a C# project, or vice versa.

    Example:
    - Define a simple F# library:
    ```fsharp
    // MathLib.fs
    namespace MathLib
    
    module MathFunctions =
        let square x = x * x
    ```
    - Use the F# library in a C# program:
    ```csharp
    // Program.cs
    using MathLib;

    class Program
    {
        static void Main()
        {
            int result = MathFunctions.square(4);
            Console.WriteLine(result);  // Output: 16
        }
    }
    ```
16. **History of Programming Languages**

    **Question**: Compare Fortran and Pascal as historical programming languages. Discuss their primary purposes, syntax, and historical significance.

    **Answer**: 
    - **Fortran**: Developed in the 1950s by IBM, Fortran (short for "Formula Translation") was primarily designed for scientific and engineering applications. It was one of the first high-level programming languages and introduced concepts such as loops and conditionals. It has a simple syntax focused on mathematical expressions and has been known for its performance in numerical computation. Fortran played a significant role in the early development of computer science and is still in use in scientific computing.
    
    - **Pascal**: Developed in the late 1960s and early 1970s by Niklaus Wirth, Pascal was designed as a teaching language to encourage good programming practices. Its syntax is more structured and readable compared to Fortran. Pascal was used widely in education and for some business applications during the 1980s. It introduced structured programming concepts and was instrumental in the development of the Modula and Ada programming languages.

17. **Dynamic vs. Static Scoping**

    **Question**: Explain the difference between dynamic scoping and static (lexical) scoping in programming languages. Provide an example of a programming language that uses dynamic scoping and one that uses static scoping.

    **Answer**: 
    - **Dynamic scoping**: Under dynamic scoping, a variable is resolved by looking up the call stack and finding the most recent instance of that variable. This means the value of the variable can change depending on where the function is called. An example of a language that has an option for dynamic scoping is Emacs Lisp.

    - **Static (lexical) scoping**: Under static scoping, the value of a variable is determined by the structure of the code, and it is resolved to the nearest enclosing block where it is declared. This makes the code easier to reason about because the value of the variable does not change depending on where the function is called. Most modern programming languages, including C, Java, and Python, use static scoping.

18. **Type Inference in Haskell and Java**

    **Question**: Compare the type inference mechanisms in Haskell and Java. How do these mechanisms help in writing programs, and what are their limitations?

    **Answer**: 
    - **Haskell**: Haskell has a very strong type inference mechanism. Almost all types can be inferred by the compiler. Haskell's type system is also very strict, meaning that type errors are caught early, often at compile-time. This can lead to safer code but sometimes makes writing certain types of programs more complex due to the need to satisfy the type system.

    - **Java**: Prior to Java 8, Java had very limited type inference, typically requiring programmers to explicitly declare the types of their variables. However, starting from Java 10, Java introduced a limited type inference with the `var` keyword, allowing the programmer to omit the type of a local variable. Java's type inference is still not as powerful as Haskell's, but it helps reduce verbosity in the code. Java’s type inference is mainly a convenience for writing code, while Haskell's is fundamental to the way programs are constructed.

19. **Garbage Collection in Python and C++**

    **Question**: Discuss how garbage collection is handled in Python and C++. Explain the benefits and drawbacks of each approach.

    **Answer**:
    - **Python**: Python uses automatic garbage collection. The primary mechanism is reference counting, where each object has a count of references to it, and when this count drops to zero, the memory is deallocated. It also has a cyclic garbage collector to catch reference cycles. The benefit of this approach is that the programmer doesn't need to explicitly manage memory, which reduces the likelihood of memory leaks. The drawback is that garbage collection can cause performance overhead at runtime.
    
    - **C++**: C++ uses manual memory management, where the programmer is responsible for allocating and deallocating memory through the `new` and `delete` operators. C++ also supports RAII (Resource Acquisition Is Initialization) principle, where resources are tied to object lifetime (scoped resource management). The benefit of manual memory management is that it can be more efficient since there is no garbage collector running in the background. The drawback is that it's easier to make mistakes, like memory leaks or accessing freed memory, which can lead to bugs and security vulnerabilities.

20. **Functional vs. Object-Oriented Programming**

    **Question**: Compare functional programming (e.g., in Haskell) with object-oriented programming (e.g., in Java). Discuss how data and functions are handled in each paradigm, and provide examples of typical use cases for each.

    **Answer**: 
    - **Functional Programming (Haskell)**: In functional programming, functions are first-class citizens, and data is immutable. Functions can be passed as arguments to other functions, and there is a heavy emphasis on recursion for iteration. Functional programming is often used for mathematical computations, data analysis, and where immutability is required for reliability and clarity.
    
    - **Object-Oriented Programming (Java)**: In OOP, data and methods that operate on that data are encapsulated into objects. There is a heavy emphasis on the interaction between these objects. OOP is widely used in large-scale software systems, GUI applications, and systems where the state is important and must be managed over time.
