## Dynamic web pages with JavaScript

## JS Intro Paragraph

## Input and Output in JS

## Variables

*4 Ways to Declare a JavaScript Variable:*
- Using var
- Using let
- Using const
- Using nothing

*Variables store values, like in algebra:*

**let x = 5;**
**let y = 6;**
**let z = x + y;**

*Use var when code is 1995 to 2015*

*Use let and const post 2015*

*const is the go to unless chnaging value of variable*

**const price1 = 5;
const price2 = 6;
let total = price1 + price2;**

*Identify variables with unique names, a must; case sensitive.*
- Names can contain letters, digits, underscores, and dollar signs.
- Names must begin with a letter
- Names can also begin with $ and _ (but we will not use it in this tutorial)
- Names are case sensitive (y and Y are different variables)
- Reserved words (like JavaScript keywords) cannot be used as names

* **=** is the assignment operator*

* **==** is teh equal to operator*

* Declare variable with **var** or **let** then assign value*
- <p id="demo"></p>

<script>
let carName = "Volvo";
document.getElementById("demo").innerHTML = carName;
</script>

**Declare variables at begginnig of script**

*seperate variables with **,** *
- let person = "John Doe",
  carName = "Volvo",
  price = 200;
  
**Re-declare variable, lose value!**
- var carName = "Volvo";
  var carName;

*You can use = and +*
- let x = 5 + 2 + 3;

**$ and _ treat as variables**

