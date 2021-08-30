# Passing Functions as Props

## React Docs - lists and keys

### 1- What does .map() return?
- We assign the new array
### 2- If I want to loop through an array and display each value in JSX, how do I do that in React?
    const numbers = [1, 2, 3, 4, 5];
    const listItems = numbers.map((number) =>
       <li>{number}</li>
    );
### 3- Each list item needs a unique ____.
- key
### 4-What is the purpose of a key?
- Keys help React identify which items have changed, are added


## The Spread Operator

### 1-  What is the spread operator?
- Spread operator allows an iterable to expand in places where arguments are expected. It is mostly used in the variable array where there is more than 1 values are expected. It allows us the privilege to obtain a list of parameters from an array. Syntax of Spread operator is same as Rest parameter but it works completely opposite of it.

### 2-  List 4 things that the spread operator can do.
- The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

### 3- Give an example of using the spread operator to combine two arrays.
    let arr1 = [1,2,3];
    let arr2 = [4,5,6];
    let arr3 = [...arr1, ...arr2];

### 4- Give an example of using the spread operator to add a new item to an array.
    let numbers = [0, 1, 2];
    let newNumber = 12;
    numbers = [...numbers, newNumber];

### 5- Give an example of using the spread operator to combine two objects into one.
    let obj1 = { name: 'Mohammad', age: 28 };
    let obj2 = { name: 'Ahmad', y: 25 };
    let merge = ( ...objects ) => ( { ...objects } );

    let mergedObj = merge (obj1, obj2);

## How to Pass Functions Between Components
### 1- In the video, what is the first step that the developer does to pass functions between components?
- Add constructor function and super
### 2- In your own words, what does the increment function do?
- find the matching name update that one its gonna work the same either
### 3- How can you pass a method from a parent component into a child component?
- The data can be passed using the props and this data can be modified by the state
### 4- How does the child component invoke a method that was passed to it from a parent component?
- Example :

       import React from 'react'

       class Child extends React.Component {
       constructor (props) {
       super(props)
       this.state = { name: 'Mohammad' }
       }
       setFromOutside (title) {
       this.setState({ name: title })
       }

       render () {
       return (
       <h1>{this.state.name}</h1>
       )
       }
       }
       export default Child