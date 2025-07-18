<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" class="logo" width="120"/>

# 100 OOPs Interview Questions with Detailed Answers

## Basic Concepts

### 1. What is Object-Oriented Programming (OOP)?

Object-Oriented Programming (OOP) is a  programming paradigm based on the concept of “objects,” which can contain data (fields, attributes) and code (methods, procedures) to manipulate that data. OOP focuses on four main principles: encapsulation, inheritance, polymorphism, and abstraction[^1][^2].

### 2. What are the main objectives of OOP?

- To increase code reuse through inheritance.
- To enhance code maintainability via encapsulation.
- To enable code flexibility and scalability through polymorphism and abstraction[^2].


### 3. What are the four pillars of OOP?

- **Encapsulation**
- **Inheritance**
- **Polymorphism**
- **Abstraction**[^3][^1]


### 4. What is a class?

A class is a blueprint or template for creating objects. It defines a set of attributes and behaviors (methods) that the created objects (instances) will have[^4][^2].

### 5. What is an object?

An object is an instance of a class. It contains real values instead of variables and represents a specific entity with a state and behavior defined by its class[^4][^2].

### 6. What is encapsulation?

Encapsulation is the mechanism of binding data and methods that operate on that data together in a single unit, restricting direct access to some of the object's components and protecting the object's integrity by preventing outsiders from setting the data into inconsistent or invalid states. Achieved via access modifiers like private, protected, and public[^3][^2].

### 7. What is abstraction?

Abstraction is the concept of exposing only the necessary features of an object to the outside world, while hiding internal details that are irrelevant for the user of the object. Abstraction is usually achieved using abstract classes and interfaces[^3][^2].

### 8. What is inheritance?

Inheritance is an OOP principle where a class (child or derived class) acquires properties and behaviors of another class (parent or base class). It promotes code reuse and establishes a parent-child relationship[^3][^2].

### 9. What is polymorphism?

Polymorphism is the ability of a single function, method, or operator to operate in different ways depending on the context, usually by redefining or overloading methods in derived classes[^3][^2].

### 10. What is the difference between a class and an object?

- A class defines the structure and behavior.
- An object is a specific instance of a class[^4][^5].


## Classes and Objects

### 11. Explain the terms: attribute, method, and constructor.

- **Attribute**: A variable within a class representing the state.
- **Method**: A function defined in a class representing behavior.
- **Constructor**: A special method invoked during object creation to initialize the object[^4][^5].


### 12. What is the purpose of a constructor?

A constructor initializes the state of an object when it is created. In most languages, it has the same name as the class[^5].

### 13. What is a destructor?

A destructor is a method called when an object is destroyed or deallocated. It is used to perform cleanup[^5][^6].

### 14. How are objects created from a class?

Objects are created by instantiating a class using the `new` keyword or a similar mechanism provided by the language[^4][^5].

### 15. Can you overload constructors?

Yes, most OOP languages allow constructor overloading, i.e., defining multiple constructors with different sets of parameters[^5].

## Inheritance

### 16. What are the different types of inheritance?

- **Single Inheritance:** One subclass inherits from one superclass.
- **Multiple Inheritance:** One subclass inherits from multiple superclasses (not supported in all languages).
- **Multilevel Inheritance:** A subclass acts as a superclass for another subclass.
- **Hierarchical Inheritance:** Multiple subclasses inherit from a single superclass.
- **Hybrid Inheritance:** A combination of more than one type of inheritance[^5].


### 17. How is code reusability achieved through inheritance?

By allowing a new class to use methods and attributes of an existing class without rewriting code[^4][^2].

### 18. What is the difference between `super` and `this` keywords?

- `super` refers to the superclass and is used to access parent class methods or constructors.
- `this` refers to the current instance of the class[^2].


### 19. Give a real-life example of inheritance.

A `Vehicle` class could be a base class, while `Car`, `Bike`, and `Truck` classes inherit from `Vehicle` and have their own specific properties and methods[^2].

### 20. What is method overriding?

Method overriding is redefining a superclass method in the child class with the same name and signature, allowing runtime polymorphism[^3][^2].

## Polymorphism

### 21. What are the two types of polymorphism?

- **Compile-time (Static) Polymorphism**: Achieved through method overloading and operator overloading.
- **Runtime (Dynamic) Polymorphism**: Achieved through method overriding[^7][^2].


