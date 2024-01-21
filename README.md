# Workshop React JS

## What is React?

React is an open-source JavaScript library developed by Facebook. When using React, we work with reusable components (e.g., buttons). Components are self-contained pieces of code that encapsulate both their logic and the associated UI. This facilitates maintenance and scalability of the application.

## Why Use React?

- Efficient state management.
- Similar to React Native with minor differences, enabling mobile app development.
- React uses a virtual DOM, an interface that represents the structure of a document.

Download Node.js: Node.js
Check the installation:
```bash
node –v
npm –v

```
## Creating a React Project

Start by installing create-react-app on your machine:

```bash
npm install -g create-react-app
```

## Creating a New React Project

To create a new React project, use the following command:

```bash
npx create-react-app My-React-Project
```

Once launched, open your browser and go to the following URL: 
http://localhost:3000 

The React project is created.



## What is a component :
Components are standalone and reusable elements that enable structuring a user interface (UI) into modular and independent pieces.

## Roles of Components: 

Modularity:
Components are self-contained units that can be reused in different parts of our code.

Reusability:
Creating a reusable component helps standardize the UI and prevent code duplication.

Encapsulation:
Each component has its own logic and state, making it completely independent of other components.

## How to Create a Component?

Create a file for your component with the extension .js or .jsx.

A functional component looks like this:

 ```bash
import React from 'react'; 
function MyComponent() { 
  return ( 
    <div> 
      {/* Component content */} 
    </div> 
  ); 
} 
```
And export your component to use it in other files.
```bash
export default MyComponent
```

Props:
Props are properties passed from a parent component to its child component. You can pass variables, functions, objects, etc., to the child component.

Example:

```bash
<MyComponent name="John" age={25} />
function MyComponent(props) {
  console.log(props.name);  // Displays "John"
  console.log(props.age);  // Displays 25
}
```
or
```bash
function MyComponent({ name, age }) {
  console.log(name);  // Displays "John"
  console.log(age);  // Displays 25
}
```
## React router DOM 

React Router DOM is a library that facilitates navigation management in a React application by allowing the creation of routes and synchronizing the URL state with the UI. It provides a declarative way to define the navigation structure of your application using React components.

Installation:
```bash
npm install react-router-dom 
```

example :
```bash
<BrowserRouter>
  <Routes>
    <Route path="/" element={<HomePage />} />
    <Route path="/faq" element={<FaqPage />} />
    <Route path="/resetPassword" element={<ResetPassword />} />
  </Routes>
</BrowserRouter>
```
## useState :  

State is a fundamental concept in React that represents the dynamic data of a component. State allows a component to track internal changes over time, typically in response to user interactions or other events. When a component's state changes, React automatically updates the UI to reflect these changes.

## useEffect :  

Effects are used to perform actions after the initial rendering of the component or after each update of the state. These actions may include operations such as fetching data from a server, subscribing to events, modifying the DOM, etc. Effects are used to handle the non-declarative aspects of React components.
- Useful for asynchronous operations like network calls, API requests, etc., after the initial rendering of the component.
- Used to manage side effects such as DOM manipulation, event subscriptions, or resource cleanup after unmounting a component.

## Exercices : 

Create a website (of your choice) using reusable components. The site should have at least 2 pages that display dynamic state changes and automatically update after 5 seconds of being on the page. Don't forget the CSS.

 
