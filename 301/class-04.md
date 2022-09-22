# Readings: React and Forms

## React Docs - Forms

controlled components the way to do forms in REACT

<input>, <textarea>, and <select> typically maintain their own state and update it based on user input

mutable state is typically kept in the state property of components, and only updated with setState()

combine the two by making the React state be the “single source of truth”

the value attribute is set on our form element, the displayed value will always be this.state.value, making the React state the source of truth

<input type ="file"> is an uncontrolled component in React

<textarea> element defines its text by its children in HTML, Ract its a value attribute 

<input type="text">, <textarea>, and <select> all work very similarly - they all accept a value attribute that you can use to implement a controlled component

(reference: https://reactjs.org/docs/forms.html)

## Questions 

1. What is a ‘Controlled Component’?

An input form element whose value is controlled by React

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

its live due to handleChange and handleSubmit

3. How do we target what the user is entering if we have an event handler on an input field?

handleChange runs on every keystroke to update the React state, the displayed value will update as the user types
## The Conditional (Ternary) Operator Explained


(reference: https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)
## Questions

condition ? value if true : value if false

1. The condition is what you’re actually testing. The result of your condition should be true or false or at least coerce to either boolean value.

2. A ? separates our conditional from our true value. Anything between the ? and the : is what is executed if the condition evaluates to true.

3. Finally a : colon. If your condition evaluates to false, any code after the colon is executed.

1. Why would we use a ternary operator?

to shorten if statements into one line of code 

2. Rewrite the following statement using a ternary statement:

if(x===y){
  console.log(true);
} else {
  console.log(false);
}

x==y ? 'True' : 'False'

## Things I want to Know more about 
- why change so many element defineition to values from html to REACT, like does it really work all the time 
- there are so many ways to code for user readibility, is there such thing as too much short hand like txting? lol jk stuff like that 