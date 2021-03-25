
# Classes  

A class is known as a *reference type*. When first created they have the value of null until given a new operator. 

To decalre a class you give it the **class** keyword such as: ```public class Example ```
A class defines a type of object but it is not an object. An object is an instance of a class. 
Classes can be inherited and can inherit any other class. 

# Constructors  

When you create a class, a *constructor* is called. A single class can have multiple constructors. 
You do not need to provide one when you create a class. C# can create one for you with default values. 


# Properties  

- Properties allow a class to expose a way for getting and setting values outside of itself. 
- You use the ```value ``` keyword ato define the value that is being assigned
- Properties can both **Read** and **Write** 


# Stack and Heap  
Webpage refused to load 

# Fundamentals of Garbage Collection  

The Garbage Collector in the CLR serves as a memory manager. 
- This can be automatically done via the code in managed code and thus a developer does not need to worry about doing it themselves. 

Benefits of the GC is that it allows developes to be free from having to manage memory manually. 
It manages objects in the head efficiently. 
Clears objects not being used and makes sure no object can use the contents of another




Objects that are a 0 or a 1 are short lived and known as *ephemeral generations*. They are given different memory sizes depending on their type. 
``` Workstation/server GC	                  32-bit	                    64-bit
    Workstation GC	                        16 MB	                      256 MB
    Server GC	                                64 MB	                      4 GB
    Server GC with > 4 logical CPUs	        32 MB	                      2 GB
    Server GC with > 8 logical CPUs	        16 MB	                      1 GB
``` 
