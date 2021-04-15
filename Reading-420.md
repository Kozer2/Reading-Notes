
# Claims based Authorization

When an identity is made, it is given one or more claims from the party that made it. A Claim is a value pair that represents what the subject is. 

You can add claim checks to your app. You first need to build and register the given policy in your ```startup.cs``` file. 


# Intro to claims

Claims are what you are authorized to do. As opposed to Authentication which is who you are. 

Using ```ClaimsPrincipal``` you can implement ```IPrincipal``` which is the first step in claims. 


# JWT Authentication 

JWT stands for JSON Webt Token, which is a means of representing claims that need to be transferred between two parties. 

The claims are encoded as a JSON object that is then signed using a JSON Web Signature or encrypted using a JSON Web Encryption. 

There are usually 3 parts to a JWT. They are:
1. The header which is made up of the alg or algorithm and the typ which is the type of token.
2. The Payload which contains standard claims.
3. The Signature which is made with a base64url encoding of the header and payload and trhen encrypted with an HMAC-SHA256
