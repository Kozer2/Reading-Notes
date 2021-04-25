
# Azure Dev Ops   

*What is it?*
Azure dev ops provides services for teams to work on and deploy apps.   
Azure provides:
- Repos
- Pipelines
- Boards
- Test Plans
- Artifacts


# MVC Basics  

Model-View-Controllers are a design pattern which helps developers develop web apps in a more efficient way than ASP.NET

The Model layer is the Object in your App. 
The View layer has the html controls. These are done with the Razor Engine.  
The Controller layer handles the user requests to the server.


# Tag helpers  

Tag helpers enable server side code to participate in creating and rendering HTML elements in a Razor file. 
Lets look at an example

``` public class Movie
{
    public int ID { get; set; }
    public string Title { get; set; }
    public DateTime ReleaseDate { get; set; }
    public string Genre { get; set; }
    public decimal Price { get; set; }
}
```
This code snippet would have a Razor markup that looks like
```
<label asp-for="Movie.Title"></label>
```
In HTML this looks like:
```
<label for="Movie_Title">Title</label>
```
# Download Bootstrap here:
[Bootstrap](https://getbootstrap.com/)
