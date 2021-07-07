#   Text

### heading

**<h1>**
Browsers display the contents of
headings at different sizes. The
contents of an <h1> element is
the largest, and the contents of
an <h6> element is the smallest.
The exact size at which each
browser shows the headings
can vary slightly*

### Paragraphs

**<p>**
To create a paragraph, surround
the words that make up the
paragraph with an opening <p>
tag and closing </p> tag.
By default, a browser will show
each paragraph on a new line
with some space between it and
any subsequent paragraphs.

### Bold & Italic

**<b>**  
By enclosing words in the tags
<b> and </b> we can make
characters appear bold.

**<i>**  
The <i> element also represents
a section of text that would be
said in a different way from
surrounding content

**<sup>**  
The <sup> element is used
to contain characters that
should be superscript such
as the suffixes of dates or
mathematical concepts like
raising a number to a power such
as 22.  
**<sub>**  
The <sub> element is used to
contain characters that should
be subscript. 

**<br>**  
As you have already seen, the
browser will automatically show
each new paragraph or heading
on a new line

**<strong>**  
The use of the <strong>
element indicates that its
content has strong importance.

![structure of HTML](https://mason.gmu.edu/~kshiffl4/375/HTML_Tags.jpg)


**Structural markup** : the elements that you can use to
describe both headings and paragraphs  
**Semantic markup** : which provides extra information; such
as where emphasis is placed in a sentence, that something
you have written is a quotation (and who said it), the
meaning of acronyms, and so on

## Summary TEXT
- HTML elements are used to describe the structure of
the page (e.g. headings, subheadings, paragraphs).
- They also provide semantic information (e.g. where
emphasis should be placed, the definition of any
acronyms used, when given text is a quotation).


## INTRODUCING CSS

*Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document written in a markup language such as HTML. CSS is a cornerstone technology of the World Wide Web, alongside HTML and JavaScript.*

| What | Why | How
| :---: | :---: | :---:
| Cascading Style Sheets | How the content Looklike | inline style : <p style="somthing:somthing" ></p>
|  | Adding coloring the web | internal Style : Single html page     <style><style>
|  | Control the position of the element | external Style : Creat new Css file and link it to the html <link rel="stylesheet" href="mystyle.css">
|  | font : size/weight/type
|  | borders
|  | Responsivness
|  | animate the website

![CSS](https://www.codegrepper.com/codeimages/how-to-add-css-file-in-django-template.png)
-------
![CSS](https://miro.medium.com/max/1400/1*J1qT2jIaj-AqsuhyIqcPbQ.png)




### Summary
- CSS treats each HTML e XX lement as if it appears inside
its own box and uses rules to indicate how that
element should look.
- Rules are made up of selectors (that specify the
elements the rule applies to) and declarations (that
indicate what these elements should look like).
- Different types of selectors allow you to target your
rules at different elements.
- Declarations are made up of two parts: the properties
of the element that you want to change, and the values
of those properties. For example, the font-family
property sets the choice of font, and the value arial
specifies Arial as the preferred typeface.
- CSS rules usually appear in a separate document,
although they may appear within an HTML page.


# JavaScript

*JavaScript often abbreviated as JS, is a programming language that conforms to the ECMAScript specification. JavaScript is high-level, often just-in-time compiled, and multi-paradigm. It has curly-bracket syntax, dynamic typing, prototype-based object-orientation, and first-class functions.*

| It is Functionality | Programming Language | For interaction with user
| :---: | :---: | :---:

# Syntax
### The Rules of doing Something
**Variables** in JavaScript can be defined using either the **var**, **int** , **boolean** or **String** keywords.

## Operator :
* arithmatic Operator 

 example : + * / -

* assigment Operator:  
 example : = 

 ## Comparison : 

* example : > < == === !=

### However, most runtime environments have a console object that can be used to print output. Here is a minimalist Hello World program in JavaScript:

# console.log("Hello World!");

## **Switch**

- The switch statement is used to perform different actions based on different conditions.

- Use the switch statement to select one of many code blocks to be executed.

*Syntax*  
switch(expression) {  
  case x:  
    // code block  
    break;  
  case y:  
    // code block  
    break;  
  default:  
    // code block  
}  

### This is how it works:

- The switch expression is evaluated once.
- The value of the expression is compared with the values of each case.
- If there is a match, the associated block of code is executed.
- If there is no match, the default code block is executed.  

**Example**  
- The getDay() method returns the weekday as a number between 0 and 6.

(Sunday=0, Monday=1, Tuesday=2 ..)

This example uses the weekday number to calculate the weekday name:

switch (new Date().getDay()) {  
  case 0:  
    day = "Sunday";  
    break;  
  case 1:  
    day = "Monday";  
    break;  
  case 2:  
     day = "Tuesday";  
    break;  
  case 3:  
    day = "Wednesday";  
    break;  
  case 4: 
    day = "Thursday";  
    break;  
  case 5:  
    day = "Friday";  
    break;  
  case 6:  
    day = "Saturday";  
}  

### The break Keyword
- When JavaScript reaches a break keyword, it breaks out of the switch block.

- This will stop the execution inside the switch block.

- It is not necessary to break the last case in a switch block. The block breaks (ends) there anyway.

**Note: If you omit the break statement, the next case will be executed even if the evaluation does not match the case.**

### The default Keyword
- The default keyword specifies the code to run if there is no case match


![Javascript/switch](https://www.javascripttutorial.net/wp-content/uploads/2016/08/JavaScript-switch-case.png)
