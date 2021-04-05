# MVC Tutorial
[Follow-along](https://docs.microsoft.com/en-us/aspnet/core/data/ef-mvc/intro?view=aspnetcore-5.0) 



# Entity Framework Core

What is EFC? EFC is a cross platform light weight version of EFDA. 

EFC uses models which are made up of classes and context objects to access data in the database. 

EFC allows you to:
- Generate a model from an existing database
- Hand code a model to match the database
- Use Migrations to create a database from the model.


# Data seeding  
Data seeding is something we all should already be familer with. It is the process of adding in initial data to a newly created database. 

EFC can make this easier by allowing seed data to be associated with entity types, which it then automatically, inserts, updates, or deletes as needed.

Example:

```
modelBuilder.Entity<Blog>().HasData(new Blog { BlogId = 1, Url = "http://sample.com" });


modelBuilder.Entity<Post>().HasData(
    new Post { BlogId = 1, PostId = 1, Title = "First post", Content = "Test 1" });



modelBuilder.Entity<Post>().HasData(
    new { BlogId = 1, PostId = 2, Title = "Second post", Content = "Test 2" });


modelBuilder.Entity<Post>().OwnsOne(p => p.AuthorName).HasData(
    new { PostId = 1, First = "Andriy", Last = "Svyryd" },
    new { PostId = 2, First = "Diego", Last = "Vega" });
 
 ```
 
 
 It does have its drawbacks and if you are working with large amounts of data, or data that needs set states, it is recommended to use custom feed data. 
 
 
 # EFC Core tutorial
 [Follow-Along](https://docs.microsoft.com/en-us/aspnet/core/data/ef-rp/intro?view=aspnetcore-2.1&tabs=visual-studio)
 
 
 # Youtube video  
 [Follow alongf video](https://www.youtube.com/watch?v=aIkpVzqLuhA)
 
 
 
 # User Secrets 
 What are user secrets? 
 They are a way to securly store private user information. These are things like, API keys, Client secrets, and connection strings. 
 
 To enable these
 1. Right click your project
 2. Select "Manage User Secrets"

This should open your appsettings.json file located somewhere like: %APPDATA%\microsoft\UserSecrets\<userSecretsId>\secrets.json.

``` {
  "myBingAPIKey": "{VALUE}",
  "textAPIKey": "{VALUE}",
  "ConnectionStrings": {
    "AzureConnection": "{CONNECTION STRING HERE}"
}
```
