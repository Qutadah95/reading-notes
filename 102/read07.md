# Expressions and operators

### Operators
JavaScript has the following types of operators. This section describes the operators and contains information about operator precedence.

- Assignment operators
- Comparison operators
- Arithmetic operators
- Bitwise operators
- Logical operators
- String operators
- Conditional (ternary) operator
- Comma operator
- Unary operators
- Relational operators

### Expressions

An expression is any valid unit of code that resolves to a value.

JavaScript has the following expression categories:

- Arithmetic: evaluates to a number, for example 3.14159. (Generally uses arithmetic operators.)
- String: evaluates to a character string, for example, "Fred" or "234". (Generally uses string operators.)
- Logical: evaluates to true or false. (Often involves logical operators.)
- Primary expressions: Basic keywords and general expressions in JavaScript.
- Left-hand-side expressions: Left values are the destination of an assignment.

#### Primary expressions
Basic keywords and general expressions in JavaScript.

this
Use the this keyword to refer to the current object. In general, this refers to the calling object in a method.

#### Grouping operator
The grouping operator ( ) controls the precedence of evaluation in expressions. For example, you can override multiplication and division first, then addition and subtraction to evaluate addition first.

#### Left-hand-side expressions
Left values are the destination of an assignment.

### Functions
Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.

#### Defining functions
A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

- The name of the function.
- A list of parameters to the function, enclosed in parentheses and separated by commas.
- The JavaScript statements that define the function, enclosed in curly brackets, {...}.

For example, the following code defines a simple function named square:

## function square(number) {
  ## return number * number;
## }

#### Calling functions
Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.

Calling the function actually performs the specified actions with the indicated parameters. For example, if you define the function square, you could call it as follows:

## square(5);


## Control flow

The control flow is the order in which the computer executes statements in a script.

Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops. 
