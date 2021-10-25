# Call Stack

## Reading #1:

1. What is a ‘call’?

*A 'call' is the act of invoking a function.*

2. How many ‘calls’ can happen at once?

*In JavaScript, only one call can happen at a time since it only has one call stack*    
    
3. What does LIFO mean?

*LIFO means Last In, First Out*

4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

![My-3D-Paint-Drawing-Of-A-Call-Stack](https://i.ibb.co/SsLnDq7/callstack.png)

5. What causes a Stack Overflow?

*A stack overflow is caused when there is a recursive function- a function that calls itself without an exit point*


*Reading Source:* [The-JavaScript-Call-Stack-What-It-Is-and-Why-It's-Necessary](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)


------------------------------------------------
# Error Messages 
## Reading #2"

1.  What is a ‘reference error’?

*A reference error is an error that occurs when you try to use a variable that is not yet declared.*

2. What is a ‘syntax error’?

*A syntax error is an error that occurs when you have something that cannot be parsed in terms of syntax like when you try to parse an invalid object using `JSON.parse`*
    
3. What is a ‘range error’?

*A range error is an error that occurs when you try to pass a value as an argument to a function that does not allow a range that includes the value*
    
4. What is a ‘type error’?

*A type error is an error that occurs when the data types you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.*
    
5. What is a breakpoint?

*A breakpoint is used in a debugger window in order to stop javascript from executing so you can examine the code, after examining the values you can resume execution.*

6. What does the word ‘debugger’ do in your code?

*The word debugger is used to reproduce the conditions in which the error has occurred, and then examine the program state at that time and identify the cause*

*Reading Source:* [JavaScript-error-messages-&&-debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)


-----------------------------------------------

## Things I would like to know more about:

* What makes a range error different from a type error? They seem very similar.

* In what instances it appropriate to use a *try catch*?