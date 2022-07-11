# Getting Started

## Getting Started with the Web

Installing basic software is first step for tool using. Ubuntu comes with gedit by default for txt editor Examples of tools used are: 

-	A Computer (Windows, Linux)

-	A text editor (VS Code)

-	Web browser (Chrome)

-	Graphics editor (Photoshop)

-	Version Control System (Github)

-	FTP program, file manager (Git)

- Automation System, running tests (Webpack)
(reference: https://developer.mozilla.org/enUS/docs/Learn/Getting_started_with_the_web/Installing_basic_software)

Website design important like we did on 102; wire frame. 

Centralize folder for web projects; capitalization important, never put a space in title. Hyphens are better than underscores computer recognition.

Structure for website include:

- Index.html

- Image folder

- Styles folder

- Script folder

(reference: https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/Dealing_with_files )

HTML is a markup language, structure of a house. Consist of element, opening and closing tag and attribute to make up the element.  

There can be an empty element like when using a script for javascript or image in CSS.

CSS is a style language, the decorations of the house.  

-	It has a selector and declaration, consisting of property and property value.

Selectors can be:

-	ID , strictly applies to one element 

-	Class, multiple image on different elements  

-	Attribute, like an image on a page

-	Pseudo- class, specific element(s) like a cursor over a link  

(reference: 
https://developer.mozilla.org/enUS/docs/Learn/Getting_started_with_the_web/CSS_basics )

You can change font style and color to specific element.

Boxing and spacing is key.

Box model consists of:

-	Padding, space around text  

-	Border , solid line outside padding

-	Margin , space around border

(reference:https://developer.mozilla.org/enUS/docs/Learn/Getting_started_with_the_web/CSS_basics )

Javascript is the programming language, behavior of the site, clothes don’t belong in the kitchen.

Script link insert in HTML key, in successfully adding javascript code to site.

Javascript consists of variables, comments, operators, conditionals, functions and when ready supercharging.

Variables stores value of code; most used by let, semicolon key in ending declaration of value.

-	String, sequence of text by using single quotes 

-	Number, numerical value using no single quote

-	Boolean, true/false event, special key words needing no use of single quote  

-	Array, multiple value in a single reference using commas, each comma has an automatic numeric value like 0, 1, 2 etc.

-	Object, can be anything, mostly used for url’s, images, a collection of properties

(reference: https://developer.mozilla.org/enUS/docs/Learn/Getting_started_with_the_web/JavaScript_basics )

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

(reference: https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics )

Supercharging is like when adding an image changer or personalized welcome message for the user.

(reference: https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics )

Null is absence of value

Publishing web site can be done by Github like in 102.  

Websites are access by a client, computer connected to wifi, requesting access to server, computer website lives, then responding back to client with asked site. 

Order of website uploading:

-	HTML 

-	DOM (Document Object Model) tree built from analyzed HTML

-	CSS

-	CSSOM (CSS Object Model) tree built from analyzed CSS in HTML

-	Javascript

-	Javascript Compilation from analyzed DOM in-memory tree

-	Browser builds tree

(Reference: https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works )

Websites names are actually a series of numbers, DNS, communicating to IP address, unique location of web address to make it user friendly.
## Questions

1. pose a short poem describing how HTTP sends data between computers.

A lost girl, the Client, is loking for her dad at Target.

She asks, requests, a Target worker, the Server, to help find her dad.

They talk in common tongue, HTTP, to get to the point and say shes lost and scared. 

The Target worker uses the intercome to find her dad, DNS, and to come to the front of the store at the help desk to find his little girl. 

The dad hears the intercome message and is found in the elctronics section looking at funko pops in G12, the IP address.

The dad franctically goes to the help desk seeing her brave little girl running to her and tells him to stop being weird and looking at funko pops.     
  
2. Describe how HTML, CSS, and JS files are “parsed” in the browser.

HTML files are analyzed through the DOM (Document Object Model) tree built from the analyzed HTML.

CSS files are analyzed through the CSSOM (CSS Object Model) tree built from the analyzed CSS link in HTML. 

Javascript files are analyzed through the Javascript Compilation from the analyzed DOM in-memory tree when the site is being populated.  

3. How can you find images to add to a Website?
You can use google images but if they are copy righted, most are, it is best to use google license filter and look for the creative common license option to prevent copyright violation. 

4. How do you create a String vs a Number in JavaScript?
String, sequence of text, is used by single quotes vs Number, numerical value, uses no single quote. 

5. What is a Variable and why are they important in JavaScript?
Variables stores value of code; most used by let, semicolon key in ending declaration of value. 

## Getting Started with HTML

HTML(Hypertext Markup Language) is a markup language that dictates the structure of a web page. 

Consists of elements, content and tags; opening and closing.

Nesting elements are elements inside another element; adding the strong element within an element creates a bold, and strong importance within that element. Make sure to open close tag a nesting element within the desired content, do not place at end of general starting element. 

Block elements are your basic main elements to create a visible block structure on a page and have a lot going on. 

Inline elements are not whole paragraphs and are used within block elements only. 

Empty elements do not follow the pattern of regular opening and closing tags, they are used to insert or embed something in the overall page like an image, link or script. 

Attributes contain extra information in and element but won’t appear as txt. The syntax for an attribute consists of: 

-	Space between element name

-	Attribute name followed by an equal sign

-	Attribute value with opening and closing quotes

(refernce: https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started )

Boolean attributes, an attribute written with no value; hold one value, same as name. 

You can use single or double quotes, just don’t mix and match, stay consistent throughout code. 

HTML comments can be written with <!—element --> to comment like in javascript the justification of code use. 

## HTML Document Structure

Basic Sections of a Document: 

-	Header 

-	Navigation Bar

-	Main Content 

-	Side Bar 

-	Footer 

Articles are used for block of related content that stands on its own like a single blog post. 

Section is for grouping multiple related sections that add function to the whole grouping like a mini map. 

Detail Elements:

main is for content unique to this page. Use main only once per page, and put it directly inside body. Ideally this shouldn't be nested within other elements.

article encloses a block of related content that makes sense on its own without the rest of the page (e.g., a single blog post).

section is similar to article, but it is more for grouping together a single part of the page that constitutes one single piece of functionality (e.g., a mini map, or a set of article headlines and summaries), or a theme. It's 
considered best practice to begin each section with a heading; also note that you can break articles up into different sections, or sections up into different articles, depending on the context.

aside contains content that is not directly related to the main content but can provide additional information indirectly related to it (glossary entries, author biography, related links, etc.).

header represents a group of introductory content. If it is a child of body it defines the global header of a webpage, but if it's a child of an article or section it defines a specific header for that section (try not to confuse this with titles and headings).

nav contains the main navigation functionality for the page. Secondary links, etc., would not go in the navigation.

footer represents a group of end content for a page.

(reference: https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure )

Non-semantic wrappers are for specific elements that will be affected by code like javascript and CSS; div, block, and span, inline.

Break line elements are used to separate txt in a paragraph; br, new paragraph, and hr, change in theme or drastic change in text. 


## Metadata in HTML

Head of an HTML document displayed on actual site, its on the tab. Can be linked to CSS to style and consists of metadata, fav icon for tab or description of document.  It’s usually very short and sweet. 

Use <title> to give heading to head. 

Meta data can affect language permission for user. 

Author and description can be added by meta data. 

Icons for site can be also be added by metadata. 

## Questions 

1. What is an HTML attribute?

It's extra information, like a class identifier for style information, for set element that won't be displayed as txt on the site. Syntax of an attribute is as followed:

-	Space between element name

-	Attribute name followed by an equal sign

-	Attribute value with opening and closing quotes 

2. Describe the Anatomy of an HTMl element.

An HTML element consists of the element with less than sign, element name and greater than sign surrounding it, opening tag. The content or txt of the element. Finally, the closing tag displayed by a less than sign, back slash, name of 

element and a greater than sign to close the element. 

3. What is the Difference between <article> and <section> element tags?

Articles are used for block of related content that stands on it's own when compared to the rest of the site; like a single blog post. While,  Sections are for grouping multiple related blocks that add function to the whole site; like a 

mini map. 

4. What Elements does a “typical” website include?

Basic Sections of a Document: 

-	Header 

-	Navigation Bar

-	Main Content 

-	Side Bar 

-	Footer 

5. How does metadata influence Search Engine Optimization?

The type of metadata, like javascript script or CSS links, infulence how the page will look like and act like when accessed by the user. Metadata is the information about the sites initial data on the site's behavior and display. It 

also helps the engine render the data to the user correctly. 

6. How is the <meta> HTML tag used when specifying metadata?

The syntax for the <meta> HTML tag is <meta metadata attribute= "content" >. 

## How to start to design a Website

Project ideation: 

- What exactly do I want to accomplish?

- How will a website help me reach my goals?

- What needs to be done, and in what order, to reach my goals?

(reference: https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Thinking_before_coding)

Project never start with technical side, keep it simple and clear. 

## Questions 

1. What is the first step to designing a Website?
Ask yourself what you want to accomplish; keep it short and sweeet, don't get technical. 
 
2. What is the most important question to answer when designing a Website?
What do you want to accomplish; keep clear and conscise goals in order to build site. 

## Semantics

Semantics is defined by the meaning of code; how and why. 

Some of the benefits from writing semantic markup are as follows:

-	Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)

-	Screen readers can use it as a signpost to help visually impaired users navigate a page

-	Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes

-	Suggests to the developer the type of data that will be populated

-	Semantic naming mirrors proper custom element/component naming

(reference: https://developer.mozilla.org/en-US/docs/Glossary/Semantics )

## Questions 

1. Why should you use an h1 element over a span element to display a top level heading?

h1 element is the default used by a browser in what will make the txt the biggest on a page and give the look of a header while the span element will make it look liek a header through rendering by the coder. 

2. What are the benefits of using semantic tags in our HTML?

It will provide the data of the site, the complete structure; only place the computer will pull it from. CSS will it give ht e look and Javascript the behavior. 
  
## What is JavaScript?

Java script will affect the behavior of a page; it’s a scripting language that enables you to create dynamically updating content, control multimedia, animate images, etc. 
(reference: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript )

Application Programming Interfaces (APIs) provide you with extra superpowers to use in your JavaScript code. Some are built in like: 

-	DOM API

-	Geolocation API

-	Canvas 
(reference: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript )

Internal JavaScript:

-	Embedded script in line with HTML element to affect only that HTML element. 

External JavaScript: 

-	Embedded script in HTML in head or first line of body to affect whole HTML document, coder preference when JavaScript wants to be prompted. 
  
## Questions 

1. Describe 2 things that require JavaScript in the Browser?

You must have the reference of the Javascript code and the function or act of the Javascript in order what to carry out for set reference. For example: 

const para = document.querySelector('p');

para.addEventListener('click', updateName);

function updateName() {
  const name = prompt('Enter a new name');
  para.textContent = `Player 1: ${name}`;
}

It must be in this order or else it will comeback as undefined. 

2. How can you add JavaScript to an HTML document?

Internal JavaScript:

-	Embedded script in line with HTML element to affect only that HTML element. All JavaScript code in HTML file. 

External JavaScript: 

-	Embedded script in HTML in head or first line of body to affect whole HTML document, coder preference when JavaScript wants to be prompted. Seperate file with all JavaScript code.

  
##  Things I want to know more about

- Markdown Semantics, I feel like there's a better way to set up notes; sometimes chracters are replaced mid paragraphed versusing having space for revisions 
- When doing ACP origin main gets messed up and directory filed is not pushed right; multiple origns are made 
- on VS code, someextensions don't save, all extensions downloaded from 102 are gone 
- VS code to ask git extension when workedin previous course 
- metadata terminology 
- JavaScript terminology, I still miss up the words and when new things are introduced my mind goes blank  