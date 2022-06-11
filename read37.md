# React
React is a JavaScript library,

Consider this variable declaration:

const element = <h1>Hello, world!</h1>;


It is called JSX, and it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like. JSX may remind you of a template language, but it comes with the full power of JavaScript.

React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

Embedding Expressions in JSX
In the example below, we declare a variable called name and then use it inside JSX by wrapping it in curly braces:
~~~
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;
~~~


After compilation, JSX expressions become regular JavaScript function calls and evaluate to JavaScript objects.

This means that you can use JSX inside of if statements and for loops, assign it to variables, accept it as arguments, and return it from functions:
~~~
function getGreeting(user) {
  if (user) {
    return <h1>Hello, {formatName(user)}!</h1>;
  }
  return <h1>Hello, Stranger.</h1>;
}
~~~


Specifying Children with JSX
If a tag is empty, you may close it immediately with />, like XML:
~~~
const element = <img src={user.avatarUrl} />;
~~~

### Rendering Elements


 React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.

 ### Rendering an Element into the DOM

We call this a “root” DOM node because everything inside it will be managed by React DOM.

Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.

## Components and Props

Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components.   

Converting a Function to a Class
You can convert a function component like Clock to a class in five steps:

### Create an ES6 class, with the same name, that extends React.Component.
Add a single empty method to it called render().
Move the body of the function into the render() method.
Replace props with this.props in the render() body.
Delete the remaining empty function declaration.

## Handling Events
Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

React events are named using camelCase, rather than lowercase.
With JSX you pass a function as the event handler, rather than a string.

### Utility-First Fundamentals

With Tailwind, you style elements by applying pre-existing classes directly in your HTML.


