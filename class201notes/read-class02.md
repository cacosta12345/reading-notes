# Reading Notes Class 2

Why this is important?

HTML and JavaScript have loads of built in functionality. It is important to know which tags or operators to use to provide users with easy to use code that is both efficient and visually pleasing.

## Intro to HTML continued...

1. Why is it important to use semantic elements in our HTML?

    * Semantic elements are used in multiple ways, for example by search engines and screen readers. Semantics provide structure and accessibilty.

2. How many levels of heading are there in HTML?

    * 6

3. What are some uses for the sup and sub elements?

    * The sup and sub element should only be used for typographical reasons—that is, to change the position of the text to comply with typographical conventions or standards, rather than solely for presentation or appearance purposes.

    * sup could be used to display exponents

    * sub could be used for marking up footnote numbers


4. When using the abbr element, what attribute must be added to provide the full expansion of the term?

    * title attribute

## Learn CSS

1. What are ways we can apply CSS to our HTML?

    * External stylesheet
    * Internal sylesheet
    * Inline styles

2. Why should we avoid using inline styles?

    * First, it is the least efficient implementation of CSS for maintenance. One styling change might require multiple edits within a single web page. Second, inline CSS also mixes (CSS) presentational code with HTML and content, making everything more difficult to read and understand. Separating code and content makes maintenance easier for all who work on the website.

    (credit: https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured ***Inline Styles***)

3. Review the block of code below and answer the following questions:
    h2 { color: black};

    * What is the representing selector?

    - h2

    * Which components are the CSS declarations?

    - color: black

    * Which components are condidered properties?

    - color

## Learn JS

1. What data type is a sequence of text enclosed in a single quote marks?

    * string

2. List 4 typles of JavaScript operators.

    * addition +

    * assignment =

    * strict equality ===

    * not !

3. Describe a real world problem you could solve with a function.

    * If you needed to add sums you could write a function that takes variable with number values as parameters and have the function add said variable. Example function addNum(num1, num2, num3){let result= num1+ num2+ num3; return result;}

## Making Decisions in your Code- Conditionals

1. An if statement checks a __ and if it evaluates to ___, then the code black will execute

    * condition, true

2. What is the use of an else if?

    * If you wanted to provide more outcomes other than if and else. Else if would capture anything else that isn't covered by the if and else. 

3. List 3 different types of comparison operators

    * strict equality or not equal === !===

    * greater than less than > <

    * greater or equal and less or equal >= <=

4. What is the difference between the logical operator && and double pipe?

    * The double && means "and". Meaning both conditions have to be true for the code block to execute.

    * The double pipe means "or". Meaning if either conditions are true the code block will execute.