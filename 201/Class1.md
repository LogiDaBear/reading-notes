# Reading Notes

## Why is this important?

These topics matter because this is essentially the foundation of learning how to code. Things learned here carry on into further and other languages. Maybe not directly but definitely by providing a solid understanding.

## An HTTP Poem

TCP? IP? No HTTP. But also all 3.
What does this mean to me.
Defining language for clients and servers,
first an address to dress the request called DNS.
A request sent to a server via me the client via an HTTP,
it will sail the interwebs with TCP/IP.
Server approval required for entry,
browser assembles chunks for a web pagey!

## HTML, CSS, and JS files parsed into browser; information regarding images, strings, numbers and variables.

### HTML, CSS, and JS files parsed into browser
- [Reading](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)

When requests are sent to servers they search the HTML files for link elements that reference CSS files and script elements that are JS scripts. 
Parsing is the step when a browser turns the data recieved over the network into the DOM and CSSOM which then is turned into a webpage.

- The [Order](https://developer.mozilla.org/en-US/docs/Web/Performance/How_browsers_work#parsing).

### information regarding images, strings, numbers and variables

In javascript in order to create a string you use ' or " around a word and it becomes a string. A number is created without using quotes.
Variables are declared using the 'let' keyword followed by whatever name you give said variable. Ex: let thisVariable; here the variable is thisVariable. Variables are important in JS because they allow us to call upon things previously stated and save time by not having to declare extra variables. They are essentially storage containers for values, whatever those values may be, could be a string, could be an equation, could be a loop... endless-ish possibilities.

- [Reading](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)

## HTML

- [Attributes](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started#attributes)

An attribute in HTML is extra information set within opening and closing tags. Attributes should contain the following:

    A space between it and the element name. (For an element with more than one attribute, the attributes should be separated by spaces too.)

    The attribute name, followed by an equal sign.

    An attribute value, wrapped with opening and closing quote marks.

The anatomy of an HTML element is an opening tag: p followed by the content, (all of this between the p tags) and then the closing tag /p.
From opening to closing tags is the element and the information in between is the content. Did I just repeat myself? Maybe.

The difference between article and section element tags:
article tags put a block of content that makes sense on its own by itself.
section tags are similar to article tags but help group things with individual functions- like a map or summary

Articles can contain section tags within them to help isolate certain parts.

Typical websites include AT LEAST the following elements...

    <!DOCTYPE html>
    <html lang="en-US">
    <head>
    <meta charset="utf-8" />
    <title>My test page</title>
    </head>
    <body>
    <p>This is my page</p>
    </body>
    </html>


- [Metadata](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML)

Metadata influences search engine optimization if you specify the content with keywords, which has the potential to make your page appear higher (like in a Google search) in relevance to whatever the keyword is. 

The [meta](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#metadata_the_meta_element) tag is used when specifying metadata in example from the following link and reading:
    <//meta
  name="description"
  content="The MDN Web Docs site
  provides information about Open Web technologies
  including HTML, CSS, and APIs for both Web sites and
  progressive web apps." />


When designing a website the first steps should be to answer what it is you want to accomplish and the goals you have for the website.

You should use an h1 element over a span element to display a top level heading because h1 is a block element where span is an inline element. Elements cannot be partially contained by other elements.

Semantic tags in HTML help the search engines determine importance and context of web pages, pages with semantic elements are much easier to read and have greater accessibility which offers a better user experience overall.

### JavaScript

2 things that are required for JS in the browser are HTML and CSS. The three make and build a complete website.

To add [JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript#how_do_you_add_javascript_to_your_page)to your webpage you can use internal, external, inline handlers.

## Things I want to know more about

I learned in 102 the specific orders of which is searched first as far as inline, external and internal with CSS but the order in which information is gathered and delivered first ex: which "chunk" will load first and the fastest?

Did M. Zuck rename FB based on Meta as the html tag or as in the gamer reference (most efficienct tactic available)? 

When meta tags are used, there are millions upon billions of websites out there and all probably use the same keywords. Can they pay to have their content placed higher?