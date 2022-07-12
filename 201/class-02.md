# Basics of HTML, CSS & JS

## HTML Text Fundamentals. 

Paragraphs wrapped by the <p> </p>

Headings are wrapped by the <h1> </h1>

- h1 can go on to h6 to make headings smaller
- h1 title of page
- h2 chapter
- h3 subsections

rule of thumb use no more than three heading types, stay in correct order, and h1 is at the top of page

Important to use headings and paragraphs to make it user friendly

Without headings SEO (Search Engine Optimization) will not run efficently and the computer won't output the page as the coder intended

Screen reader won't run effectively for user with no proper semantics

CSS and java script won't run effectively without the proper semantics

<span> </span> with inline CSS can make something look like h1, but that's extra unnecesary work and the SEO won't read it offically as a title

<ul> </ul>, <ol> </ol> for unorderd lists

<li> </li> for ordered list items

Nesting elemnts for list should go like this: 
<ol>
  <li>
    <ul>
      <li></li>
    </ul>
  </li>
</ol>

<em></em> to emophasis inline paragrapgh text

<span> with inline CSS to italize 

<strong></strong> to strongly show importance in line text in paragraph; bold. 

<b></b> and <span> with CSS to style better with bold 

<i> is used to convey a meaning traditionally conveyed by italic: foreign words, taxonomic designation, technical terms, a thought...
<b> is used to convey a meaning traditionally conveyed by bold: keywords, product names, lead sentence...
<u> is used to convey a meaning traditionally conveyed by underline: proper name, misspelling...

(reference: https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals)

## HTML Advanced Text Formatting

<dl> is description lists
  Wrapped with <dt> for description term 
  Also <dd> for description definition>

<blockqoute cite= "url"></blockqoute> for references 
  When using qoutes use <q></q>

<cite>text</cite> attribute helps underline and italize reference and easier for screen readers 

<abr title= "text"> abbreviation </abbr>
  The full abbreviation text will appear when hovered over abbreviation

<address> author details </address>

<sup> is used for super script in smaller front and is displayed in smaller front next to text; like dates

<sub> is used to define subscipt text; like chemical formulas
## Questions

Computer code elements: 

- <code>: For marking up generic pieces of computer code.

- <pre>: For retaining whitespace (generally code blocks) — if you use indentation or excess whitespace inside your text, browsers will ignore it and you will not see it on your rendered page. If you wrap the text in <pre></pre> tags however, your whitespace will be rendered identically to how you see it in your text editor.

- <var>: For specifically marking up variable names.

- <kbd>: For marking up keyboard (and other types of) input entered into the computer.

- <samp>: For marking up the output of a computer program.

<time datetime= "year-month-date numerically"> day month(alphabetical) year</time> used for time and dates 

<time datetime="19:30:01.856">19:30:01.856</time> used solely for time

<time datetime="2016-01-20T19:30+01:00">7.30pm, 20 January 2016 is 8.30pm in France</time> used for combination of date and time 
(reference: https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting)

## Questions

1. Why is it important to use semantic elements in our HTML?

The importance to use semantics is to make it user friendly. Without headings SEO  will not run efficently and the computer won't output the page as the coder intended. Also, screen reader won't run effectively for user with no proper semantics. Finally,  CSS and java script won't run effectively without the proper semantics either.

2. How many levels of headings are there in HTML?

There are 6 levels.

3. What are some uses for the <sup> </sup> and <sub> </sub> elements?

<sup> is used for super script in smaller front and is displayed in smaller front next to text; like dates.
<sub> is used to define subscipt text; like chemical formulas.

4. When using the <abbr> </abbr> element, what attribute must be added to provide the full expansion of the term?
The tile= "spelled out acronym" is used for abbreviations.

## How CSS Is Structured

External CSS has a <link rel= "stylesheet" href = "styles.css"> in the head 

Internal CSS has <style> CSS code in head; usefuel when you don't have access to external CSS file

Inline CSS has <element name style="CSS code;"> text </element name>; affect single element, avoid messes with SEO order flow

Class attribute is used when wanting to specify to a single element of code like in a paragraph 

Element attribute is to apply to all similar elements 

Class over rides element attribute 

