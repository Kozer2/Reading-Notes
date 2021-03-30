
# Interfaces

What is an Interface? Well and Interface contains the definitions for groups of related functionalities that any non-abstract class needs to implement. 

They are defined by:
``` interface Example<T>
{
  bool IExamples( T obj);
}
```
What is with that "I" in front of example you may be wondering.   
Well by convention, all interface names in C# begin with an "I".


# Back to Basics

An Interface solves the issue of how we use something and seperate it from how it is implemented.   
We can use an Interface to allow us to write code that woks with all kinds of different implementations without needing to specify each one. 

Interfaces are **Always** implemented by more than one class.


# Interfaces # Two

As an Interface defines a contract, any class that uses that contract must use an implementation of the members defined inside the Interface. 

An Interface declaration can contain other declarations using any of the following:
- Methods
- Properties
- Indexers
- Events

These usually do not contain a body.   
Interfaces may also include:
- Constants
- Operators
- Static constructors
- nested types
- Static fields, methos, properties, events, and indexers. 
