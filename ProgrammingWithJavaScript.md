# Programming With JavaScript

## Expressions and Operators

JS Has the following type of operators:

* Assignment operators: Assigns a value to its left operand based on the value of it's right 
* Comparison operators: Compares it's operands and on whether the comparison is true ex: equal (==) not equal (!=_)
* Arithmetic operators: Takes numeric values (literals or variables) as their opperand and returns a single numeric value. ex- (+) addition (-) subtraction (*) multiplication and (/) division
* Bitwise operators: Treats their operands as a set of 32 bits (zeros and ones) rather than a decimal, hexidecimal, or octal numbers <br> ex- a & b returns a one in each bit position for which the corresponding bits of both operands are ones</br>
a | b returns a zero in each bit position for both th corresponding bits of both operands and zeros<br>
a ^ b returns a zero in each bit position position for which the corresponding bits are the same</br>
~ a inverts the bits of its operand
* Logical operators: Typically used with Boolean (logical) values; when they are they return a Boolean Value. However the && and || operators return the value of one of the specified operands. This means if the operators are used with non-Boolean values, they can return non-Boolean values.
* String operators: The operator (+)Concatenates two string values together, returning another string that is in union of the two operand strings<br>
ex:console.log('my ' + 'string'); // console logs the string "my string".</br>
* Conditional (ternary) operator: The only JS operator that takes three operands. The syntax is condition ? val1 : val2
if the condition is true, the operator has the value of val1, otherwise it has the value of val2. <br>
ex: var status = (age >=18) ? 'adult' : 'minor';</br> //This statement assigns the value "adult" to the variable status if age is eighteen or more. Otherwise, it assigns the value "minor" to status.
* Comma operator: Evaluates both of its operands and returns the value of the last operand. Primarily used for a for loop
 * Unary operator: Requires a single operand either before or after the operator
 * Relational operator: Compares its operands and returns a Boolean value based of whether the comparison is true

 ## Functions

 A function in JS is similar to a procedure-- a set of statements that performs a task or calculates a value 

 ### Function declarations
 A function declaration consists of:
 * The function keyword followed by--
 * The name of the function
 * A list of parameters to the function, enclosed in paranthesis and separated by commas
 * The JS statements that define the function enclosed in curly brackets

<br>ex: the following code defines a simple function named square
</br>
function square(number) {
  return number * number;
}

## JS Function Syntax

Control flow is the order in which the computer executes statements in a script. A JS function is executed when "something" invokes it

<br> ex: imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or if...else// 

if (field==empty) {
    promptUser();
} else {
    submitForm();
}

