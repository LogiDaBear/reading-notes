# Reading Notes for Object-Oriented Programming, HTML Tables

## Domain Modeling

- [Domain_Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)

1. Explain why we need domain modeling: We need domain modeling because it makes our lives as developers easier by validating and verifying specific problems amongst numerous stakeholders.

## HTML Table Basics

- [HTML Table Basics](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)

1. Why should tables not be used for page layouts?
Tables are not automatically responsive, they produce a "tag soup" mmmm and the layout tables reduce accessibility.

2. List and describe 3 different semantic HTML elements used in an HTML `<table>`:
[scope](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/th#attr-scope)
`scope` - the `th` element defines a cell as header of a group of table cells.
[thead](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/thead)
`thead` - defines a set of rows defining the head of the columns of the table
[tbody](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/tbody)
`tbody` - encapsulates a set of table rows indicating that they comprise the body of the table

## Introducing Constructors

- [IntroducingConstructors](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors)

1. What is a constructor and what are some advantages to using it?
A constructor is a function called using the `new` keyword and when called it will...
   - create a new object
   - bind `this` to the new object, so you can refer to `this` in your constructor code
   - run the code in the constructor
   - return the new object.

2. How does the term `this` differ when used in an object literal versus when used in a constructor?
In an object literal `this` is used to create one object whereas in a constructor it can be used to create more than one object from a single object definition.

## Object Prototypes Using A Constructor

- [ObjectPrototypesUsingAConstructor](https://ui.dev/beginners-guide-to-javascript-prototype)

1. Explain prototypes and inheritance via an analogy from your previous work experience:
Prototype is a template cutout that was used for placing weldments on armored vehicles in the correct spot. Everyone used it and shared it. Inheritance is the weldment coming with the spot already cut due to the prototype properties being streamlined.

## Things I want to know more about