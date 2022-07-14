# HTML Links, JS Functions, and Intro to CSS Layout

## Learn HTML

Creating hyperlinks are the way in HTML to open files such as images, audio and other multimedia functions. To insert a link it's best to use <a href="url">decription of page for user</a>. You can use Title <a> element of a hyperlink to describe when hovered over link what's about; like an attention grabber. You can use the <a> element with the URL to create a block level element in order to insert saved file  with alt message for user. Absolute URL is the actual url link versus relative URL is the file in its directory; file path. Same Directory is to show exact file to desired URL. Moving down into subdirectories is for showing the file and parent folder to show where to find URL. Link in CSS you can id the file by using document fragment in order to place url location in multiple elements; id in heading and actual URL in paragraph. Must use # to link id to URL location. Syntax is very important for the computer, user and some software liek screen reader to work properly.

(reference: https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)

## Questions

1. To create a basic link, we wrap text or other content inside what element?

- <a></a>

2. The href attribute contains what information?

- The URL

3. What are some ways we can ensure links on our pages are accessible to all readers?

- Add a title and alt attribute; when hovered description on site shown to user versus description in code for screen reader for people with disabilities.

## CSS Layout

Normal Flow is the way the webpage elements lay out as a default; best for computer to analyze CSS file. By removing and moving the location of elements in line, it could greatly affect the page as a whole; this is why normal flow is important. By default elements are in block level elements.  Inline elemnts are just the size of the content in the element. You can't affect height and width in an inline element since it's already formated due to the block level element. Block flow direction is the automatic layout of rendered content. The content will be layed out vertically by default. Inline elements are wrapped around the block element content. Margin collapsing is when the elemnt with the larger element will over ride and flow over the smaller margin. Positioning is greatly affected by coder; override normal document flow. Static positioning is a nothing atttribute since its just diplaying normal flow. Relative positioning starts in default flow but can be modified by affecting top, left, right bottom properties. Absolute position takes away normal flow function. Its stacked on other elements on a purposeful manner. You do this to add Ui to your page to not affect he page as a whole.  Initial containing block has no dimensions of viewport, site; when element has no ancestor element. Z-index affects z-axis; the stacking order. Z-axis is teh imaginary of user to screen interaction. Use small increments for z-axis. Fixed positioning fixed is static to nearest view point not positioned ancestor. use top: 0 to fix element at top of screen. Sticky is a hybrid like relative and fixed; scrolls with page for a bit and then fixed. 

(reference: https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning)
(reference: https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow)

## Questions 

1. What is meant by “normal flow”?

- The defualt layout of a site in way the elements are displayed. 

2. What are a few differences between block-level and inline elements?

- Block-level: default setting on site by computer, displayed through element block flow direction, one on top of the other vertically

- Inline: size depended on element its in, can't affect height and width

3. ___ positioning is the default for every html element.

- static

4. Name a few advantages to using absolute positioning on an element.

- not default flow
- can be used for UI purposes and not affect site flow, like pop ups

5. What is a key difference between fixed positioning and absolute positioning?

Fixed positioning is fixed static to nearest view point not positioned ancestor; it'll move and then move by a lot or a little to nearest element.

## Learn JS

Functions can be reused with short command; it's a reusable code. Anytime you make () it's a function; like for loop, while or do...while, if..else. Invoke means execute. Functions are part of methods; object. You can call functiosn from other functions. Math.random will make computer chose a number randomly from 0 to 1 by default or 0 to whatever number you declare. Invoke a function by declaring it in code {}. replace() function needs two strings for it to work; main and subset. = invokes default parameter. A function with no name is called an anonymous function; function(), doen when function expects peramter in code eventually. addEventListener() is when you want to run code when user interacts with text box and expect code to run; expects two or more perameters. function(event) is the same as (event) => . If function has only one line of code or one peramter no curly bracket more than oen needs curly bracket. map() to double every value in original array. Scope is compartments. 

## Questions

1. Describe the difference between a function declaration and a function invocation.

- Function declaration: define function 

- Function invocation: execute function 

2. What is the difference between a parameter and an argument?

- Parameter: optional, arrow functions, can be an array, can be recreated at any time, can be anonymous 

- Arguement: mandatory, non arrow functions; arguement object not an array, passed down from previous arguemnts 

## Things I want to know more about

- I am still completely lost on the last two questions for lab 03; js is my kryptonite 
- I feel a lot better about CSS and HTML
- is there common dimensions to center page besides auto?
- what's a real life example of a sticky positioning?
- join()? need clarification 