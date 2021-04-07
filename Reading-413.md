
# Dependency Injection

Dependency Injection (DI) is a technique that ASP.NET Core uses to achieve Inversion of Control between classes and their dependencies. 

Dependency Injection addresses problems of Interface and inheritance by:
- Using an interface or base class to abstrract the dependency implementation
- Registers the dependency into a service container
- Injects the service into the constructor of the class where it needs to be used. 

These can be injected in startup so that you can have the services at the start. 


# Repository pattern

Repositories are classes or components that encapsulate the logic required to access their data sources. 

You should have 1 repository class per aggregate or aggregate root. 

A repository allows you to populate data in memory that is coming from the database in the form of domain entities. 

Using this pattern, it is easier to test the logic of your application. The decoupled approach allows you to create and run unit tests 
that focuys on the logic of your application without needing connectivity to the database.

The repository pattern differs from the Data Access CLass because unlike the DAL, it does not directly performs data access and persistence. It marks the data with the operations you
want to perform in the memory. 

They are not **Mandatory** 

# Repository Design Pattern
Did not open or load. 


# SOLID Principlies.  
The SOLID principles come from Robert Martin. 
These are:
- Single Responsibility Principle
  - This is the idea that every method or class in your app should have exactly one reason to change
- The Open/Close Principle
  - This states that software should be open for extension, but closed to modification
- The Liskov Substitution Principle
  - This states that an object should be able to be replaced with a type derived from it without breaking the application
- The Interface Segregation Principle
  - This states that clients should not be forced to rely on interfaces they do not use
- And The Dependency Inversion Principle
  - And finally this says that we need to make all coupling as loose as we possibly can. 



