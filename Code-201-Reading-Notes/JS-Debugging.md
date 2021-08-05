# JavaScript Debugging 
Debugging is the process of searching for (and fixing) errors in programming code.

## Error Objects
When we have an error in our code, the JavaScript console will display an error object, which can help us find our mistakes and our browser can help us read them. On the left of our JavaScript console it will display the error type along with the error message. On the right, we can find the name of the file, and the line number it occurred in.

**Error objects will consist of the following properties:**
* `name` - the *type* of error
* `message` - a description of the error
* `fileNumber` - the name of the JavaScript file
* `lineNumber` - the line where the error happened

**The seven built-in error objects in JavaScript include:**
* `Error` - generic error, which all other errors are based upon
* `SyntaxError` - proper syntax has not been followed
* `ReferenceError` - tried to reference a variable that is not declared/within scope
* `TypeError` - an unexpected data type that can not be coerced
* `RangeError`- numbers not in expected range
* `URIError` - `encodeURI()`, `decodeURI`, or similar methods used incorrectly
* `EvalError` - `eval()` function used incorrectly 

## Debugging Workflow
Debugging is a deduction process that involves eliminating the potential causes of an error. Here is a workflow we can follow when we are searching for errors:

#### *WHERE* IS THE PROBLEM? 
Here is how we can narrow down the area where the problem seems to be:

1. **Interpret the error message, it tells us:**
* The script that is causing the problem
* The line where it became a problem
* The type of error

2. **Check how far the script is running**
Use tools to write messages to the console so we can tell how far our script has executed.

3. **Use breakpoints where things are going wrong**
They let us pause execution and inspect the values that are stored in variables.

#### *WHAT* IS THE PROBLEM?
Here is how we can look for clues to find the *actual* line of code that is causing the error:

1. **Check the values of our variables around our breakpoints**
When we have set breakpoints, we can check the variables around them to see if they have the values we expect them to. *If not*, we need to look earlier in the script.

2. **Break down/break out parts of the code to test smaller pieces for functionality**
* Write values of variables into the console
* Call functions from the console to check if they return the expected results
* Check if objects exist and that they have the methods/properties that we think they do

3. **Check the number of parameters for a function, or the number of items in an array**



