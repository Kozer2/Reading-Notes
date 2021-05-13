

# Fetching with React Hooks

Currently in React, we use hooks to fetch data by using state effect hooks. This will change and in the future instead of hooks, something called Suspense will be in charge of getting data.
[Hook Tutorial](https://www.robinwieruch.de/react-hooks-fetch-data)

Example Hook: 
```
import React from "react";
import useFetch from "react-fetch-hook";

const Component = () => {
  const { isLoading, data } = useFetch("https://swapi.co/api/people/1");

  return isLoading ? (
    <div>Loading...</div>
  ) : (
    <UserProfile {...data} />
  );
};
```
Use ```npm i react-fetch-hook --save``` to install the hook


# React Query

React Query makes faetching, caching, synchronizing and updating server state a very simple matter. 

Many state libraries do not effectivly handle server state because server state is different from client state. 
React Query handles server state in a simple matter and is one of the best libraries for it. 
