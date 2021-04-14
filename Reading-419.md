
# Intro to Identity 

ASP.NET Core identity is a system that adds login functions to ASP.NET Core apps. 

You can use SQL server databases to store usernames and passwords and other user data. 

You need to start a Visual Studio project with Individual user Accounts on. 

# Identity Demystified 
Identities are made up of 3 classes. 
1. Claim
2. ClaimsIdentity
3. ClaimsPrincipal 


A claim is a single fact about the user. A user can have multiple claims but each claim is only 1 fact, such as: First name, Last name, DoB, Age, etc. 

ClaimsIdentity is a form of identification, it s a way for the identity to tell the server what it is. 

ClaimsPrincipal is the actual user

Terms for Identity: 
- Authenticate
    - Gets the user’s information if any exists (e.g. decoding the user’s cookie, if one exists)
- Challenge
    - Requests authentication by the user (e.g. showing a login page)
- SignIn
    - Persists the user’s information somewhere (e.g. writes a cookies)
- SignOut
    - Removes the user’s persisted information (e.g. deletes the cookies)
- Forbid
    - Denies access to a resource for unauthenticated users or authenticated but unauthorized users
