# Reading Notes Class 02

## Why this is important

* As we get further into React, it's important to know how it behaves and it's limitations. Using state and props is one of the best things about React, but it can be a bit confusing to know when to use what.

## React Lifecycle

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

    * render

2. What is the very first thing to happen in the lifecycle of React?

    * Mounting, specifically constructor

3. Put the following things in the order that they happen:

    * constructor, render, react updates, componentDidMount, componentWillUnmount

## React State Vs Props

1. What types of things can you pass in the props?

    * primitives, functions, objects, arrays, react elements 
    * (chatGPT helped here)

2. What is the big difference between props and state?

    * If when handling info in a component and only in the component and no where else, you would use state. If your  handling that info outside the component, like in a parent for example, then you would use props.

3. When do we re-render our application?

    * When the state of a component changes

4. What are some examples of things that we could store in state?

    * User input ex. form fields, text content area

    * UI state ex. toggling state active or inactive

    * counter