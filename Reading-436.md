
# React

How to display Hello World with React
``` 
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);
```
That is it. 

What is React?  
React is a JavaScript library

# JSX

JSX is a syntax extension to JS. Use it with React to help design your UI. Since React knows that rendering logic is tied with other UI logic, it allows us to use other means to design our site. 

Example of using JSX with a function in React:
```
function formatName(user) {
  return user.firstName + ' ' + user.lastName;
}

const user = {
  firstName: 'Harper',
  lastName: 'Perez'
};

const element = (
  <h1>
    Hello, {formatName(user)}!
  </h1>
);

ReactDOM.render(
  element,
  document.getElementById('root')
);
```

# Rendering with React

React elements are plain objects are are cheap and easy to create. 

React uses a root normally called ```<div id="root"></div>```

# [React Router](https://reactrouter.com/web/guides/quick-start)


# [React Bootstrap](https://react-bootstrap.github.io/)\


# [React Typescript](https://www.typescriptlang.org/docs/handbook/react.html)
