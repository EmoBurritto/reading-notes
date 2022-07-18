# Problem Domain, Objects, and the DOM

## JavaScript Object Basics

An object is a collection of related data and/or functionality. These usually consist of several variables and functions (which are called properties and methods when they are inside objects)

To create an object you must first define and initialize a variable

You can rename the original object with defining and initializing a new varible; there can be multiple

You can also add new peoperties to further define original variable; user name, age, etc

Dot notation is naming the object followewd by a period with the corresponding property of the namespace; variable. attribute()

You can do an dditional dot with the type of property object used to further find  and isolate a particular object in a line of code; variable.object.specific variable object

Do not use array  numeric when trying to use dot notation on a object; variable['specific variable object'] ; associating array

This keyword is used when reffeering a specific function, or response to a certain variable; for object liteals

To use this method for mmultiple objects in a varaible use constructors

Construction is like a combination of inline function codes except you can add a new fucntion to call a new object; use this or add new to new object to be used as a constructor  

(reference: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

## Questions

1. How would you describe an object to a non-technical friend you grew up with?

A grouping of similar like things mixed with actions for them to be executed in a group of code.   

2. What are some advantages to creating object literals?

An advantage would be to add properties for the object to better define original variable. 

3. How do objects differ from arrays?

No index in objects.

4. Give an example for when you would need to use bracket notation to access an object’s property 

Objects are similar like objects and repeated or added while array is just a list of similar objects in a single ine of code identified with brackets.

5. Evaluate the code below. What does the term this refer to and what is the advantage to using this?
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}

The this keyword makes the name variable by affected to the function log code in this line of code. If you wanted to add another dog you would rewrite the code tailering to another user's respose, or dog in this instance. 

## Introduction to the DOM

The Document Object Model (DOM) is the data representation of the objects that comprise the structure and content of a document on the web

DOM is referred by data taypes:

- Document: root document

- Node: objects in document

- Element: specific element or node in document

- NodeList: arroy of elements in document 

- Attr: applies to specific object refernce in document

- NamedNodemap: array accessed by index or element in document


(reference: https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)
# Questions 

1. What is the DOM?

The programming language that dictates the content and objects of a site; can be affected by nodes and objects

2. Briefly describe the relationship between the DOM and JavaScript.

Dom is the content on the site while js is the programming laguage affecting the behavior of the site's content. 

## Things I want to know more about
- using object gettinf in running code 
- how to correctly code running code 
- clarification on new and this constructors 
- clarifcatin on intefaces and classes on a DOM
