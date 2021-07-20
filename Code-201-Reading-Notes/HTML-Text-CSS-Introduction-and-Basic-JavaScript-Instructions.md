# HTML Text, CSS Introduction, and Basic JavaScript Instructions
<br>

## Chapter 2: HTML Text - Worksheet
#### Directions: Use what you have learned in chapter 2 of your textbook to fill in the blanks with the correct word to complete each statement.

1. When creating a webpage you add tags, also known as   ____________, to the content of the page.

2. These tags provide extra ___________ and allow browsers to show users the appropriate _____________ for the page.

3. Elements that you can use to describe both headings and paragraphs are called _______________  markup.

4. ______________ markup provides extra information, such as where emphasis is placed in a sentence, to indicate something you have written is a quotation (and who said it), the meaning of acronyms and so on.

5. In HTML, there are six “levels” of  _____________.

6. The _____ tag is used for main headings and the _____ tag is used for subheadings.

7. To create a paragraph in HTML, you must surround the words that make up the paragraph with an opening and closing  _______.

8. By enclosing words with <b> and </b> we can make the characters appear _________.

9. To make characters italic, you must enclose words in a ____ opening tag and a ____ closing tag.

10. Characters such as the suffixes of dates or mathematical concepts like raising a number to a power such as 22  are called _____________ and are contained  with the ____ tag.

11. Characters like footnotes or chemical formulas such as H2O  are called  ______________  and are contained with the _____ tag. 

12. When a browser comes across two or more spaces next to each other, it displays as _____ space(s).

13. If you want to add a line break inside the middle of a paragraph, you can use the ____ tag.

14. If you want to create a break between themes, you can use the _____ tag.

15. Content management systems and HTML editors usually have two views of the page you are creating: a _________ editor and a _______ view.

16. Code _______ shows you the code created by the visual editor so you can manually edit it or so you can just enter new code yourself.

17. Visual _______ often resemble word processors and although each one will differ slightly, there are some features that are common to most editors that allow you to control the presentation of a text.

18. There are some text elements that are not intended to affect the structure of your web pages, but they do add extra information to the pages, they are known as ____________ markup.

19. By default, browsers will show the contents of a <strong> element in _________ and they will show the contents of a <em> element in _________.

20. For long quotations that take up an entire paragraph, the  ______________ element is used, but for shorter quotes that sit within a paragraph, a _____ element is used.

21. Browsers tend to _________ the contents of a <blockquote> element, however this element should not be used just to indent a piece of text -- rather, you can achieve that effect using CSS.

22. Browsers are supposed to  put _________ around the <q> element, however Internet Explorer does not, which is why many people avoid using the <q> element.

23. In HTML5 both abbreviations and acronyms use the ________ element.

24. Browsers will render the content of a <cite> element in __________.

25. The <dfn> element should be used to indicate the _________ instance of a new term.

26. The <address> element is used to contain the ________ details for the owner of the page.

27. The _____ element is used to show text that has been deleted from the page, and the text of this element usually appears on the page with a ______ through it.

28. The <ins> element can be used to show content that has been _________ into a document, and the text of an <ins> element usually appears on the page with a ____________.

29. The _____ element indicates something that is no longer accurate or relevant (but should not be deleted) Visually, the text effected by this element will usually be displayed with a  _______ through the center. 

30. Some browsers show the content of a <dfn> element in _______, however ________ and _________ do not.
<br />

### Chapter 10: Introducing CSS - Vocabulary List
#### Keywords, Phrases, and Definitions From Chapter 10

**Block Elements:** Elements that will always appear on a new line in the browser window.

**Inline Elements:** Elements that will always appear to continue on the same line as their neighboring elements.

**CSS Rule:** Made up of two components, a selector and a declaration.

**Selector:** Indicates which element (paragraphs, headings, etc.) the rule applies to. Types of selectors include: Universal, Type, Class, ID, Child, Descendant, Adjacent Sibling, and General Sibling.

**Declaration:** Decides how the elements referred to in the selector should be styled. Declarations consist of two parts, a property and a value pair. 

