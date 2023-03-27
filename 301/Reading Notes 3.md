# Passing Functions as Props

## Lists and keys
1. What does .map() return?
Given the code below, we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it:
2. If I want to loop through an array and display each value in JSX, how do I do that in React?
You can build collections of elements and include them in JSX using curly braces {}.

Below, we loop through the numbers array using the JavaScript map() function. We return a <li> element for each item. Finally, we assign the resulting array of elements to listItems:
3. Each list item needs a unique <ul>.
4. What is the purpose of a key?
A “key” is a special string attribute you need to include when creating lists of elements. We’ll discuss why it’s important in the next section.

## The Spread Operator
1. What is the spread operator?
InJavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.
2. List 4 things that the spread operator can do.
Copying an array
Concatenating or combining arrays
Using Math functions
Using an array as arguments
3. Give an example of using the spread operator to combine two arrays.

      const myArray = [`🤪`,`🐻`,`🎌`]
      const yourArray = [`🙂`,`🤗`,`🤩`]
      const ourArray = [...myArray,...yourArray]
      console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩
4. Give an example of using the spread operator to add a new item to an array.
        const fewFruit = ['🍏','🍊','🍌']
        const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
        console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]
5. Give an example of using the spread operator to combine two objects into one.
        const objectOne = {hello: "🤪"}
        const objectTwo = {world: "🐻"}
        const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
        console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
        const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
        objectFour.laugh() // 😂😂😂😂😂

## Pass Functions between Components
1. In the video, what is the first step that the developer does to pass functions between components?
They create the functions where the state is going to be changed; in between the constructor and render
2. In your own words, what does the increment function do?
It creates a function that will change the state
3. How can you pass a method from a parent component into a child component?
Create a function in the parent component that accepts a callback as an argument. Pass the function to the child component as a prop. In the child component, create the function you want to pass UP to the parent. Call the parent function prop in the child component with the child function as the argument.
4. How does the child component invoke a method that was passed to it from a parent component?
Use a combination of the useImperativeHandle hook with the forwardRef HOC.
Trigger the function using a useEffect hook inside the child.

## Things I want to know more about