### 22. What is method overloading?

Method overloading is defining multiple methods in a class with the same name but different parameter lists[^7][^2].

### 23. What is method overriding, and how is it different from overloading?

- **Overriding**: Change behavior of inherited method in derived class; occurs at runtime.
- **Overloading**: Multiple methods with same name but different parameters; occurs at compile-time[^7][^2].


### 24. How is polymorphism achieved in OOP?

By method overloading (static) and method overriding (dynamic)[^3][^2].

### 25. Provide an example of runtime polymorphism.

Overriding a `draw()` method in a base `Shape` class by child classes `Circle`, `Rectangle`, etc. Each class has its own implementation of `draw()`[^8].

## Abstraction and Encapsulation

### 26. How is data abstraction achieved?

By using abstract classes and interfaces that provide a template without exposing the complete implementation[^7][^2].

### 27. What is the difference between encapsulation and abstraction?

- **Encapsulation**: Hides the internal state and binds data and methods.
- **Abstraction**: Hides complexity by showing only the necessary details[^2].


### 28. How do access modifiers support encapsulation?

By controlling the visibility of attributes and methods to the outside world (e.g., `private`, `protected`, `public` in Java/C++)[^3].

### 29. What is data hiding, and how is it related to encapsulation?

Data hiding restricts direct access to some components of an object, which is achieved through encapsulation using private/protected members[^3][^2].

### 30. Why is encapsulation important in OOP?

It secures data, promotes code modularity, maintenance, and flexibility[^3][^2].

## Advanced Concepts

### 31. What is an abstract class?

A class that cannot be instantiated and may contain one or more abstract methods that must be implemented by subclasses[^2].

### 32. What is an interface?

An interface only declares method signatures without providing their implementations. Classes implement interfaces to agree on certain behaviors[^5].

### 33. What is the difference between abstract classes and interfaces?

- Abstract classes can have implemented methods; interfaces cannot (prior to Java 8).
- A class can implement multiple interfaces but usually extend only one abstract class[^5].


### 34. Can a class implement multiple interfaces?

Yes, a class can implement multiple interfaces, enabling multiple inheritance of type[^5].

### 35. What is multiple inheritance? Is it supported in all programming languages?

Multiple inheritance is when a class derives from more than one base class. Not all languages support this (e.g., Java avoids ambiguity through interfaces)[^2].

### 36. What is hybrid inheritance?

Hybrid inheritance is a combination of two or more types of inheritance[^5].

### 37. What is a virtual function?

A function declared in the base class and overridden by derived class. Used for achieving runtime polymorphism[^2].

### 38. What is the difference between composition and inheritance?

- **Inheritance**: Expresses an “is-a” relationship.
- **Composition**: Expresses a “has-a” relationship, where a class contains objects of other classes[^2].


### 39. What is a copy constructor?

A constructor that initializes a new object as a copy of an existing object[^5].

### 40. What is operator overloading?

Operator overloading means defining new behavior for existing operators based on operand types[^2][^5].

## Practical \& Coding

### 41. How would you implement a real-time system using OOP?

Break the system into objects and classes mapping real-world entities and their behaviors; use principles like encapsulation, abstraction, inheritance, and polymorphism to model and achieve functionality[^4].

### 42. How do you achieve code reusability in OOP?

Through inheritance, composition, and implementation of interfaces[^4].

### 43. What is a static member?

A static member belongs to the class rather than any specific instance, so it is shared across all instances[^2].

### 44. What is a final class?

A final class cannot be extended/inherited by other classes (Java)[^2].

### 45. What is a pure virtual function?

A function declared in an abstract base class and meant to be overridden in derived classes. It has no implementation in the base class (C++)[^2].

### 46. Explain the SOLID principles.

- **Single Responsibility Principle**: Each class should have only one purpose.
- **Open/Closed Principle**: Software entities should be open for extension but closed for modification.
- **Liskov Substitution Principle**: Subtypes should be substitutable for their base types.
- **Interface Segregation Principle**: Many specific interfaces are better than one general-purpose interface.
- **Dependency Inversion Principle**: Depend upon abstractions, not concretions[^8].


### 47. What is the role of the `super` keyword?

`super` keyword is used to call parent class constructors/methods from a child class[^2].

### 48. What is the difference between aggregation and composition?

