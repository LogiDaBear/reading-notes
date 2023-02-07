# Reading Notes: HTML Lists, Control Flow with JS and the CSS Box Model

This topic matters as we are learning how to set-up our github repositories and apply everything we need within the terminal. It is adding on to our previous lessons and further cementing best practices.

## Learn HTML Questions

1. When should you use an unordered list in your HTML document?

ul should be used when there is no meaningful order, or if you are adding things to a category in no particular order. Also is a bulleted list.

2. How do you change the bullet style of unordered list items?

This can be changed in the CSS using the list-style-type property.

3. When should you use an ordered list vs an unorder list in your HTML document?

ol are more meaningful and should be used for specific instructions such as step-by-step, cooking, by decreasing or increasing numerical values.

4. Describe two ways you can change the numbers on list items provided by an ordered list?

You can add roman numerals to your list using the ol type="i" and then continue with your list. Example from [reading](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol#examples):
  
  <ol type="i">
  <li>Introduction</li>
  <li>List of Grievances</li>
  <li>Conclusion</li>
  </ol>

Or another way to change would be to create a nested list you would list another ol after the first part of the ol list. Example from [reading](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol#examples):
  
  <ol>
  <li>first item</li>
  <li>
    second item
    <!-- closing </li> tag is not here! -->
    <ol>
      <li>second item first subitem</li>
      <li>second item second subitem</li>
      <li>second item third subitem</li>
    </ol>
  </li>
  <!-- Here's the closing </li> tag -->
  <li>third item</li>
  </ol>




### Reading for HTML
- [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [OrderedLists](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol)
- [UnorderedLists](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)

## Learn CSS Questions

1. Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?

Margin is the cool Uncle that was always there on the side lines allowing you your space. Sometimes its negative and sometimes positive. Whatever you told him to do, he was your guy. A little unorthadox if you don't know what you're saying but there none the less. Almost an invisible guardian angel at any side you told them to be. Now this padding character.
Padding is the person that allows you to have space within a strict rule of equality. A real stickler for rules. You give them one value? Okay, all four sides are now that pal. Only two? Alright slim jim, first we have top and bottom values and then the sides. Three aye? Top is the first value, left and right side are second and bottom is the third. Four...okay okay, go clockwise starting at the top- in that order sucka. Dont even THINK about negatives because Padding aint havin it wise guy.

2. List and describe the four parts of an HTML elements box as referred to by the box model.

**Margin**
- The crust (yeah we're going earth with it). The outermost layer that wraps the other 3 elements and can be sized with the margin property
**Border**
- The mantle. Wraps content and padding. Sized with the semantic border.
**Padding**
- The Outer core. Surrounds your content with a white space. Sized with padding.
**Content**
- The Inner core. Where your stuff goes and is displayed. A colorful medley of size options such as: inline-size, block-size, width or height.


### Reading for CSS
- [BoxModel](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)

## Learn JS Questions

1. What data types can you store inside of an Array?

Lists of data items under the given variable - Single objects that contain multiple values but each value within can be accessed with just the variable name. 

2. Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?  
  
  const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];

Yes it is a valid array and you can access the array by calling the variable 'people' such as in a console.log(people);. Although it won't distinguish what are people- it will spew the entire list.

3. List five shorthand operators for assignment in javascript and describe what they do.

  Addition assignment	x += f()	          x = x + f()
  Subtraction assignment	x -= f()	      x = x - f()
  Multiplication assignment	x *= f()	    x = x * f()
  Division assignment	x /= f()	          x = x / f()
  Remainder assignment	x %= f()	        x = x % f()

These are mathematical shorthand operators that evaluate to the far right equation.

4. Read the code below and evaluate the last expression and explain what the result would be and why.  
  
 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;

The result would be 10dog because a number and string can't be added and c is just returning false which essentially means nothing here so 10 plus dog is..10dog.

5. Describe a real world example of when a conditional statement should be used in a JavaScript program.

Conditional statements should be used in the event of determining if code can execute or not and a real world example would be:

  let workDone = false;
  let planesFly;

  if (workDone === true){
    planesFly = 'flying';
  }else {
    planesFly = 'Flights Canceled';
  }

6. Give an example of when a Loop is useful in JavaScript.

From [loops](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code#why_are_loops_useful) a good example of a useful loop would be if you needed to draw 100 random circles on a canvas element! Tried it and it is fun! (I am also a simple man to please).

## Things I want to know more about
 
Who the cuss actually took the time to sit down and put this all to work in the way that they did. I understand it is a compilation of great coders stacking on-top of existing knowledge but I mean... What!?!

How would I go about creating a canvas element and making random circles like in the example in the reading except with different images and/or gifs? Code for reference to return to this:

    const btn = document.querySelector('button');
    const canvas = document.querySelector('canvas');
    const ctx = canvas.getContext('2d');

  document.addEventListener('DOMContentLoaded', () => {
    canvas.width = document.documentElement.clientWidth;
    canvas.height = document.documentElement.clientHeight;
  })

  function random(number) {
    return Math.floor(Math.random()*number);
  }

  function draw() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    for (let i = 0; i < 100; i++) {
      ctx.beginPath();
      ctx.fillStyle = 'rgba(255,0,0,0.5)';
      ctx.arc(random(canvas.width), random(canvas.height), random(50), 0, 2 * Math.PI);
      ctx.fill();
    }
  }

  btn.addEventListener('click',draw);
