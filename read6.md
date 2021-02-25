## HOW MEMORY &VARIABLES WORK
Global variables use more memory. The browser has to remember them
for as long as the web page using them is loaded. Local variables are only
remembered during the period of time that a function is being executed. 


CREATING THE VARIABLES IN CODE
Each variable that you declare takes up memory.
The more variables a browser has to remember,
the more memory your script requires to run.
Scripts that require a lot of memory can perform
slower, which in turn makes your web page take
longer to respond to the user. 

NAMING COLLISIONS
You might think you would avoid naming collisions;
after all you know which variables you are using.
But many sites use scripts written by several people.
If an HTML page uses two JavaScript files, and both
have a global variable with the same name, it can
cause errors. Imagine a page using these two scripts:


### WHAT IS AN OBJECT? 
Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names. 
 ![](ssssss.PNG)


USING WHILE LOOPS 



This loop will continue to run
for as long as the condition in
the parentheses is true. That
condition is a counter indicating
that, as long as the variable
i remains less than 10, the
statements in the subsequent
code block should run. 

USI NG DO WHILE LOOPS 


The key difference between
a whi 1 e loop and a do whi 1 e
loop is that the statements in
the code block come before the
condition. This means that those
statements are run once whether
or not the condition is met. 

summary 

Conditional statements allow your code to make
decisions about what to do next.
Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>)
are used to compare two operands.
Logical operators allow you to combine more than one
set of comparison operators.
if ... else statements allow you to run one set of code
if a condition is true, and another if it is false.
switch statements allow you to compare a value
against possible outcomes (and also provides a default
option if none match).
Data types can be coerced from one type to another.
All values evaluate to either truthy or falsy.
There are three types of loop: for, while, and
do ... while. Each repeats a set of statements.


# document Object Model 
The Document Object Model (DOM) specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window.

THE DOM TREE IS A
MODEL OF A WEB PAGE

As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.
It consists of four main types of nodes.



