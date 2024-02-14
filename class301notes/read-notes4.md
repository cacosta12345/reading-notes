# Class 04 Reading Notes

## Why is this important

* Forms are used everywhere and it's important to know what they are, what they can do and the different ways React uses forms. As our skills improve it is good practice to start using more advanced ways of writing long code. The ternary operator ? is a great way to minimize length of code instead of writing cumbersome if statements.

## How to Use Forms in React

1. What is a ‘Controlled Component’?

    * A controlled React Form is a component that gets controlled by React and does not manage its internal native HTML state anymore

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

    * Should we use controlled or uncontrolled forms basically. If the form is simple, one can go with an uncontrolled form. However, once the form gets more requirements (e.g. having control over the state), you would have to use a controlled form. They each have their uses, and are situationally dependant.

3. How do we target what the user is entering if we have an event handler on an input field?

    * event.target.value will get whatever the user inputs

## The Conditional (Ternary) Operator Explained

1. Why would we use a ternary operator?

    * Using a conditional, like an if statement, allows us to specify that a certain block of code should be executed if a certain condition is met. A shorter way to do an if statement is the ? operator.

2. Rewrite the following statement using a ternary statement:
    if(x===y){
    console.log(true);
    } else {
    console.log(false);
    }

    * console.log(x === y ? true : false);