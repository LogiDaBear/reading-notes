# Reading Notes for CSS Layout

## CSS Flexbox :muscle:

- [Flexbox](https://web.dev/learn/css/flexbox/)

1. Flexbox is designed for one-dimensional content. Explain what this means.
It takes the different sizes of items and returns them with the best layout for all items.

2. Explain the difference between the main axis and cross axis.

Three boxes next to each other with an arrow, pointing left to right. The arrow is labelled Main axis
Flex items move as a group on the main axis. 
![Alt text](https://web-dev.imgix.net/image/VbAJIREinuYvovrBzzvEyZOpw5w1/xKtf0cHRw0xQyiyYuuyz.svg)
The cross axis runs in the other direction to the main axis, so if flex-direction is row the cross axis runs along the column.
![Alt text](https://web-dev.imgix.net/image/VbAJIREinuYvovrBzzvEyZOpw5w1/5wCsZcBmK5L33LS7nOmP.svg)
Three boxes of different heights, next to each other with an arrow, pointing left to right. The arrow is labelled Main axis. There's another arrow pointing top to bottom. This one is labelled Cross axis
You can do two things on the cross axis. You can move the items individually or as a group, so they align against each other and the flex container. Also, if you have wrapped flex lines, you can treat those lines as a group to control how space is assigned to those lines. 

3. How can using certain properties of flexbox negatively impact accessibility?

It can re-order your visuals and misplace content

## CSS Flexbox :muscle: pt.II Layout

- [SwollBox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)

1. What are some advantages of using flexbox over float?
With flexbox things such as... 

- Vertically centering a block of content inside its parent.
- Making all the children of a container take up an equal amount of the available width/height, regardless of how much width/height is available.
- Making all columns in a multiple-column layout adopt the same height even if they contain a different amount of content.

...are all possible where the legacy float could not or would be very difficult to make happen.

2. How does this topic connect with your long term goals?
It makes me feel confident in the designing and placement when applying my CSS to make it look appealing especially when the floodgates of no longer having to use the reset.css become applicable. Oh sweet baby jesus. I understand the reasoining though, training wheels.

## Things I want to know more about
Is this applicable in every design scenario and how often does it misplace/rearrange the visuals with accessibility features? What circumstances would be better to use legacy methods?