- **Aggregation**: A “has-a” relationship where the existence of child does not depend on parent.
- **Composition**: Stronger relation; if parent is destroyed, child is destroyed too[^5].


### 49. Can you access a private attribute of a class directly from outside the class?

No, private members can only be accessed within the same class. Access from outside requires getter/setter methods[^3][^2].

### 50. What is dynamic binding?

Process whereby the code to be executed is determined at runtime, especially for overridden methods[^7][^2].

## Constructors \& Destructors

### 51. What is a default constructor?

A default constructor takes no parameters and is provided by default unless another constructor is defined[^5].

### 52. What is a parameterized constructor?

A constructor that takes arguments[^5].

### 53. What is a copy constructor?

A constructor used to create a new object as a copy of an existing object[^5].

### 54. Can constructors be overloaded?

Yes, constructors can be overloaded by varying parameter lists[^5].

### 55. What is a destructor, and when is it called?

A destructor is a special method invoked when an object is about to be destroyed, used for cleanup[^5][^6].

## Access Modifiers

### 56. What are access modifiers?

Keywords that define the access scope of class members (e.g., private, protected, public)[^3][^2].

### 57. What is the difference between public, private, and protected access?

- **Public**: Accessible everywhere.
- **Private**: Accessible only within the class.
- **Protected**: Accessible within the class and its subclasses[^3][^2].


### 58. Can you change the access modifier of an overridden method?

Yes, but the new modifier cannot reduce the accessibility from the original[^5].

### 59. Why is data hiding important?

It restricts exposure of internal data, making implementation details invisible and only allowing controlled access[^3][^2].

### 60. How is data hiding achieved in OOP?

By using private and protected access modifiers[^3].

## Advanced Questions

### 61. How do abstract classes differ from concrete classes?

- **Abstract classes**: May have unimplemented (abstract) methods; cannot be instantiated.
- **Concrete classes**: All methods implemented; can be instantiated[^2].


### 62. What is an interface segregation principle?

The idea that clients should not be forced to depend on interfaces they do not use; each interface should have a specific responsibility[^8].

### 63. What are design patterns?

Standard solutions to common software design problems in OOP, such as Singleton, Factory, Observer, and Strategy patterns[^8].

### 64. Explain the Singleton pattern.

Ensures a class has only one instance and provides a global point of access to it[^8].

### 65. What is the “diamond problem”? How is it solved?

It occurs in multiple inheritance when a class inherits from two classes which both inherit from a common base class, causing ambiguity. Solved by virtual inheritance or using interfaces (e.g., Java avoids by not allowing multiple inheritance)[^5].

### 66. What is duck typing?

A concept where the type or class of an object is determined by its behavior or methods, rather than its inheritance or implementation[^1].

### 67. What is object slicing?

Occurs in languages like C++ when an object of a derived class is assigned to a variable of a base class type, slicing off derived class-specific information[^5].

### 68. What is a friend function?

In C++, a friend function is given access to private and protected members of a class, even though it is not a member of the class[^2].

### 69. What are static and dynamic binding?

- **Static binding**: Method calls are resolved at compile time.
- **Dynamic binding**: Method calls are resolved at runtime[^7][^2].


### 70. What is covariance and contravariance?

Related to the type relationships in overriding or implementing methods, generally regarding how return types and parameter types are treated in subclassing and interface implementation[^6].

## Practical/Others

### 71. Give a real-world example of encapsulation.

A capsule in medicine stores several drugs, encapsulating them inside a shell; only the shell is visible from outside[^2].

### 72. What is meant by data member and member function?

- **Data member**: An attribute or field in a class.
- **Member function**: A method defined in a class[^4][^2].


### 73. Can a class inherit from multiple classes in Java?

No, Java does not support multiple inheritance for classes (only through interfaces)[^2].

### 74. Explain hierarchical inheritance with example.

A base class is inherited by multiple derived classes. Example: `Animal` base class, `Dog` and `Cat` derived classes[^5].

### 75. What is the use of “final” keyword?

In Java, prevents a class from being inherited, a method from being overridden, or a variable from being changed[^2].

### 76. What is a namespace?

A declarative region that provides a scope to identifiers to avoid name conflicts[^2].

### 77. What is an inline function?

A function defined with keyword `inline` that signals the compiler to substitute the function code at the point of call (C++)[^2].

### 78. What is the difference between deep copy and shallow copy?

