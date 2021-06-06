# Functions:



![](https://replit.com/@rawnaqaburumman/Reading-notes-7#Function1-300x154.png)
Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output.

## Defining functions:
## Function declarations:
A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

* The name of the function.
* A list of parameters to the function, enclosed in parentheses and separated by commas.
* The JavaScript statements that define the function, enclosed in curly brackets, {...}.


`function square(number) {
  return number * number;
}`

### Function expressions:
While the function declaration above is syntactically a statement, functions can also be created by a function expression.

`const square = function(number) { return number * number }
var x = square(4) // x gets the value 16`

Calling functions
Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.

Calling the function actually performs the specified actions with the indicated parameters.

`square(5);`