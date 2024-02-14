# Reading Notes Class 3

Why is this important?

Lists and CSS provide users with clean accessible content that is easy to digest. Conditionals and loops are very importand to make code efficient and save time and space. Longer code is expensive code.

## Ordered and Unordered lists

1. When should you use an unordered list in your HTML document?

    * When the order of the list items don't matter and can be displayed in any order without changing the meaning

2. How do you change the bullet style of unordered list items?

    * Using CSS you can change using list-style-type

3. When should you use an ordered list vs an unorder list in your HTML document?

    * When the order is meaningful, you would use an ordered list. For example, steps to a recipe, turn-by-turn directions, lists of ingredients. Otherwise, an unordered list can be used if order does not matter

4. Describe two ways you can change the numbers on list items provided by an ordered list?

    * a for lowercase letters

    * A for uppercase letters

    * i for lowercase Roman numerals

    * I for uppercase Roman numerals

    * 1 for numbers (default)

## Learn CSS - The box model

1. Descrbie the CSS properties of margin and padding as characters in a story. What is their role in the story titled: The Box Model?

    * The padding sits around the content as white space; size it using padding and related properties.

    * The margin is the outermost layer, wrapping the content, padding, and border as whitespace between this box and other elements; size it using margin and related properties.

2. List and describe the four parts of an HTML elements box referred to by the box model

    * Content box: The area where your content is displayed; size it using properties like inline-size and block-size or width and height.
    * Padding box: The padding sits around the content as white space; size it using padding and related properties.
    * Border box: The border box wraps the content and any padding; size it using border and related properties.
    * Margin box: The margin is the outermost layer, wrapping the content, padding, and border as whitespace between this box and other elements; size it using margin and related properties.

    (credit: https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model#the_box_model_and_inline_boxes ***Parts of a box***)

### Learn JS - Arrays, Operators and Expressions, Conditionals, Loops

1. What data types could you store in an array?

    * Numbers, strings, booleans, objects, arrays, functions, null, symbols, dates, custom objects, mixed data types

2. Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?

    * Yes, you can access it using it's location in the list. Index starts at 0 so first item is 0, second is 1 so on and so forth. Use bracket notation myArray[ 2 ]. In this case it would target the third item in the array

3. List five shorthand operators for assignment in JavaScript and describe what they do

    * Addition assignment  x += f() -----> x = x + f()

    * Subraction assignment x -= f() -----> x = x - f()

    * Division assignment x /= f() -----> x = x / f()

    * Remainder assignment x %= f() ------> x = x % f()

4. Read the code below and evaluate the last expression and explain what the result would be and why.

    let a=10; let b='dog'; let c= false ----- evaluate (a+c)+b;

    * '10dog'

    * There are different data types being added. Because b is a string it would concatenate the answer into one string

5. Describe real world example of when a conditional statement should be used in a JavaScript program.

    * In a website, if you need the user to input a number that you would write a conditional statement to verify it's type number and reject anything else

6. Give an example of when a loop is useful in JavaScript

    * Anytime you would need to go through every member of an array. In an array of Names, you might need to loop through all and take out the ones that start with "A".