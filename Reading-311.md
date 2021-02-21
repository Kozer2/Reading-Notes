
You might be asking yourself, "***What is EJS?***
Well **I** am here to tell you that EJS is Embedded JavaScript!
"Well, what does that mean?!"

It means that EJS allows you to make HTML amrkup with normal JS. Simple. Easy. Done. 

To install EJS just run this command in ubuntu ```npm install ejs```
Make sure EJS is added in your package.json. Should look like     

```{
  "name": "node-ejs",
  "main": "server.js",
  "dependencies": {
    "ejs": "^3.1.5",
    "express": "^4.17.1"
  }
]
```
You'll also need to set the view engine for your app using ```app.set('view engine', 'ejs');``` or something similar. 
Below is an example of our HTML to utulize EJS in the browser.
```<ul>
    <% mascots.forEach(function(mascot) { %>
        <li>
            <strong><%= mascot.name %></strong>
            representing <%= mascot.organization %>, born <%= mascot.birth_year %>
        </li>
    <% }); %>
</ul>
```
EJS will use forEach to iterate over items in a list to display them all to the page.
