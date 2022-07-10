## Programming with JavaScript

## MDN Control Flow

*Control flow is the way the computer executes commands; statetments in a script*

conditionals and loops are the frequent commands given to a computer

conditional structure is a if...else command; like when a user forgets to fill something in

if (field==empty) {
    promptUser();
} else {
    submitForm();
}

scripts can be set up for when an event is occured, a command

order of execution matters 

most basic statement 

{
  statement_1;
  statement_2;
  ⋮
  statement_n;
}

block statemenst used with  (if, for, while)

while (x < 10) {
  x++;
}

true, false statement is a boolean

if (condition_1) {
  statement_1;
} else if (condition_2) {
  statement_2;
} else if (condition_n) {
  statement_n;
} else {
  statement_last;
}

don't do x=y for if..else statements
if (x = y) {
  /* statements here */
}
