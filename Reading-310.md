
A **call stack** is a way for the interpreter to track the places of functions that are being ran and their order. 
- When a function is called it is added to the current stack.
- Functions that that function call are added above it
- -When the function is finished it is removed from the stack and the interpreter continues from where it left off
- If the stack htakes up more memory that it was given, it will cause a stack overflow error 




The Call stack uses the Last In, First Out principle to manage function invocations. 
If you have 3 functions arranaged with each of them calling the one above it with the first not calling any, with the last function being called first, that first function called which is ***the last function*** will be the last function to appear on your terminal. 

JavaScript like many languages has errors that you can learn to read. Once you know them, it will be far easier to track down what is wrong with you code. 
- A reference error means you do not have a declared variable for what you are trying to call
- A syntax error means that you are trying to parse invalid objects. These can range from misspelling things to forgetting commas. 
- A range error means that you were working with an object and gave it a wrong length
- A type error means that you tried to compare invalid types. Such as a string with a number. 
