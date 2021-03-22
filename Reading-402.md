
# Unit Testing

Unit tests test speciific blocks of your code. In C# we can write a method and then test it using our best practices  
1. Arranage, Act, Asset.   
- Create the data you will need to test your method.  
- Invoke the method using the data  
- Verify how it went  
2. One Assert per test Method  
- Don't try to test multiple things. Try to only test one thing at a time.   
3. Avoid Test Interdependence  
- Do not piggyback off of one test when moving into another. While it could work for a time it may break.   
4. Keep it short, sweet, and visible  
- aBy keeping the tests as easy to follow as possible, when something breaks we can more easily figure out what went wrong.   
5. Recognize Test setup Pain as a smell  
- If you are finding that you are coding large amounts to get a test setup, you have a design problem with your code. Keep the tests light.  
6. Add them to the Build. 
- If you are testing multiple things and 1 breaks, stop there and fix that problem. Don't ignore it to keep moving on. 

# XUNIT Documentation
**Did not load. 404 error.**


# Art of Readme

A README exists because it is important to the function of whatever it is about.  
A README should: 
- Tell the user what it is about
- Show them what it looks like when it functions
- Tell them how to use it
- Other info as needed

READMEs should be long enough to hit all key points, but should be kept as short as possible. 

When making a README there are some key elements to be aware of
1. Give it a simple Name that is descriptive. 
2. Give 1 quick line that tells the reader what the module does. 
3. Tell the user how the product is used
4. Give them easy access to the API
5. Tell them how to install it. Remember, they may be new. 
6. The License. If you have a restrictive license, try to put it closer to the top. 


https://github.com/jehna/readme-best-practices
