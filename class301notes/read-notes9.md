# Reading Notes Class 9

## Functionanl Programming Concepts

1. What is functional programming?

    * Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia

2. What is a pure function and how do we know if something is a pure function?

    * A pure function is a function in computer programming that has two main characteristics: Deterministic, No side effects.

    * Here are some key points to identify whether a function is pure:

    Input-Output Relationship: A pure function's output is solely determined by its input parameters. It doesn't rely on any external state or data.

    No Side Effects: The function doesn't modify any external state or have any observable side effects. This includes modifying global variables, modifying input parameters, or performing I/O operations.

    Immutable Data: If a function uses data structures, it should not modify them. Instead, it should create and return new data structures.

    No External Dependencies: A pure function should not rely on external systems or services that might introduce variability or side effects.

3. What are the benefits of a pure function?

    * predictability, testability, debugging, parrallelization, memoization, referential transparency

4. What is immutability?

    * Immutability means that once an object is created, its state cannot be changed. Operations that seem to modify the object actually create a new object with the desired changes. It promotes predictability, thread safety, and is a fundamental concept in functional programming.

5. What is Referential transparency?

    * Referential transparency means that a function, given the same inputs, will always return the same output, and its invocation can be replaced with its result without affecting program behavior.

(questions 2-5 were answered with help from chatGPT since I don't have an account with the article site and couldn't read it)    

## Node JS Tutorial for Beginners 6

1. What is a module?

    * Essentially just another JS file

2. What does the word ‘require’ do?

    * lets you use the file you are "requiring". It's like using import in React

3. How do we bring another module into the file the we are working in?

    * In the node module you want to share, you have to export. Ie. module.exports.counter. In the file you want to use that in you have to "require" it. I.e. var counter = require('./count')

4. export it. module.exports = whateverYouWantToExport