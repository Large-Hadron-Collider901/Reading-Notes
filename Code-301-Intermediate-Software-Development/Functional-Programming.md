
# Functional Programming 


## READING 
1. What is functional programming?

*Functional programming (FP) is a programming paradigm which is essentially the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects. Functional programming is declarative rather than imperative, and application state flows through pure functions. Contrast with object oriented programming, where application state is usually shared with methods in objects*
* *Some examples of functions that enable functional programming include:* <br />
`String.prototype.slice`, `Array.protoype.filter`, `Array.prototype.join`, `filter`, `map`, `reduce`, `concat`, *and* `Object.assign` .
<br />

* `const` is so a perfect declaration for functional programing since we wont be mutating data

* *Some examples of impure functions include:* <br />
`Array.prototype.forEach` *and* `Array.prototype.push`

2. What is a pure function and how do we know if something is a pure function?

*A pure function is a function which:*
* *Given the same inputs, always returns the same output and*
* *Has no side effects* 

*For example:* 
`console.log( double(5));` *is the same as* `console.log(10);`
*This is true because* `double()` *is a pure function, but if* `double()` *had side-effects, such as saving the value to disk or logging to the console, you couldn’t simply replace double(5) with 10 without changing the meaning*

3. What are the benefits of a pure function?

*Some benefits of a pure function include:*
* *They are the simplest reusable building blocks of code in a program*
* *Pure functions are completely independent of outside state, and as such, they are immune to entire classes of bugs that have to do with shared mutable state.*
* *Their independent nature also makes them great candidates for parallel processing across many CPUs, and across entire distributed computing clusters, which makes them essential for many types of scientific and resource-intensive computing tasks.*
* *Pure functions are also extremely independent — easy to move around, refactor, and reorganize in your code, making your programs more flexible and adaptable to future changes.*


4. What is immutability?

 *Immutable objects are objects whose state cannot be changed after declaration.*

5. What is Referential transparency?

*Referential Transparency is a term for the process of being able to replace a function call with it's resulting value without changing the meaning of the program*

6. What is a side-effect?

*A side effect is any work a function performs that isn’t directly related to calculating a final output*

*Reading Sources:*
[Master-the-JavaScript-Interview:-What-is-a-Pure-Function?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-pure-function-d1c076bec976)

[Demystifying-Functional-Programming-(Part-2)-The-need-for-immutability](https://medium.com/walmartglobaltech/demystifying-functional-programming-part-2-the-need-for-immutability-4f5c16ae2c9a)

[Node-js-Modules](https://www.geeksforgeeks.org/node-js-modules/)


----------------------------------------------------------------------------------

## VIDEO

1. What is a module?

*A module is a block of encapsulated code whose function is to communicate with an external application on the basis of their related functionality*
    
2. What does the word ‘require’ do?

*In JavaScript, `require()` is a built in function that allows us to include external modules that exist in separate files. The way `require()` works is it reads a JavaScript file, executes it, and then returns the export object*


3. How do we bring another module into the file the we are working in?

*To bring a module into the file we are working on, we need to include the following line of code in the head of our file:* `const <module> = require('<module>')`

<br />

*For Example:*  `const axios = require('axios');` 

  
4. What do we have to do to make a module available?

*In order to make a module available for us to use in the first place, we need to run the following command in our terminal in the directory which we will be importing the module `npm install <module>`*
 <br />

 *For Example* `npm install axios`

 <br />
 <br />


*Video Source*
[Node-JS-Tutorial-for-Beginners-#6-Modules-and-require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

## Things I want to know more about

* Can you turn an impure function into a pure function, and if so, how?
* What are currying functions?
* Regarding the lack of loops and 'if' statements, what benefit does excluding those serve besides maybe making it easier to determine the running time without dealing with exceptional cases?
* Considering the fact that most programs rely not only on taking input from the user, but remembering that input, and such memory is a state, is it actually even possible to write a program that is strictly functional, or is the idea that you write a bunch of pure functions using this paradigm and then use those functions in a more standard style of programming?