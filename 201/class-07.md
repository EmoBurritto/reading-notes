#  Object-Oriented Programming, HTML Tables

## Domain Modeling

Domain modeling is creating a conceptial model into code for a specific problem 

object-orientated model is storing data in properties and wraps functions

its a communication tool between developers to explain their code 

(reference: https://github.com/codefellows/domain_modeling#domain-modeling)
## Questions

1. Explain why we need domain modeling.

To turn spaghetti code into clean code ; use less code

# HTML Table Basics

A table is a structure set of data made up of rows and columns

table are user friendly and for readibility

Without CSS and prpoer HTML syntax, initial table is not user friendly and readble. 

tables should not be used for tabular data

CSS layouts fixed HTML basic structure of table

tag soup is a result of table used in HTML

tables use parent element default width in HTML

colspan: makes a cell span column; space for individual cell, data, inbetween text 

rowspan: makes cell span row; space for rows inbetween text

colgroup: defines CSS styling for columns; shorthand for all column style 

(reference: https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics )

## Questions

1. Why should tables not be used for page layouts?

Without CSS and prpoer HTML syntax, initial table is not user friendly and readble. 

2. List and describe 3 different semantic HTML elements used in an HTML <table>.

colspan: makes a cell span column; space for individual cell, data, inbetween text 

rowspan: makes cell span row; space for rows inbetween text

colgroup: defines CSS styling for columns; shorthand for all column style 

## Introducing Constructors

A function to group methods and objects; you can add, subtract multiple variables.

this refers to current object 

this refers to current object, can create multiple objects 

object literals create one object

when adding a new prpoerty update object 

an object hasa  prpoerty and a method

method is a function for objects 

using new will create a new object 

by binding this, you can refer to new object in constructor 

constructors start with capital letter 

constructors are named in relation to onject 

when using DOM, you use document as an object and accompainewd with a method, function 

(reference: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors)

## Questions

1. What is a constructor and what are some advantages to using it?

A function to group methods and objects; you can add, subtract multiple variables.

2. How does the term this differ when used in an object literal versus when used in a constructor?

this refers to current object, can create multiple objects 

## Object Prototypes Using A Constructor

Prototype is a property on a function that points to an object. 

Constructor function builds prototype. 

Every prototype has a function. 

You can add and share  methods to constructor function to look up methods for named variables. 

object.create delegates failed lookup to function prototype. 

must declare and return variable in order for prototype to work. 

use new to add new variable and string to use constructor function

when using new, add this to declaration of variable to avoid return and typical declaration

new is function declaration

new replaces object.create

js didn't have class keyword = new 

class keyword is like new 

to on failed lookups = get the prototype a variable will delegate too

used getPrototypeOf to get prototype of a variable 

for in loops going to loop over all of the enumerable properties on both the object itself as well as the prototype it delegates to

by default, any property you add to the functions prototype is enumerable

hasOwnProperty(key) = look specific property; lives on the objects prototype, use if function

arrow functions can be a constructor function; don't have prototype property 

=> arrow function

(reference: https://ui.dev/beginners-guide-to-javascript-prototype)

(reference: https://www.youtube.com/watch?v=XskMWBXNbp0)
#
# Questions 

1. Explain prototypes and inheritance via an analogy from your previous work experience.

NOTE: This is a very common front end developer interview question

Prototype is a property on a function that points to an object.

Inheritance is uaed to define a class and take functionality to a from parent class and allow to add more.

## Things I want to know more about 
- do I use STAR method top answer interview question correctly
- when to use arrow function 