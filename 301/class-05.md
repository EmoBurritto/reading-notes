# Readings: Putting it all together

## React Docs - Thinking in React

always identify components first, as well as subcomponents 

its like creating which first, object or function 

if component grows, break down into subcomponents 

UI and data models, json, have similar archeticture breakdown; component heirarchy 

static version for the foundation and then interactive UI for the true REACT portion; more thinking less coding  

state is not use for static version of app 

prop use for static version of app, foundation 

where does state live: 

Identify every component that renders something based on that state.
Find a common owner component (a single component above all the components that need the state in the hierarchy).
Either the common owner or another component higher up in the hierarchy should own the state.
If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

(reference: https://reactjs.org/docs/thinking-in-react.html)

## Questions 

1. What is the single responsibility principle and how does it apply to components?

identify sole purpose, object vs function for component 

2. What does it mean to build a ‘static’ version of your application?

a non interactive app 

3. Once you have a static application, what do you need to add?

props

4. What are the three questions you can ask to determine if something is state?

Is it passed in from a parent via props? If so, it probably isn’t state.
Does it remain unchanged over time? If so, it probably isn’t state.
Can you compute it based on any other state or props in your component? If so, it isn’t state.

5. How can you identify where state needs to live?

Identify every component that renders something based on that state.
Find a common owner component (a single component above all the components that need the state in the hierarchy).
Either the common owner or another component higher up in the hierarchy should own the state.
If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Higher-Order Functions

Functions that operate on other functions, either by taking them as arguments or by returning them

Higher-order functions allow us to abstract over actions, not just values

(reference: https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

## Questions

1. What is a “higher-order function”?

Functions that operate on other functions, either by taking them as arguments or by returning them,

2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

return parameter m that is greater than parameter n 

3. Explain how either map or reduce operates, with regards to higher-order functions.

map is a higher order function since it takes in other methods, functions, of an object to get a more clear value with an a more concise action 

## Things I want to Know more about 
- the first article is better to understand state vs prop 
- whats the best example of a fully fleshed out static app? besides gallery of horns another real life example 
- the three questions of is it state vs prop should be taught day one 
- what are some higher order function examples in gallery of horns, woudld it be what we mapped when searching the data for a specific horn beast?