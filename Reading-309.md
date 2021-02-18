A pure function returns the same results if given the same arguements every time. 
That means a function is not pure if it uses a random number or if it reads files. 
To make a function pure, make it so that it does not change its variables. If it is given A. Make it return B.

Pure functions are immutable and in JS you can use recursion instead of for loops to keep this immutability. 

If you are given large sets of numbers or objects to work with, you should use hash functions to make the work quicker
