
# Claims Based Authentication

When creating an identity it may be issued one or more claims. A claim is a name-value-pair that represents what the subject is, not what it can do. 


Claim based authorization checks are declarative. They are used with a Controller or an action.


# Intro to claims

As we have talked about before, Authentication is the process of figuring out who a user is. Authoerization is what they are allowed to do. 

Claims based authentication is not as confusing as it sounds. Claims contain a statement of a name and a value. Like a name or DoB. 

``` 
public class ClaimsIdentity: IIdentity
{
    public string AuthenticationType { get; }
    public bool IsAuthenticated { get; }
    public IEnumerable<Claim> Claims { get; }

    public Claim FindFirst(string type) { /*...*/ }
    public Claim HasClaim(string type, string value) { /*...*/ }
}
```
The above is an example version of what a simple version of a class looks like for claim auth