**Property:** Specifies the aspects of the element you want to change (color, font, width, height, border, etc.)

**Value:** Chooses the settings you want to use for the chosen property. For example, if you want to choose a color property, then the value is going to be the color you want the content in these elements to be. 

**External CSS:** A separate CSS file that defines all of the style sheet rules you want to apply to your web page. You can link external CSS files to an HTML file using the following syntax

<link href="your-external-stylesheet.css" type="text/css" 
    rel="stylesheet" />

**Internal CSS:** An internal stylesheet is used to style a single document, and is defined in the <head> element of an HTML page. Here's an example of how you can add an internal stylesheet to an HTML file

<head>
  <title>My Internal CSS Stylesheet</title>
   <style type=text/css>
     body {
      font-family: arial;
        background-color: blue; }
     h1 {
      color: black; }
   </style>


## Chapter 2: Basic JavaScript Instructions - Vocabulary List
#### Keywords, Phrases, and Definitions From Chapter 2

**Script:** A series of instructions that a computer can follow one-by-one

**Statement:** Each individual instruction or step in the script. Each statement starts on a new line.

**Semicolon:** Tells the JavaScript interpreter when a step is over, indicating that it can move on to the next.

**Code Block:** A statement surrounded by curly braces, in which the closing curly brace is *not* followed by a semi-colon. Code blocks are often used to group together multiple statements, which helps programmers organize their code.

**Comments:** Notes that explain your code to anyone who is reading it. Comments will not run in the JavaScript interpreter, they are only there to describe certain aspects of your code such as: what your code is doing, how the script works, preventing a portion of the script from running while testing it, etc. Good use of comments will help make your code easier to read and understand, for you or for other programmers. There are two types of comments in JavaScript- Multi-line comments for any comment that stretches over more than one line, and single line comments which are used for brief descriptions that cover what your code is doing.

**Variables:** Represents numbers or other types of data

**Declare:** Announcing that you would like to use a variable, which involves creating the variable and giving it a name. Here's an example of declaring a variable. Var is the variable keyword and quantity is the variable name.
 var quantity;  

**Variable Name:** An identifier for your variable

**Variable Keyword:** A keyword is a word that the JavaScript interpreter knows. For example, the JavaScript Interpreter knows the keyword "var" and it understands that it is used to create a variable.

**Assign A Value:** The process of telling the JavaScript interpreter what information you would like it to store for you. To assign a value to a variable, you will need a variable name, an assignment operator, and a variable value.

**Assignment Operator:** Used to update the value of a variable. The (=) sign is an assignment operator.

**Variable Value:** If not initialized it stores 0 as a default. Until you have assigned a value to a variable, programmers say the value is "undefined"

**Numeric Data Type:** Handles numbers

**String Data Type:** Consists of letters and other characters

**Boolean Value Type:** Can have one of two values, true or false.

**Array:** A special type of variable that stores a list of values.

**Index:** Each item in an array is automatically given a number, that number is called an index.

**Expressions:** Evaluates into a single value. There are two types of expressions- expressions that just assign a value to a variable and expressions that use two or more values to return a single expression

**Operators:** Allow programmers to create a single value from one or more values.

**Assignment Operators:** Assign a value to a variable. Ex- color = 'beige';
**Arithmetic Operators:** Perform basic math. Ex- area = 3 * 2;
**String Operators:** Combine two strings. Ex- greeting = 'Hi' + 'Molly';
**Comparison Operators:** Compare two values and return true or false.
**Logical Operators:** Combine expressions and return true or false. Ex- buy = (5 > 3) && (2 < 4>); 


## Chapter 4: Declarations & Loops - Synopsis
#### A Summary Of What I Learned In Chapter 4

    Today in the Code Collective Academy, one of our assignments included reading "Chapter 4: Declarations and Loops" from our textbook which is titled: "JavaScript & Jquery - Interactive Front-End Web Development" written by Jon Duckett. In this brief summary, I will be sharing with you some of the key concepts covered in the chapter, as well as what I learned from the content.
   
    As you know, chapter four is all about declarations and loops in JavaScript!