- **Shallow copy**: Copies object references.
- **Deep copy**: Copies the entire object and objects referenced by it[^5].


### 79. What are access specifiers?

Define how the members (fields or methods) of a class are accessed, similar to access modifiers[^2].

### 80. What is garbage collection?

Automatic memory management that reclaims memory occupied by objects no longer in use[^2].

## Miscellaneous

### 81. List some OOP languages.

- Java
- C++
- Python
- C\#
- Ruby[^7][^1]


### 82. What is operator overloading? Name some operators that cannot be overloaded.

Customizing the operation of existing operators for user-defined types. Operators like `::`, `.` and `?:` in C++ can’t be overloaded[^2].

### 83. What is an exception?

An event that disrupts normal flow of a program, usually handled by exception handling mechanisms like try/catch blocks[^5].

### 84. What is interface in Java?

A blueprint that can have only abstract methods and final variables. Classes implement interfaces to provide method implementations[^2].

### 85. Differentiate between aggregation and association.

- **Association**: General relationship between classes.
- **Aggregation**: Specialized association where one class contains a reference to another class, representing "has-a" relationship[^5].


### 86. What is the difference between early and late binding?

- **Early binding (static)**: Method call is resolved at compile time.
- **Late binding (dynamic)**: Method call is resolved at runtime[^7][^2].


### 87. Explain the term “constructor chaining”.

Invoking one constructor from another constructor in the same class or base class[^5].

### 88. Give an example of an immutable object.

Objects of `String` class in Java are immutable; once created, they cannot be altered[^2].

### 89. What is an abstract method?

A method that is declared but contains no implementation. Must be implemented by subclasses[^2].

### 90. What is shadowing in OOP?

When a variable declared in a subclass hides a variable of the same name in the parent class[^2].

## Scenario-based \& Experience

### 91. How would you use OOP to design an e-commerce platform?

By identifying main entities like Product, User, Order as classes; using inheritance for product types; applying encapsulation to secure attributes like price; and polymorphism for payment methods[^4].

### 92. Give an example where you used inheritance to reduce code redundancy.

Sharing common logging or validation code through a base class in a hierarchy of business objects[^4].

### 93. How do you handle versioning in OOP systems?

Through backward compatible changes, abstract base classes, and interface versioning[^8].

### 94. How to create a singleton class in your preferred OOP language?

By making the constructor private, providing a static method to get the unique instance, and storing a static reference to it[^8].

### 95. Explain the principle of “composition over inheritance”.

Favoring building classes with components rather than extending classes, to achieve greater flexibility and encapsulation[^8].

### 96. How do you ensure the security of data in OOP?

By using encapsulation, private fields, and providing controlled accessor and mutator methods[^2].

### 97. How do you refactor legacy procedural code to OOP?

Identify objects and their responsibilities; create classes; encapsulate data and behavior; and refactor functions into methods[^8].

### 98. Why is OOP considered more flexible than procedural programming?

Due to code reusability, scalability, maintainability, and easy-to-understand mapping to real-world problems[^3].

### 99. How do you test OOP code effectively?

By writing unit tests for classes and methods, mocking dependencies, and testing edge cases and object states[^8].

### 100. If you could improve one OOP concept, what would it be and why?

Open answer; can refer to better syntax for composition, improved type safety for interfaces, or more elegant solutions for multiple inheritance ambiguity.

These questions cover breadth and depth across OOP concepts, making them suitable for interviews at various levels[^1][^7][^3].

<div style="text-align: center">⁂</div>

[^1]: https://www.almabetter.com/bytes/articles/top-oops-interview-questions

[^2]: https://www.simplilearn.com/tutorials/java-tutorial/oops-interview-questions

[^3]: https://www.geeksforgeeks.org/interview-prep/oops-interview-questions/

[^4]: https://www.upgrad.com/blog/oops-interview-questions-answers-for-freshers-experienced/

[^5]: https://prepinsta.com/interview-preparation/technical-interview-questions/oops/

[^6]: https://www.slideshare.net/slideshow/oop-interview-questions-answers/79936180

[^7]: https://www.interviewbit.com/oops-interview-questions/

[^8]: https://www.lambdatest.com/learning-hub/oops-interview-questions

[^9]: https://www.simplilearn.com/tutorials/java-tutorial/oops-interview-questions-article

[^10]: https://github.com/Devinterview-io/oop-interview-questions

