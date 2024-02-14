# Reading Notes Class 03

## Why this is important

* React has a few key differences from plain JavaScript. One of those is the fact that you can not simply write for loops to iterate through arrays. A way to get around that in React, is using the map() method.

## React Docs- lists and keys

1. What does .map() return?

    * Returns a copy array with the length of the original

2. If I want to loop through an array and display each value in JSX, how do I do that in React?

    * Use a function that uses the map method to loop through an array and then you can return each "item" as a list item (li). Example used in the reading:
    <!-- const listItems = products.map(product =>

    <li key={product.id}>
    {product.title}
     </li>
    );

    return (
    <ul>{listItems}</ul>
    ); -->

3. Each list item needs a unique ____.

    * key

4. What is the purpose of a key?

    * A key uniquely identifies the item among it's siblings. React uses your keys to know what happened if you later insert, delete, or reorder the items.

## The Spread Operator

1. What is the spread operator?

    * The spread (...) syntax allows an iterable, such as an array or string, to be expanded in places where zero or more arguments (for function calls) or elements (for array literals) are expected. (directly from the reading)

2. List 4 things that the spread operator can do.

    * Replace apply()

    * Copying an array

    * Concatenate arrays

    * Copying and merging objects

3. Give an example of using the spread operator to combine two arrays.

    * let arr1 = [0, 1, 2];
    const arr2 = [3, 4, 5];

    arr1 = [...arr1, ...arr2];
    // arr1 is now [0, 1, 2, 3, 4, 5]
    (example from the reading)

4. Give an example of using the spread operator to add a new item to an array.

    * const isSummer = false;
    const fruits = ["apple", "banana", ...(isSummer ? ["watermelon"] : [])];
    // ['apple', 'banana']
    (example from the reading to conditionally add to the array)

5. Give an example of using the spread operator to combine two objects into one.

    * const obj1 = { foo: "bar", x: 42 };
    const obj2 = { bar: "baz", y: 13 };

    const mergedObj = { ...obj1, ...obj2 };
    // { foo: "bar", x: 42, bar: "baz", y: 13 }
    (example from the reading)

## How to Pass Functions Between Components

1. In the video, what is the first step that the developer does to pass functions between components?

    * Passed the function as a prop

2. In your own words, what does the handleClick function do?

    * It console logs the string "parent click"

3. How can you pass a method from a parent component into a child component?

    * create a function that takes a callback, pass it to child

4. How does the child component invoke a method that was passed to it from a parent component?

    * simply invoke the callback function that was passed just as you would invoke a regular function()