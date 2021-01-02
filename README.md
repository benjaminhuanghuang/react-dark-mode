# How to do Dark Mode with React Hooks
- https://dev.to/joefstack/how-to-do-dark-mode-with-react-hooks-23gi




## CSS Variable
```
html[data-theme="light"]  {
  --color: rgb(5, 5, 5);
  --background-color: rgb(250, 250, 250);
}

html[data-theme="dark"]  {
  --color: rgb(250, 250, 250);
  --background-color: rgb(5, 5, 5);
}

.App-header {
  background-color:var(--background-color);
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  font-size: calc(10px + 2vmin);
  color:var(--color);
}
```

## DOM
using the HTML data- attribute, which allows us to store information in semantic HTML elements
````
  document.getElementsByTagName("HTML")[0]
          .setAttribute("data-theme", localStorage.getItem("theme"));
```
