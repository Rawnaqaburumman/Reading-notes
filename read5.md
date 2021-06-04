# Operators:
### Types of operators:



1. **Assignment operators:** An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=).
`x = y`, `x += y`, `x -= y`.

2. **Comparison operators:** compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values.`var1 != 4 `, `3 == var1`, `var2 > var1`.

3. **Arithmetic operators:** takes numerical values (either literals or variables) as their operands and returns a single numerical value. `1 / 2` , `12 % 5`.

4. **Bitwise operators:** treats their operands as a set of 32 bits (zeros and ones), rather than as decimal, hexadecimal, or octal numbers. For example, the decimal number nine has a binary representation of 1001. `a & b` ,
`a ^ b` .

5. **Logical operators:** are typically used with Boolean (logical) values; when they are, they return a Boolean value. `expr1 && expr2 ` , `expr1 || expr2`.
6. **String operators:** the concatenation operator (+) concatenates two string values together, returning another string that is the union of the two operand strings.

7. **Conditional (ternary) operator:** takes three operands. The operator can have one of two values based on a conditionIf `condition` is true, the operator has the value of `val1`. Otherwise it has the value of `val2`.

8. **Comma operator:** evaluates both of its operands and returns the value of the last operand. This operator is primarily used inside a for loop, to allow multiple variables to be updated each time through the loop
9. **Unary operators:** A unary operation is an operation with only one operand.
10. **Relational operators:**A relational operator compares its operands and returns a Boolean value based on whether the comparison is true.
# Expressions:
An expression is any valid unit of code that resolves to a value.Every syntactically valid expression resolves to some value but conceptually, there are two types of expressions: with side effects (for example: those that assign value to a variable) and those that in some sense evaluate and therefore resolve to a value.
##### JavaScript has the following expression:
*  Primary expressions: Basic keywords and general expressions in JavaScript ex : `this` 
* Arithmetic: evaluates to a number,(Generally uses arithmetic operators.)
* String: evaluates to a character string,  (Generally uses string operators.)
* Logical: evaluates to true or false. (Often involves logical operators.)
* Primary expressions: Basic keywords and general expressions in JavaScript.
* Left-hand-side expressions: Left values are the destination of an assignment.

# Loops : 
Loops offer a quick and easy way to do something repeatedly.

### for statement: 
A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop.

`for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement.`


  ### while statement:
  A while statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:
  `while (condition)
  statement`.

