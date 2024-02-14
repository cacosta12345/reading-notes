# Reading Notes Class 5

## What is the purpose of CSS?

CSS is a language for specifying how documents are presented to users -- how they are styled, laid out, etc.

## What are the three ways to insert CSS into your project?

* External CSS - Can change the look of an entire website with one file. The html page must include a reference to the external style sheet file inside the <link> element, inside the head section.

* Internal CSS - May be used if one single HTML page has a unique style.
  The internal style is defined inside the <style> element, inside the head section.

* Inline CSS - May be used to apply a unique syle for a single element. To use, add style attribute to the relevant element. The style attribute can contain any CSS property.

## Write an example of a CSS rule that would give all <p> elements red text.

    <head>
        <style>
            p {
            color: red;
            }

        </style>

    </head>
