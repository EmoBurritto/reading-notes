# Forms and JS Events

## HTML Forms

forms are one of the main points of interaction between a user and a web site or application

forms allow user data to be stored and processed by the application or possibly used to immediately update the interface in someway for user  use

form controls is equal to widgets on an appplication

HTML forms aid in the overall structure of the form

controls can be single or multi-line text fields, dropdown boxes, buttons, checkboxes, or radio buttons, <input> elements

form validation helps visually impaired users

UX is user's experience point of view

<form>- formally defines the form; action is url where user data is sent, method is function used to send data, get or post

<label>- class id for js reasons, along with name of line

<input>- where you specify the type of data user will enter along with corresponding class ID for label and js reasons

<textarea>- multiline text field; needs closing tag

<button>- allows user data to be submitted to application; includes button type and txt describing button

(reference:https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form )
(reference: https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form)

## Questions

1. Why are forms so important in web development?

forms are one of the main points of interaction between a user and a web site or application;  allow user data to be stored and processed by the application or possibly used to immediately update the interface in someway for user  use

2. When designing a form, what are some key things to keep in mind when it comes to user experience?

keep it simple, keep the form user friendly and don't ask too much of the user

3. List 5 form elements and explain their importance.

<form>- formally defines the form; action is url where user data is sent, method is function used to send data, get or post

<label>- class id for js reasons, along with name of line

<input>- where you specify the type of data user will enter along with corresponding class ID for label and js reasons

<textarea>- multiline text field; needs closing tag

<button>- allows user data to be submitted to application; includes button type and txt describing button

to group similar wigets, use fieldset and legend for ease of use 

## Learn JS

Events are actions or occurrences that happen in the system you are programming, which the system tells you about so your code can react to them

event handler, used for user to react to event

event handler the same as event listener 

registering an event handler- code running in response to event being called 

addEventListener() function, we specify two parameters: the name of the event we want to register this handler for, and the code that comprises the handler function we want to run in response to it

removeEventListener()  to remove desired event 

In the capturing phase:

The browser checks to see if the element's outer-most ancestor (<html>) has a click event handler registered on it for the capturing phase, and runs it if so.
Then it moves on to the next element inside <html> and does the same thing, then the next one, and so on until it reaches the direct parent of the element that was actually clicked.
In the target phase:

The browser checks to see if the target property has an event handler for the click event registered on it, and runs it if so.
Then, if bubbles is true, it propagates the event to the direct parent of the clicked element, then the next one, and so on until it reaches the <html> element. Otherwise, if bubbles is false, it doesn't propagate the event to any ancestors of the target.
In the bubbling phase, the exact opposite of the capturing phase occurs:

The browser checks to see if the direct parent of the clicked element has a click event handler registered on it for the bubbling phase, and runs it if so.
Then it moves on to the next immediate ancestor element and does the same thing, then the next one, and so on until it reaches the <html> element.

(reference: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

## Questions

1. How would you describe events to a non-technical friend?

Events are like the desired cause and effect in life. When you turn the key in your ignition, the desired effect is the car engine turning and idling, ready to hit the road. 

2. When using the addEventListener() method, what 2 arguments will you need to provide?

the name of the event and a function to handle the event

3. Describe the event object. Why is the target within the event object useful?

its one of two arguements or parameters in an event handler function, it can specify where the event will happen by giving function a new name 

4. What is the difference between event bubbling and event capturing?

bubbling- when both parent and child element are affected by event  

capturing- moves through HTML element heirachy to see if event is applicable 

## Things I want to know more about
- how to properly use similar widgets with fieldset element 
- when to use multiple handlers for single event 
- when to use nesting events 