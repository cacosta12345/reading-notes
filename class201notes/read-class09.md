# Reading-Notes Class 9

## HTML Forms - How to structure a web form

1. Why are forms so important in web development?

    * Forms are one the main points of interaction between a user and a website.

2. When designing a form, what are some key things to keep in mind when it comes to user experience?

    * Prioritize scannability and readability

    * If the form is long, dont expose everything be default.

    * Single column layout works best

3. List 5 form elements and explain their importance.

    * label- represents a caption for an item in a user interface

    * input -  on the imput element the most important attribute is the type attribute. This attribute is extremely important because it defines the way the input element appears and behaves.

    * button - allows the user to send, or "submit", their data once they have filled out the form

## Learn JS - Intro to Events

1. How would you describe events to a non-technical friend?

    * an event is any action that happens in a browser. For example, a click, an error, the web page finished loading. Almost anything can be an event in a browser. When you move the mouse cursor, interacting with the keyboard. Anything

2. When using the addEventListener() method, what 2 arguments will you need to provide?

    * the event  for example: ("click") or ("hover")

    * the onclick function, or the function that will fire once the event is initialized

3. Describe the event object. Why is the target withing the event useful?

    * the event object describes the event in question, like click, mouse movement, keyboard input. 

    * you need the event object to write your onEvent function to do whatever it is you wanted to do on that event. Like prevent default behavior, redirect to somewhere else, change display etc...