# Reading Notes for Problem Domain, Objects, and the DOM

## Java-Script Object Basics

- [JSObjectBasics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

1. How would you describe an object to a non-technical friend you grew up with?
A storage container for tools you want to use for later

2. What are some advantages to creating object literals?
Shorter syntax, transferring series of structured related data items (one object rather than several)

3. How do objects differ from arrays?
An array is one container of information with placeholders in numerical order where an object is a collection of data and functionality that has several uses besides just storing data.

4. Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.
If an objects property name is in a variable then you can't access it with dot notation

5. Evaluate the code below. What does the term `this` refer to and what is the advantage to using `this`?

`This` refers to the const dog and the advantage is that it can be used for anything within that object without having to re-write code.

        const dog = {
      name: 'Spot',
      age: 2,
      color: 'white with black spots',
      humanAge: function (){
        console.log(`${this.name} is ${this.age*7} in human years`);
      }
    }

## Le DOM
- [IntroductionToLeDOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

1. What is the DOM?
Document Object Model is a programming interface for web documents in which it represents the page so that programs can change the structure, style and content. FTW.

2. Briefly describe the relationship between the DOM and JavaScript.
Without the DOM, JS would not have any model of web pages, HTML, SVG and their counterparts. They are like lamb and tuna fish.

## Things I want to know more about
Can you create an object by using DOM by using an object... object-ception..