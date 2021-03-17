

# Try and Catch Blocks  

If you have a block of that you feel *might* throw an exception or error you can put it into a try block with some following lines of code aimed to handle the error in a following catch block. 
What does this do?  
If the code in the try blocks throws and error, the catch blocks will try and handle it without crashing the code. 


# Exception Handling  
C# Has several exception handling statements. They are:
- ```throw```
- ```try-catch```
- ```ry-finally```
- ```try-catch-finally```



# C\# in a Nutshell  
A Try block **must** be followed by a Catch block or a Finally block. Or Both. 
The Catch block can access the exception errors information and you can then use this block to help your program through it or rethrow the error to log it. 
A Finally block adds determinism to your program. 

*Catch Clause* 
- Specifies what type of exception to catch. 
- Using ```System.Exception``` Catches all possible errors. 
- You will usually want to catch only specific erros. 

*Finally* block. 
- A Finally block always executes regardless if the code has thrown an exception. 
- They are typically used to help cleanup code. 
- Can break by 2 things.
  - An infinite loop
  - Or ending the process early. 

 
