# HTML Lists

There are three types of lists in HTML:

### 1. Ordered List: Organized by number, a good choice for lists that consist of a certain number of steps that need to be done in order, or for lists that require a format with sections

````
HTML Example:                     Result:
<ol>                            
   <li>List item</li>             1. List item
   <li>List item</li>             2. List item
   <li>List item</li>             3. List item                                
</ol>
````
### 2. Unordered List: Organized with bullet points. The HTML syntax for unordered lists is the same as it is for ordered lists except for instead of opening and closing <ol></ol> elements, you will use opening and closing <ul></ul> elements.

````
HTML Example:                      Result:
<ul>                                                                    
  <li></li>                        • List item        
  <li></li>                        • List item
  <li></li>                        • List item
</ul>
````

### 3. Definition List: A vocabulary list that is made up of a set of terms along with their definitions. The structure of a definition list is a little bit different from the other types of lists, but not much different. A definition list open with a <dl> element and close with a </dl> element. The term that is going to be defined (definition term) will go between an opening <dt> element and a closing </dt> element. Then, the definition for that term will be contained with an opening <dd> element and a closing </dd> element


```` 
HTML Example:                     Result:

<dl>                                                                    
  <dt></dt>                       Term         
  <dd></dd>                          Definition                
  <dt></dt>                       Term
  <dd></dd>                          Definition
  <dt></dt>                       Term
  <dd></dd>                          Definition                
</dl>
````
You can also put a second list inside an <li> element to make a nested list

````
HTML Example:                      Result:

<ul>
   <li>Item</li>                   • Item
   <li>Item                        • Item
     <ul>                             • Nested item
       <li>Nested item</li>           • Nested item
       <li>Nested item</li>           • Nested item
       <li>Nested item</li>        • Item
    </ul>
   </li>
  <li>Item</li>
</ul>
````


# CSS Boxes


# JS Control Flow