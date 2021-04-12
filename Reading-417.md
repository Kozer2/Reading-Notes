
# Data Transfer Objects

A DTO is an objects that defines how the data is sent over the network to the client. 


# How to use DTOs

DTOs can be used for abstraction or data hiding. 
Here is an example of a DTO in action

``` public class Employee
    {
        public int Id { get; set; }
        public string FirstName { get; set; }
        public string LastName { get; set; }
        public string DepartmentName { get; set; }
        public decimal Basic { get; set; }
        public decimal DA { get; set; }
        public decimal HRA { get; set; }
        public decimal NetSalary { get; set; }
    }
```
First we create a class here with all kinds of info. 
In another DTO file we create a dto class
```
public class EmployeeDTO
    {
        public int Id { get; set; }
        public string FirstName { get; set; }
        public string LastName { get; set; }
        public string DepartmentName { get; set; }
    }
 ```
 
 This way we can control what is seen over the network. 
 
 DTOs should be immutable 
