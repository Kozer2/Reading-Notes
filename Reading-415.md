
# MVC Routing

The good news is, when you create a new ASP.NET MVC app, it is already setup to use the ASP.NET routing.   
This routing is setup in the Webt Config File (Web.config) where it has 4 sections. 
1. system.web.httpModules section
2. system.web.httpHandlers section
3. system.websever.modules section
4. system.webserver.handlers section

And in the apps Global.asax file. This is the *important* file. 


# ASP.NET Core routing

Routing is used to match incoming HTTP requests and dispatching those requests to the apps endpoints.  
Apps configure routing by:
- Controllers
- Razor Pages
- SignalR
- gRPC Services
- Endpoint-enabled middleware
- Delegates and lambdas 


You can get to endpoints using the MapGet method. 

ASP.NET Core has endpoints that are:
- Executable
- Extensible
- Selectable
- Enumerable


You generate URLs by calling the LinkGenerator.GetPathByAddress method.  
This method allows you to use address which themselves use endpoints

To implement Address you need:
- Using Endpoint(string) as the address:
  - Provides similar functionality to the MVCs route
  - Resolves the provided string against the metadata 
  - Throws an exception on startup if multiple endpoints use the same name
  - Recommended for general purpose use
 - Using route values as the address:
  - Provides similar functionality to controllers and Razor pages
  - Very complex to extend and debug
  - Provides the implementation used by IUrlHelper. 
