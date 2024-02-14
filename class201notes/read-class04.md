# Reading Notes Class 4

## Learn HTML - Creating Hyperlinks

1. To create a basic link, we wrap text or other contents inside what element?

    * a tag

2. The href attribute contains what information?

    * contains the url of the link you want to provide

3. What are some ways we can ensure links on our pages are accessible to all readers?

    * Use clear link wording!

    * Create a navigation menu

## CSS Layout - Normal Flow CSS Layout: Postitioning

1. What is meant by normal flow?

    * By default, elements on a webpage lay out in normal flow if you haven't applied any CSS to change the way they behave.

2. What are a few differences between block-level and inline elements?

    * Display and Structure:

    Block-Level Elements: These elements create a "block" or a rectangular box in the document's layout. They typically start on a new line and occupy the full width of their parent container. Examples include div, p, h1, ul, and li.
    Inline Elements: Inline elements, on the other hand, do not create new lines, and they flow within the content. They only occupy the necessary width to display their content and don't force a new line. Examples include span, a, strong, and e.

    * Width and Height:

    Block-Level Elements: Block-level elements can have both width and height specified, making them suitable for creating structured layout elements like divs and sections.
    Inline Elements: Inline elements generally don't have a specified width and height; their size is determined by their content.

    * Margins and Padding:

    Block-Level Elements: Block-level elements can have margins and padding applied to them. This allows you to control the space around and within these elements.
    Inline Elements: Inline elements can have horizontal margins, but vertical margins often collapse, which means that the largest margin value among adjacent inline elements is used.

    * Nested Elements:

    Block-Level Elements: Block-level elements can contain both block-level and inline elements. You can nest other block-level elements within block-level elements.
    Inline Elements: Inline elements can contain only inline elements or text. They cannot contain block-level elements.

    * Examples of Use:

    Block-Level Elements: Block-level elements are commonly used to structure the layout of a webpage, such as dividing it into sections or columns. They are also used for paragraphs, headings, lists, and other content that should start on a new line.
    Inline Elements: Inline elements are used to apply formatting to text within a block-level element, like making text bold or italic, creating links, or adding inline images.

    * Default Behavior:

    Block-Level Elements: By default, block-level elements take up the entire available width of their parent container and start on a new line.
    Inline Elements: Inline elements flow within the content and do not start on a new line unless a line break is explicitly added.

    * (**ChatGPT helped answer this!**)

3. ___ positioning is the default for every HTML element

    * Static positioning

4. Name a few advantages to using absolute positioning on an element.

    * You can create isolated UI features that don't interfere with the layout of other elements on the page. For example, pop up boxes

    * Precise placement - because absolute positioning doesn't interfier with normal layout, you can specify anywhere on the page you want to display whatever it is you want to display

    * Useful for drag and drop interfaces or interactive components

5. What is the key difference between fixed positioning and absolute positioning?

    * With absolute positioning, elements are positioned realative to the nearest ancestor and moves with the site ie. when scrolling it scrolls with it. With fixed, the element stays static because it positions relative to the viewport.

## Learn JS - Functions- Reusable Blocks of Code

1. Describe the difference between a function declaration and a function invocation.

    * With function declaration, the function doesn't invoke when it's defined. You then have to call the function elsewhere for it to execute.

    * Function invocation is the act of executing the function by calling it my named variable. ie. myfunction()

2. What is the difference between a parameter and an argument?

    * the parameter is the variable placeholder in the function's declaration

    * the argument is the actual value of the parameters placeholder that the function needs to execute. If 2 parameters were num1 and num2 then the arguments would have to be values relative to the parameters so they could be something like (2, 4)

## Miscellaneous - 6 Reasons for Pair Programming

1. Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.

    * Greater efficiency - it's easier to catch mistakes. Research indicates that although pair programming takes slightly longer, it produces higher quality code.

    * Learning from fellow students - Developers have different ways to code. Although you may have learned one way to do things, in coding there is often many ways to acomplish the same problem. By using pair programming. You give yourself the opportunity to see how someone else codes and possibly learn new ways to make code more efficient.

## Notes

* I had not heard of the term pair programming before or see the benefits. I like the arguments it gave to the benefits of pair programming and would like to see it in action