Two basic components of CSS is property and value; color (property) : blue (value);
- also known as CSS declaration, found in CSS Declaration block 

Selector is element{}

Case sensitive, use : to seperate prpoerty and value 

calc() can bye used to do simple math within CSS 

Transform function, rotate(), can literally rotate image
- transform: rotate(numerical valueturn);

Short hand properties; font, background, padding, border and margin

padding order: top, right, bottom, left 

background order: color, image, position, repeat, attachment

To comment in CSS use /* text */
- good for testing CSS code

## Questions

1. What are ways we can apply CSS to our HTML?

External, Internal, Inline 

2. Why should we avoid using inline styles?

It affects the flow of the code, one CSS inline chnage affects the rest of the html file if done wrong; SEO can execute the order wrong and produce not desired site. It's also not coder friendly when working on a team, CSS and HTML code can get mixed up. 

3. Review the block of code below and answer the following questions:

  - What is representing the selector?
    h2
  - Which components are the CSS declarations?
    color: black;
    padding: 5px;
  - Which components are considered properties?
    color and padding

h2 {
     color: black;
     padding: 5px;
   }
  
##  JavaScript Basics
 Comments are used by two forward slashes and are automated from live code but used as the how and why for coders to justify code use.

Operators are a mathematical symbol that produce value of two variables.

-	Addition- combine two strings or numbers together using plus sign 

-	Subtraction, multiplication, division- used by minus sign, asterisk, and forward splash respectively to give numerical value to two or more values

-	Assignment- declares value of variable by using equal sign

-	Strict equality- test Boolean value using three equal signs

-	Not, Does-not-equal- opposite value of Boolean used by exclamation point outside parentheses of Boolean statement, or exclamation point followed by three equal signs 

(reference: https://developer.mozilla.org/enUS/docs/Learn/Getting_started_with_the_web/JavaScript_basics )

Conditionals are used to test if an expression is true or not, like the if ... else used in 102.

Functions are for repeated use of code.

Functions take arguments, the data inside parenthesis separated by commas if more than one.

Events are real time interactivity by a user on a site, like a click event.

## Questions

1. What data type is a sequence of text enclosed in single quote marks?

conditionals 

2. List 4 types of JavaScript operators.

addition, +, add two numerical values or combine two strings 
assignment, =, assigns value to variable  
strict equality, ===, true/false booleans occurs 
subtraction, -, subtraction of two numerical values

3. Describe a real world Problem you could solve with a Function.

When documenting on a patient at a hospital setting, the software can tell you if a value of a blood lab to check their white blood cells count is within range or not; resulting in prpoer care of patient.  
  
## Making Decisions In Your Code – Conditionals

Conditionals can be used like in video games when your health baar is 0 and thus results in game over. 

Decion making in JavaScript

if else statement:
- if (condition) {
  code ran if true
} else {
  run other code
}

if is true 

else is false

curly brackets are key

use else if for multiple choices 

Comparison operators:

- === and !== test if one value is identical to, or not identical to, another.
- < and > test if one value is less than or greater than another.
- <= and >= test if one value is less than or equal to, or greater than or equal to, another.

Any value that is not false, undefined, null, 0, NaN, or an empty string ('') actually returns true 

(refernce: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals )

use - for nesting conditional elements

logical operator: 
- && is and, makes both statements true 
- || is or, makes both statements run code to see if true
- ! is not, makes statement false

switch statement that runs through the code to give absolute response

ternary gives one response if true and other if false

## Questions

1. An if statement checks a __ and if it evaluates to ___, then the code block will execute.

condition, true

2. What is the use of an else if?

In order to give more than two responses to user. 

3. List 3 different types of comparison operators.

=== and !== value idenitcal or not
< and > value less than or greater than 
<= and >= value less than equal to or greater than equal too

4. What is the difference between the logical operator && and ||?

&& makes both or more expressions true 
|| check each expression if true

## Things I want to know more about
- when to use <address> element 
- is the <cite> element the way we are suppose to cite from now on
- when to properly used code elements
- when to use calc() function for CSS
- need clarification on @rules for CSS 
- now I see why /' was used thought it was a typo 
- more clarification on switch statements 
- more clarification on ternary statements 