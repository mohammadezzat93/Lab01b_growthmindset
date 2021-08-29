# State and Props
 
 ## React lifecycle

 ### 1- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

- React render() is being called before componentDidMount()

### 2- What is the very first thing to happen in the lifecycle of React?

- Constructor()

### 3- Put the following things in the order that they happen: 
 A - constructor -> B - render -> C - componentDidMount -> D - React Updates -> E - componentWillUnmount

### 4- What does componentDidMount do?

- The componentDidMount() method allows us to execute the React code when the component is already placed in the DOM (Document Object Model). This method is called during the Mounting phase of the React Life-cycle i.e after the component is rendered.

## React State Vs Props

### 1- What types of things can you pass in the props?
- Props allows us to pass values from a parent component down to a child component. The values can be any data type, from strings to functions, objects, etc.

### 2- What is the big difference between props and state?
- **Props** : are immutable
- **State** : is mutable

### 3- When do we re-render our application?
- React components automatically re-render whenever there is a change in their state or props. A simple update of the state, from anywhere in the code, causes all the User Interface (UI) elements to be re-rendered automatically.
- A component’s setState() method is called.

### 4- What are some examples of things that we could store in state?
-In React, whenever we are working with any data, we always use state for storing that data which may be a **string**, **number** or any **complex object**.