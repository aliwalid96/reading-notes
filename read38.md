# React
Conditional Rendering
In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application.

### Element Variables
You can use variables to store elements. This can help you conditionally render a part of the component while the rest of the output doesn’t change.

### Inline If with Logical && Operator
You may embed expressions in JSX by wrapping them in curly braces. This includes the JavaScript logical && operator. It can be handy for conditionally including an element


Inline If-Else with Conditional Operator
Another method for conditionally rendering elements inline is to use the JavaScript conditional operator condition ? true : false.

In the example below, we use it to conditionally render a small block of text.

## Lists and Keys
First, let’s review how you transform lists in JavaScript.

Given the code below, we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it:

## Rendering Multiple Components
You can build collections of elements and include them in JSX using curly braces {}.

Below, we loop through the numbers array using the JavaScript map() function. We return a <li> element for each item. Finally, we assign the resulting array of elements to listItems:
~~~
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
);
~~~

Basic List Component
Usually you would render lists inside a component.

We can refactor the previous example into a component that accepts an array of numbers and outputs a list of elements.

## Keys
Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:



## Extracting Components with Keys
Keys only make sense in the context of the surrounding array.

For example, if you extract a ListItem component, you should keep the key on the <ListItem /> elements in the array rather than on the <li> element in the ListItem itself.

## Forms
HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state. For example, this form in plain HTML accepts a single name:


## Controlled Components
In HTML, form elements such as <input>, <textarea>, and <select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

The file input Tag
In HTML, an <input type="file"> lets the user choose one or more files from their device storage to be uploaded to a server or manipulated by JavaScript via the File API.



Handling Multiple Inputs
When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.

    
Controlled Input Null Value
Specifying the value prop on a controlled component prevents the user from changing the input unless you desire so. If you’ve specified a value but the input is still editable, you may have accidentally set value to undefined or null.

The following code demonstrates this. (The input is locked at first but becomes editable after a short delay.)


Alternatives to Controlled Components
It can sometimes be tedious to use controlled components, because you need to write an event handler for every way your data can change and pipe all of the input state through a React component. This can become particularly annoying when you are converting a preexisting codebase to React, or integrating a React application with a non-React library. In these situations, you might want to check out uncontrolled components, an alternative technique for implementing input forms.



## Composition vs Inheritance
React has a powerful composition model, and we recommend using composition instead of inheritance to reuse code between components.

In this section, we will consider a few problems where developers new to React often reach for inheritance, and show how we can solve them with composition.


### Containment
Some components don’t know their children ahead of time. This is especially common for components like Sidebar or Dialog that represent generic “boxes”.
