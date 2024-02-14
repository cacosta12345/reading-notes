# Reading Notes Class 1

Why this is important?

Before learning to code with more advanced languages like JavaScript, Python, or C#, it is important to first know the basic building blocks of code and how websites operate. HTML is that building block. HTML is how websites display your code on the browser for users to seee and interact with.

## Getting Started

1. Compose a short poem describing how HTTP sends data between computers

    * A client requests,
    A working server responds,
    I toil in-between

    ***a haiku by chris***

2. Describe how HTML, CSS, and JS files are parsed in the browser.

    * The browser parses the HTML file first, and that leads to the browser recognizing any <link>-element references to external CSS stylesheets and any <script>-element references to scripts.
    * As the browser parses the HTML, it sends requests back to the server for any CSS files it has found from <link> elements, and any JavaScript files it has found from <script> elements, and from those, then parses the CSS and JavaScript.
    *The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and compiles and executes the parsed JavaScript.
    * As the browser builds the DOM tree and applies the styles from the CSSOM tree and executes the JavaScript, a visual representation of the page is painted to the screen, and the user sees the page content and can begin to interact with it.

    (credit: https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works  ***How the web works***)

3. How can you find images to add to a website? 

    * You can search google images, and save image as on your desktop. Note, most images are copyrighted. To avoid violating copyright, use Google license filter, and choose ***Creative Commons licenses***.

4. How do you create a String vs a Number in JavaScript?

    * a string in put between quotation marks "". Example: let name = "chris"
    * a number is typed without quotes. Example: let age = 30
    * note: a number put between quotes will make it a data type string

5. What is a variable and why are they important in JavaScript?

    * Variables are containers that store values. The variable could then be used multiple times wherever needed and could also be reassigned or "emptied" whenever needed.

## Intro to HTML

1. What is an HTML attribute?

    * attributes contain extra info about the element that won't appear in the content.

2. Describe the anatomy of an HTML element.

    * the anatomy of an HTML element consists of 3 man parts; Opening tag, Content, and Closing tag

3. What is the difference between <article> and <section> element tags?

    * article is used to define a self-contained, independant piece of content that makes sense on it's own. Whereas section is used to group related content and cannot stand on it's own.

4. What elements does a typical website include?

    * a typical website can include:
        1. header - <header>
        2. navigation bar - <nav>
        3. main content - <main>, <article>, <section>, <div>
        4. sidebar - <aside>; often placed in <main>
        5. footer - <footer>

5. How does the metadata influence Search Engine optimization?

    * Web browsers use information contained in the head to render HTML document correctly. Info in the meta tags in the head can then be used for search enging results.

    Note: Meta tags often aren't used anymore. Spammers were just filling the keyword lists with hundreds of keywords, biasing results.

6. How is the meta tag used when specifying metadata?

    * Meta tags are HTML elements used to specify metadata about a web page. They provide information about the page to browsers and search engines. The most common use of meta tags is to provide information like the page's title, character encoding, and a brief description.

    (chatgpt helped me answer this)

## Miscellaneous

### How to start to design a Website

1. What is the first step to designing a Website?

    * Answer the following questions:

    What exactly do I want to accomplish?

    How will a website help me reach my goals?

    What needs to be done, and in what order, to reach my goals?

2. What is the most important question to answer when designing a Website?

    * What exactly do I want to accomplish?

### Semantics

1. Why should you use an h1 element over a span element to display a top level heading?

    * By default, most browsers will style an h1 with a large font size to make it look like a heading. You can style a span tag with attributes to make it appear like a heading but it has no semantic value, so it will not get the extra benefits of default browser user agent stylesheets.

2. What are the benefits of using semantic tags in our HTML?

    * Some of the benefits from writing semantic markup are as follows:

    1. Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)
    2. Screen readers can use it as a signpost to help visually impaired users navigate a page
    3. Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes
    4. Suggests to the developer the type of data that will be populated
    5. Semantic naming mirrors proper custom element/component naming

    (credit: https://developer.mozilla.org/en-US/docs/Glossary/Semantics ***Semantics in HTML***)

### What is JavaScript?

1. Describe 2 things that require JavaScript in the Browser?

    * Form validation and dynamic web content

    (answered by chatgpt)

2. How can you add JavaScript to an HTML document?

    * JavaScript is applied to your HTML page in a similar manner to CSS. Whereas CSS uses <link> elements to apply external stylesheets and <style> elements to apply internal stylesheets to HTML, JavaScript only needs one friend in the world of HTML — the <script> element.

    (credit: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript ***How do you add JavaScript to your page?*** )