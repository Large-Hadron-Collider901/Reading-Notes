# HTML Text, CSS Introduction, and Basic JavaScript Instructions
<br>

## Chapter 2: HTML Text - Worksheet
Here is a fill in the blank worksheet I created from the content I read in Chapter 2: HTML Text in the textbook *HTML & CSS design and build websites* By John Duckett. You can access the worksheet [Here](https://docs.google.com/document/d/1G8jiRYhfsWZKJDVyVo6xEhdZboIX6wdHBF6qEBFDk5g/edit?usp=sharing)
<br />
![Chapter2-HTML-Text-Worksheet-1](https://i.ibb.co/LnV7PbL/Chapter2-HTML-Text-Worksheet-1.png)
![Chapter2-HTML-Text-Worksheet-2](https://i.ibb.co/QCrvwfq/Chapter2-HTML-Text-Worksheet-2.png)
![Chapter2-HTML-Text-Worksheet-3](https://i.ibb.co/NsbDYTZ/Chapter2-HTML-Text-Worksheet-3.png)


<br />

### Introducing CSS - Vocabulary List

Keywords, Phrases, and Definitions From Chapter 10: Introducing CSS in the textbook *HTML & CSS design and build websites* By John Duckett.<br>

* **Block Elements:** Elements that will always appear on a new line in the browser window.

* **Inline Elements:** Elements that will always appear to continue on the same line as their neighboring elements.

* **CSS Rule:** Made up of two components, a selector and a declaration.

* **Selector:** Indicates which element (paragraphs, headings, etc.) the rule applies to. Types of selectors include: Universal, Type, Class, ID, Child, Descendant, Adjacent Sibling, and General Sibling.

* **Declaration:** Decides how the elements referred to in the selector should be styled. Declarations consist of two parts, a property and a value pair. 

* **Property:** Specifies the aspects of the element you want to change (color, font, width, height, border, etc.)

* **Value:** Chooses the settings you want to use for the chosen property. For example, if you want to choose a color property, then the value is going to be the color you want the content in these elements to be. 

* **External CSS:** A separate CSS file that defines all of the style sheet rules you want to apply to your web page. You can link external CSS files to an HTML file using the following syntax

<link href="your-external-stylesheet.css" type="text/css" 
    rel="stylesheet" />

* **Internal CSS:** An internal stylesheet is used to style a single document, and is defined in the <head> element of an HTML page. Here's an example of how you can add an internal stylesheet to an HTML file

 <head>
  <title>My Internal CSS Stylesheet</title>
   <style type=text/css>
     body {
      font-family: arial;
        background-color: blue; }
     h1 {
      color: black; }
   </style> 

<br />

## Chapter 2: Basic JavaScript Instructions - Vocabulary List
#### Keywords, Phrases, and Definitions From Chapter 2 <br />

* **Script:** A series of instructions that a computer can follow one-by-one

* **Statement:** Each individual instruction or step in the script. Each statement starts on a new line.

* **Semicolon:** Tells the JavaScript interpreter when a step is over, indicating that it can move on to the next.

* **Code Block:** A statement surrounded by curly braces, in which the closing curly brace is *not* followed by a semi-colon. Code blocks are often used to group together multiple statements, which helps programmers organize their code.

* **Comments:** Notes that explain your code to anyone who is reading it. Comments will not run in the JavaScript interpreter, they are only there to describe certain aspects of your code such as: what your code is doing, how the script works, preventing a portion of the script from running while testing it, etc. Good use of comments will help make your code easier to read and understand, for you or for other programmers. There are two types of comments in JavaScript- Multi-line comments for any comment that stretches over more than one line, and single line comments which are used for brief descriptions that cover what your code is doing.

* **Variables:** Represents numbers or other types of data

* **Declare:** Announcing that you would like to use a variable, which involves creating the variable and giving it a name. Here's an example of declaring a variable. Var is the variable keyword and quantity is the variable name.
 var quantity;  

* **Variable Name:** An identifier for your variable

* **Variable Keyword:** A keyword is a word that the JavaScript interpreter knows. For example, the JavaScript Interpreter knows the keyword "var" and it understands that it is used to create a variable.

* **Assign A Value:** The process of telling the JavaScript interpreter what information you would like it to store for you. To assign a value to a variable, you will need a variable name, an assignment operator, and a variable value.

* **Assignment Operator:** Used to update the value of a variable. The (=) sign is an assignment operator.

* **Variable Value:** If not initialized it stores 0 as a default. Until you have assigned a value to a variable, programmers say the value is "undefined"

* **Numeric Data Type:** Handles numbers

* **String Data Type:** Consists of letters and other characters

* **Boolean Value Type:** Can have one of two values, true or false.

* **Array:** A special type of variable that stores a list of values.

* **Index:** Each item in an array is automatically given a number, that number is called an index.

* **Expressions:** Evaluates into a single value. There are two types of expressions- expressions that just assign a value to a variable and expressions that use two or more values to return a single expression

* **Operators:** Allow programmers to create a single value from one or more values.

* **Assignment Operators:** Assign a value to a variable. Ex- color = 'beige';
* **Arithmetic Operators:** Perform basic math. Ex- area = 3 * 2;
* **String Operators:** Combine two strings. Ex- greeting = 'Hi' + 'Molly';
* **Comparison Operators:** Compare two values and return true or false.
* **Logical Operators:** Combine expressions and return true or false. Ex- buy = (5 > >); 
<br />

## Decisions & Loops - Synopsis <br />
#### A Summary Of What I Learned <br />

    Today in the Code Collective Academy, one of our assignments included reading: Decisions and Loops" from our textbook which is titled: "JavaScript & Jquery - Interactive Front-End Web Development" written by Jon Duckett. In this brief summary, I will be sharing with you some of the key concepts covered in the chapter, as well as what I learned from the content.
   
    As you know, chapter four is all about decisions and loops in JavaScript, which details the decision making process, and all of the different ways your code can act to handle different circumstances. In this chapter, the author walks us through the protocol of deciding which course of action is the proper direction to take our code based on the following notions: Evaluations, Decisions, and Loops.
    
    In JavaScript, there are two main components involved in making a decision. The first step in the process is to set a condition, which you will then proceed to evaluate using a comparison operator such as greater than, less than, equal to. The condition will return either true or false. The second component involved in decision making is to use a conditional statement which determines where your code will go from there, based on if/then/else; IF the condition is true, THEN your code will take one path, ELSE it chooses a different path. The last key concept I learned about JavaScript in this chapter is looping. The purpose of a loop is to carry out a specific set of instructions that will continue until a certain condition is met (or is no longer met). When your loop reaches this point, it will end and allow your script to continue on to the next line of code. 
    In closing, Chapter 14 of JavaScript & JQuery by Jon Duckett is packed with all kinds of important information regarding decision making and loops in JavaScript. While reading this chapter, I learned about the different ways I can evaluate, analyze, and customize my scripts. However, my summary does not do the book justice, as I could not present all of the great analogies, diagrams, code snippets and other helpful bits that are displayed not only in this chapter but throughout the book. I would highly recommend this textbook to anyone looking to learn JavaScript programming!