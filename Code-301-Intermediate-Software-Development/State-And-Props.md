# State and Props

## Component Life Cycle Events

**1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**

In the component lifecycle, `render` occurs right before `componentDidMount`

**2. What is the very first thing to happen in the lifecycle of React?**

The first step in the lifecycle of a component is the constructor is called to begin creating the component.

**3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates**

 1. `constructor`
 2. `render`
 3. react updates  
 4. `componentDidMount`
 5. `componentWillUnmount`



**4. What does componentDidMount do?**

`componentDidMount` is a method that allows us to execute react code when the component is already place in the DOM. This method is called after the component is rendered during the mounting phase of the react lifecycle.

## React State And Props

**1. What types of things can you pass in the props?**
Values that we can pass in the props include any data type such as strings, functions, objects, integers, and arrays.

**2. What is the big difference between props and state?**
Props get *passed to* the component whereas 
state is managed *inside* the component.

**3. When do we re-render our application?**
When a change is made to the application's state.

**4. What are some examples of things that we could store in state?**
- We can track the number of times an element has been clicked on by incrementing the value each time a click is executed

- If we are working on a task tracker app for example, we can toggle a checkbox on or off + we can set a reminder if the box is checked or turn off the reminder if the box is unchecked 