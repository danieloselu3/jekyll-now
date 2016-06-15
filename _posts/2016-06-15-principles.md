---
layout:post
title:PRINCIPLES OF OOP
---
In order for a programming language to be object-oriented, it has to enable working with classes and objects as well as the implementation and use of the fundamental object-oriented principles and concepts: inheritance, abstraction, encapsulation and polymorphism. Let’s summarize each of these fundamental principles of OOP:<br />

     **Encapsulation**
       We will learn to hide unnecessary details in our classes and provide a clear and simple interface for working with them.
     **Inheritance**
       We will explain how class hierarchies improve code readability and enable the reuse of functionality.
     **Abstraction**
       We will learn how to work through abstractions: to deal with objects considering their important characteristics and ignore all other details.
     **Polymorphism**
       We will explain how to work in the same manner with different objects, which define a specific implementation of some abstract behavior.
       Some OOP theorists also put the concept of exception handling as additional fifth fundamental principle of OOP. We shall not get into a detailed dispute about    whether or not exceptions are part of OOP and rather will note that exceptions are supported in all modern object-oriented languages and are the primary mechanism of handling errors and unusual situations in object-oriented programming. Exceptions always come together with OOP and their importance is explained in details in the chapter "Exception Handling".<br />


**Inheritance**
 Inheritance is a fundamental principle of object-oriented programming. It allows a class to "inherit" (behavior or characteristics) of another, more general class. For example, a lion belongs to the biological family of cats (Felidae). All cats that have four paws, are predators and hunt their prey. This functionality can be coded once in the Felidae class and all its predators can reuse it – Tiger, Puma, Bobcat, etc. Inheritance is described as is-kind-of relationship, e.g. Tiger is kind of Animal.<br />
 
How Does Inheritance Work in .NET?
 Inheritance in .NET is defined with a special construct in the class declaration. In .NET and other modern programming languages, a class can inherit from a single class only (single inheritance), unlike C++ which supports inheriting from multiple classes (multiple inheritance). This limitation is necessitated by the difficulty in deciding which method to use when there are duplicate methods across classes (in C++, this problem is solved in a very complicated manner). In .NET, classes can inherit multiple interfaces, which we will discuss later.
 The class from which we inherit is referred to as parent class or base class / super class.<br />


**Abstraction**
       The next core principle of object-oriented programming we are about to examine is "abstraction". Abstraction means working with something we know how to use      without knowing how it works internally. A good example is a television set. We don’t need to know the inner workings of a TV, in order to use it. All we need is a remote control with a small set of buttons (the interface of the remote) and we will be able to watch TV.<br />
 The same goes for objects in OOP. If we have an object Laptop and it needs a processor, we use the object Processor. We do not know (or rather it is of no concern to us) how it calculates. In order to use it, it’s sufficient to call the method Calculate() with appropriate parameters.<br />
 Abstraction is something we do every day. This is an action, which obscures all details of a certain object that do not concern us and only uses the details, which are relevant to the problem we are solving. For example, in hardware configurations, there is an abstraction called "data storage device" which can be a hard disk, USB memory stick or CD-ROM drive. Each of these works in a different way internally but, from the point of view of the operating system and its applications, it is used in the same way – it stores files and folders. In Windows we have Windows Explorer and it can work with all devices in the same way, regardless of whether a device is a hard drive or a USB stick. It works with the abstraction "storage device" and is not involved with how data is read or written. The drivers of the particular device take care of that. They are implementations of the interface "data storage device".<br />
 Abstraction is one of the most important concepts in programming and OOP. It allows us to write code, which works with abstract data structures (like dictionaries, lists, arrays and others). We can work with an abstract data type by using its interface without concerning ourselves with its implementation. For instance, we can save to a file all elements from a list without bothering if it is implemented with an array, a linked list, etc. The code remains unchanged, when we work with other data types. We can even write new data types (we will discuss this later) and make them work with our program without changing it.<br />
 Abstraction allows us to do something very important – define an interface for our applications, i.e. to define all tasks the program is capable to execute and their respective input and output data. That way we can make a couple of small programs, each handling a smaller task. When we combine this with the ability to work with abstract data, we achieve great flexibility in integrating these small programs and much more opportunities for code reuse. These small subprograms are referred to as components. This approach for writing programs is widely adopted since it allows us to reuse not only objects, but entire subprograms as well.<br />


**Encapsulation**
 Encapsulation is one of the main concepts in OOP. It is also called "information hiding". An object has to provide its users only with the essential information for manipulation, without the internal details. A Secretary using a Laptop only knows about its screen, keyboard and mouse. Everything else is hidden internally under the cover. She does not know about the inner workings of Laptop, because she doesn’t need to, and if she does, she might make a mess. Therefore parts of the properties and methods remain hidden to her.<br />
 The person writing the class has to decide what should be hidden and what not. When we program, we must define as private every method or field which other classes should not be able to access.<br />


**Polymorphism**
 The next fundamental principle of Object-Oriented Programming is "Polymorphism". Polymorphism allows treating objects of a derived class as objects of its base class. For example, big cats (base class) catch their prey (a method) in different ways. A Lion (derived class) sneaks on it, while a Cheetah (another derived class) simply outruns it.<br />
 Polymorphism allows us to treat a cat of random size just like a big cat and command it "catch your prey", regardless of its exact size.
 Polymorphism can bear strong resemblance to abstraction, but it is mostly related to overriding methods in derived classes, in order to change their original behavior inherited from the base class. Abstraction is associated with creating an interface of a component or functionality (defining a role). We are going to explain method overriding shortly.

