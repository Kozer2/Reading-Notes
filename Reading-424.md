
# Azure blobs

In MVC *views* handle the apps way of presentting data. A view is an HTML template that can be edited like HTML. Their file tags are .cshtml

Your projects will start with a HomeController that works with a view in the home folder to create your basic index and privacy.  
Creating a view is simple. Here is an example:
```
@{
    ViewData["Title"] = "About";
}
<h2>@ViewData["Title"].</h2>
<h3>@ViewData["Message"]</h3>
```  

For a controller to return a view you just use ```View()``` in the return statement. 
*It doesn't matter if you implicitly return the ViewResult with return View(); or explicitly pass the view name to the View method with return View("<ViewName>");. 
 In both cases, view discovery searches for a matching view file in this order:*
  
  


# 4 ways to make a form in MVC
[Link to a useform form tutorial](https://www.completecsharptutorial.com/asp-net-mvc5/4-ways-to-create-form-in-asp-net-mvc.php)
