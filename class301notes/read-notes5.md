# Reading Notes Class 5

## Thinking in React

1. What is the single responsibility principle and how does it apply to components?

    * a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

2. What does it mean to build a ‘static’ version of your application?

    * build a version that renders the UI from your data model without adding any interactivity… yet! It’s often easier to build the static version first and add interactivity later. Building a static version requires a lot of typing and no thinking, but adding interactivity requires a lot of thinking and not a lot of typing.

3. Once you have a static application, what do you need to add?

    * useState to add interactivity

4. What are the three questions you can ask to determine if something is state?

    * Does it remain unchanged over time? If so, it isn’t state.

    * Is it passed in from a parent via props? If so, it isn’t state.

    * Can you compute it based on existing state or props in your component? If so, it definitely isn’t state!

5. How can you identify where state needs to live?

    * Identify every component that renders something based on that state.

    * Find their closest common parent component—a component above them all in the hierarchy.

    * Decide where the state should live:
    Often, you can put the state directly into their common parent.

    * You can also put the state into some component above their common parent.

    * If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common parent component.

## Higher-Order Functions

1. What is a “higher-order function”?

    * Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions

2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

    * using a call back function that checks if a value (m) is greater than the parameter given (n)

3. Explain how either map or reduce operates, with regards to higher-order functions.

    * The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function.

    * The higher-order operation that represents this pattern is called reduce (sometimes also called fold). It builds a value by repeatedly taking a single element from the array and combining it with the current value. When summing numbers, you’d start with the number zero and, for each element, add that to the sum.