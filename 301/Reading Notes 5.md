# Reading Notes 5

## React Docs - Thinking in React
1. What is the single responsibility principle and how does it apply to components?
use the same techniques for deciding if you should create a new function or object. One such technique is the single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.
2. What does it mean to build a ‘static’ version of your application?
To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. Props are a way of passing data from parent to child. (If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.)
3. Once you have a static application, what do you need to add?
You can either build “top down” by starting with building the components higher up in the hierarchy (like FilterableProductTable) or “bottom up” by working from components lower down (like ProductRow). In simpler examples, it’s usually easier to go top-down, and on larger projects, it’s easier to go bottom-up.
4. What are the three questions you can ask to determine if something is state?
Does it remain unchanged over time? If so, it isn’t state.
Is it passed in from a parent via props? If so, it isn’t state.
Can you compute it based on existing state or props in your component? If so, it definitely isn’t state!
5. How can you identify where state needs to live?
The original list of products is passed in as props, so it’s not state.
The search text seems to be state since it changes over time and can’t be computed from anything.
The value of the checkbox seems to be state since it changes over time and can’t be computed from anything.
The filtered list of products isn’t state because it can be computed by taking the original list of products and filtering it according to the search text and value of the checkbox.

## Higher-Order Functions
1. What is a “higher-order function”?
Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions
2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
returning m if equal to or greater than m but only return if greater than n
3. Explain how either map or reduce operates, with regards to higher-order functions.
The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function.

## Things I want to know more about