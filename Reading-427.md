
# View Components

View Components are sort of like views, but more powerful. They don't need model binding and only need data when called.   
A view component:
- Renders a chunk rather than a whole response.
- Includes the same separation-of-concerns and testability benefits found between a controller and view.
- Can have parameters and business logic.
- Is typically invoked from a layout page.

View Components use ```InvokeAsync``` as a method to return data from their Task. 

Lets look at an example of how to create a view component. 
``` 
[ViewComponent(Name = "Example")]
public class ExampleViewComponent : ViewComponent
{
    return Content("Example");
}
```

To call or invoke this view on our pages, we would use ```@Component.Invoke("Example")```
