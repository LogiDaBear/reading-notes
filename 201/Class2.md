# Reading Notes: Basics of HTML, CSS & JS

This topic matters because it is a refresher of the foundations of coding and the beginning of the 201 journey.

### HTML Questions

[HTMLTextFundamentals](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals)

[HTMLAdvancedTextFormatting](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting)

1. Why is it important to use semantic elements in our HTML?

It is important to use semantics because they give meaning to the element and its function can be easily identified.

2. How many levels of headings are there in HTML?

There are 6 levels of headings in HTML. H1 being the highest and H6 the lowest.

3. What are some uses for the sup and sub elements?

sup- superscript and sub- subscript
These are used for dates, formulas and math equations so that they are displayed correctly. Example from HTMLAdvancedTextFormatting:
    <p>My birthday is on the 25<sup>th</sup> of May 2001.</p>
    <p>
  Caffeine's chemical formula is
  C<sub>8</sub>H<sub>10</sub>N<sub>4</sub>O<sub>2</sub>.
    </p>
    <p>If x<sup>2</sup> is 9, x must equal 3 or -3.</p>


4. When using the abbr element, what attribute must be added to provide the full expansion of the term?

The attribute, title, must be used to give the full expansion of the term.

### CSS Questions

[HowCSSisStructured](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured)

1. What are ways we can apply CSS to our HTML?

- We can apply it with an external stylesheet (a .css doc) which will require an href.
- With an internal stylesheet that resides in the HTML doc itself
- Finally, with inline styles which should be AVOIDED when possible. These are declarations that affect a single HTML element.

2. Why should we avoid using inline styles?

It makes it harder to do maintenance on the CSS, rather than changing an element you have to find that specific part in the code. Keeping code and content makes it easier for everyone involved. Inline styles affect one element and are the end all be all.

3. Review the block of code:
       h2 {
     color: black;
     padding: 5px;
        }
  1. What is representing the selector?
  h2 is the selector.

  2. Which components are the CSS declarations?
  the content within the {} are the CSS declarations.

  3. Which components are considered properties?
  color and padding are the properties.

### JS Questions

[JavaScriptBasics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)

1. What data type is a sequence of text enclosed in single quote marks?

A string

2. List 4 types of JavaScript operators.

Assignment-=
Strict equality-===
Not (will return the opposite), Does not equal(will test if values are not equal- !, !==

3. Describe a real world Problem you could solve with a Function.

You could auto-fill in places on a form that hold the value of a function for someones name that was entered by user input or more a simple example would be to create a calculator.

[Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)

1. An if statement checks a __ and if it evaluates to ___, then the code block will execute.

condition ; true

2. What is the use of an else if?

To give more than just 2 outputs.

3. List 3 different types of comparison operators.

To test if values are identical === or not !==
Test a value is less than < or greater >
Test a value is less than or equal to <= and greater than or equal >= 

4. What is the difference between the logical operator && and ||?

The difference is && means AND which allows you to chain together expressions so that they all must be true to return true and || means OR and also chains but not all have to return true for true, just one or more. 

## Things I want to know more about

Switch statements and Objects (which I know are coming eventually). JavaScript in general I would like to know more about.