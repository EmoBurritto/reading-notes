# HTML Lists, Control Flow with JS, and the CSS Box Model

## HTML

Can look through references section to further expand knowledge of HTML

(reference: https://developer.mozilla.org/en-US/docs/Web/HTML)

## Ordered and Unordered 

<ol> is the element for ordered list 

CSS Attributes to affect <ol> are:
- reversed: changes boolean attribute of list
- start: changes font style; use start="4" for roman numeral use
- type: changes numbering type; use type="i" for lowercase roman numerals

orded list: list order has meaning
- Steps in a recipe
- Turn-by-turn directions
- The list of ingredients in decreasing proportion on nutrition information labels

unordered list: list order with no numerical ordering and no meaning

nesting lists: use li then corresponding list element to nest <ol> or <ul>

(reference: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol)

(reference: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul )

## Questions 

1. When should you use an unordered list in your HTML document?

lists with no numerical ordering and list order has no meaning

2. How do you change the bullet style of unordered list items?

list-style-tye property in CSS

3. When should you use an ordered list vs an unorder list in your HTML document?

orded list - list order has meaning
unordered list- list order with no numerical ordering and no meaning

4. Describe two ways you can change the numbers on list items provided by an ordered list?

start: changes font style; use start="4" for roman numeral use
type: changes numbering type; use type="i" for lowercase roman numerals

## Learn CSS
 
Use CSS models to further expand learning base of CSS 

(refrences: https://developer.mozilla.org/en-US/docs/Learn/CSS)
## Box Model 

Two type of boxes:
- block boxes
- inline boxes

The boxes affect how content is displayed 

Boxes anatomy: 

- display type: inline will not break into new line
    - width and height not applied 
    - vertical padding, margins, and borders will apply but will not cause other inline boxes to move away from the box 
    - Horizontal padding, margins, and borders will apply and will cause other inline boxes to move away from the box

- outer display type: break onto new line
    - width and height applied 
    - Padding, margin and border will cause other elements to be pushed away from the box.
    - The box will extend in the inline direction to fill the space available in its container; the box will become as wide as its container, filling up 100% of the space available

<h1> and <p> use block as default

Box model: applies to block boxes; defines how the different parts of a box work together to create a box on a page

Parts of a box: 

Content box- space where text, images or any content of the page lives
Padding Box- the ether between the content and border
Border Box- wraps content and padding
Margin Box- outermost layer, wrappes context


(reference: https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)

## Questions

1. Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?

The Box Model: A Story about life

In  life there are things that effects us, whether we know it or not. We start with the individual, going day by day in life trying to make something happen; the Content. Although, We have our DNA like Width and Height, telling us how big or small we will be no matter what. Our inital interactions with the world in how we live it; the Padding. But as we have seen through trial and error, we are maintained by our physical limitations in how we interact with the world; our Border. As time has taught as, that doesn't stop the human spirit, we aspire for more and reach out to the ether for more; the Margin. Really we are all just trying to make it in this world; what have you done to make a difference?

2. List and describe the four parts of an HTML elements box as referred to by the box model.

Content box- space where text, images or any content of the page lives
Padding Box- the ether between the content and border
Border Box- wraps content and padding
Margin Box- outermost layer, wrappes context

## Learn JS

Refer models for further reading in models for more js concepts 

(reference: https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
## Arrays

Array: list liek object; multiple value store list

Different types of Arrays: 

- strings
- numbers
- objects

const random =: to implement different types of arrays in one list

First array is always 0, then follwoing numerical value due to how computer reads it

indexOf(): used to find certain array in list

push(): used to add array in list

unshift(): to add array at start of list

pop(): to remove last item in list 

shift(): to remove first item in list

splice(): removes specific array if known with indexOf use 

for..of: use all array

map(): used to commit same action to each array

filter(): used to only apply action to same tyoe of array that fit criteria

split(): to use only certain array for new action 

join(): opposite of split()

toString(): to conert array to string

(reference: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Arrays)
## Conditionals 

if...else: for boolean use; if this is good run that and vice versa

else if: used to chain more than one prompt for user

switch(): sine expression will always get one certain prompt 

(reference: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)
## Loops 

loops used to recreate code without having to write it out; can be as simple as just chnaging a single variable in a line of code to get different response

ypu can loop through a collection; array 

for...of: loop through an array

map(): appply action to complete array, has all original array 

filter(): apply action to certain array, only has new array that have been applied

for: to simply repeat code 
  - intializer: counter variable
  - condition: tells loop when to stop
  - final-expression: make loop false eventually

for..of: loop for certain condition 

break: stop loop for new code to run 

while: liek for loop but initializer variable set before loop; final-expression in loop

do..while: loop executed entirely at least once

(reference: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code)

# Questions 

1. What data types can you store inside of an Array?

Strings, numbers and objects

2. Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?
 const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];

No, it has to use the random array since its multideminsional; different data types.

3. List five shorthand operators for assignment in javascript and describe what they do.

x = f() it assigns value to variable by stating assignment operation is equal to the assigned value
x +- f() it assigns value to variable by adding value and to value to the right to result to true value
x -= f() it assigns value to variable by subtracting value and to value to the right  to result to true value
x *= f() it assigns value to variable by multiplying value and to value to the right  to result to true value

4. Read the code below and evaluate the last expression and explain what the result would be and why.

 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 
 (a + c) + b;

When I ran in replit, there is no value. This is due to being a random array. It needs const random = to be declared for it to work. In the shell it says ~/random$  

5. Describe a real world example of when a conditional statement should be used in a JavaScript program.

A complex example would be when someone is playing a video game and trying to decide what item to use. They can plug and play which item to use and see the stats increase or decrease accordingly. The game developer would code the conditional statement along eith many others to give value to each item.

6. Give an example of when a Loop is useful in JavaScript.

A loop would be useful in javascript when wanting to change one variable in a code in order to create different outcomes. For example, when attempting to look through a pdf file using the cntrl f feature on windows, you can filter through an exact term on the pdf file and click through until the user finds what they were looking for. 

## Things I want to know more about

- random arrays application
- is there a easier way to bloack elemenst around txt in page, there was a cdoncept in 102 that was taught that was a quick fixed but never work; float
- lost on ternary conditions 
- what's calculating squares 
- while vs do..while 