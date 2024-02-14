# Reading Notes Class 7

## Domain Modeling

1. Explain why we need domain modeling.

    * A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

## HTML Table Basics

1. Why should tables not be used for page layouts?

    * Layoout tables reduce the accessibility for visually impaired users

    * Tables produce tag soup

    * Tables are not automatically responsive

2. List and describe 3 different semantic HTML elements used in an HTML table.

    * table, td (table data), tr (table row)

## Introducing Constructors

1. What is a constructor and what are some advantages to using it?

    * In object-oriented programming, a constructor is a special method or function that is used to initialize an object when it is created. The primary purpose of a constructor is to ensure that an object is in a valid and usable state when it is first created.

    * Initialization: Constructors initialize the attributes or properties of an object with default values or values provided as arguments during object creation. This helps ensure that the object's data is set up correctly from the start.

    * Automatic Invocation: Constructors are automatically called when an object is created from a class, so you don't need to explicitly call them. This simplifies object creation and initialization.

    (chatGPT helped answer this)

2. How does the term this differ when used in an object literal versus when used in a constructor?

    * In an object literal, this, would refer to the object being defined. In a constructor, this, refers to the instance of the object that is being created by the "new" keyword.

## Object Prototypes Using A Constructor

1. Explain prototypes and inheritance via an analogy from your previous work experience.