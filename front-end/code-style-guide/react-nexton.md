# React - Nexton Best Practices

## Using Hooks instead of Classes

* Classes confuse both people and machines With classes you need to understand binding and the context in which functions are called, which often becomes confusion.
* Often with classes Mutually unrelated code often ends up together or related code tends to be split apart, it becomes more and more difficult to maintain. An example of such a case is event listeners, where you add listeners in componentDidMount and remove them in componentWillUnmount . Hooks let you combine these two
* Hooks are a new addition to React in version 16.8 that allows you use state and other React features, like lifecycle methods, without writing a class.
* Hooks let you always use functions instead of having to constantly switch between functions, classes, higher-order components, and render props.
* Hooks allow us to reuse stateful logic without changing your component hierarchy.

[Hooks API References](https://reactjs.org/docs/hooks-reference.html)

## Keep components small and function-specific

* As we all know, with React, it’s possible to have huge components that execute a number of tasks. But a better way to design components is to keep them small, so that one component corresponds to one function.
* Ideally, a single component should render a specific bit of your page or modify a particular behavior. There are many advantages to this.

## Reusability is important

* By sticking to the rule of one function = one component, we can improve the reusability of components. We should skip trying to build a new component for a function if there already exists a component for that function.

## DRY your code

* You can achieve this by scrutinizing the code for patterns and similarities. If you find any, it’s possible you’re repeating code and there’s scope to eliminate duplication. Most likely, a bit of rewriting can make it more concise.

```jsx
const buttons = ["facebook", "twitter", "youtube"];

return (
  <div>
    {buttons.map((button) => {
      return <IconButton onClick={doStuff(button)} iconClass={button} />;
    })}
  </div>
);
```

## Components Name

* It’s a good practice to name a component after the function that it executes so that it’s easily recognizable.
* For example, `ProductTable` – it conveys instantly what the component does. On the other hand, if we name the component based on the need for the code, it can be confuse at a future point of time.

## Testing Code

* The code we write should behave as expected, and be testable easily and quickly. It’s a good practice to name your test files identical to the source files with a `.test` suffix. It’ll then be easy to find the test files.

## File Structure

* We organize all the files by function type `components`, `actions`, `services`.

### Components Structure

#### Components

* The main components of the App like TopBar, SideBar, and Footer should be in the components folder.
* Small Components used in multiple components, should be be in the components folder.

#### Pages Components

* If there’s any small component used only by a particular Page Component , it makes sense to keep these smaller components all together within that component folder. The hierarchy will then be easy to understand – large components have their own folder and all their smaller parts are split into sub-folders. This way, we can easily extract code to any other project or even modify the code whenever we want.

```text
my-app
├── build
├── node_modules
├── public
│   ├── favicon.ico
│   ├── index.html
│   └── manifest.json
├── src
│   ├── assets
│   │   └──images
│   │       └── logo.svg
│   ├── components
|   |   ├── Authentication
|   |   |   ├── Auth.js
|   |   |   └── AuthenticateRoute.js
|   |   ├── Component
|   |   |   ├── Component.js
|   |   |   ├── Component.css
|   |   |   └── Component.test.js
│   │   ├── app
│   │   ├── app.js
│   │   └── app.test.js
|   ├── config
|   ├── helpers
|   ├── pages
|   ├── resources
|   ├── services
|   ├── store
│   ├── utils
│   │   ├── errorService.js
│   │   └── errorService.test.js
│   ├── index.js
│   ├── index.html
│   ├── routes.js
├── .gitignore
├── package.json
└── README.md
```

