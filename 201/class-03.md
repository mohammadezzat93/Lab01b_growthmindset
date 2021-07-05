## Lists

- There are lots of occasions when we
need to use lists. HTML provides us with
three different types:  
- ** Ordered lists : **are lists where each item in the list is
numbered. For example, the list might be a set of steps for
a recipe that must be performed in order, or a legal contract
where each point needs to be identified by a section
number.

**<ol>**  
The ordered list is created with
the <ol> element.  
**<li> **  
Each item in the list is placed
between an opening <li> tag
and a closing </li> tag. (The li
stands for list item.)

- ** Unordered lists : ** are lists that begin with a bullet point
(rather than characters that indicate order).

**<ul>**  
The unordered list is created
with the <ul> element.  
**<li>**
Each item in the list is placed
between an opening <li> tag
and a closing </li> tag. (The li
stands for list item.)
- ** Definition lists : ** are made up of a set of terms along with the
definitions for each of those terms.

![List](https://media.gcflearnfree.org/content/5e46ef60397c182fec255f32_02_14_2020/lists.png)

**<dl>**
The definition list is created with
the <dl> element and usually
consists of a series of terms and
their definitions.
Inside the <dl> element you will
usually see pairs of <dt> and<dd> elements.   

**<dt>** 
This is used to contain the term
being defined (the definition
term).  

**<dd>**
This is used to contain the
definition.
Sometimes you might see a list
where there are two terms used
for the same definition or two
different definitions for the same
term.

![List](https://www.w3docs.com/uploads/media/default/0001/01/61895012b984c01394157fb224f371e8463d59bc.png)


## Boxes

- The box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. 

**Border**  
Every box has a border (even if
it is not visible or is specified to
be 0 pixels wide). The border
separates the edge of one box
from another.  

**Margin**  
Margins sit outside the edge
of the border. You can set the
width of a margin to create a
gap between the borders of two
adjacent boxes.

**Padding**  
Padding is the space between
the border of a box and any
content contained within it.
Adding padding can increase the
readability of its contents.

## Border Style
The border-style property specifies what kind of border to display.

The following values are allowed:

- dotted - Defines a dotted border  
- dashed - Defines a dashed border  
- solid - Defines a solid border  
- double - Defines a double border  
- groove - Defines a 3D grooved border. The effect depends on the - border-color value  
- ridge - Defines a 3D ridged border. The effect depends on the border-color value  
- inset - Defines a 3D inset border. The effect depends on the border-color value  
- outset - Defines a 3D outset border. The effect depends on the border-color value  
- none - Defines no border  
- hidden - Defines a hidden border  

## Border Color
The border-color property is used to set the color of the four borders.

The color can be set by:

- name - specify a color name, like "red"
- HEX - specify a HEX value, like "#ff0000"
- RGB - specify a RGB value, like "rgb(255,0,0)"
- HSL - specify a HSL value, like "hsl(0, 100%, 50%)"
transparent

![List](https://static.javatpoint.com/htmlpages/images/how-to-add-border-in-html.png)

## Summary BOXES

- CSS treats each HTML e XX lement as if it has its own box.
- You can use CSS to control the dimensions of a box.
- You can also control the borders, margin and padding
for each box with CSS.
- It is possible to hide elements using the display and
visibility properties.
- Block-level boxes can be made into inline boxes, and
inline boxes made into block-level boxes.
- Legibility can be improved by controlling the width of
boxes containing text and the leading.
- CSS3 has introduced the ability to create image
borders and rounded borders.


## JavaScript Variables
- There are 3 ways to declare a JavaScript variable:

*Using var*  
*Using let*  
*Using const*  

- Variables are containers for storing data (values).

In this example, x, y, and z, are variables, declared with the var keyword:

Example
var x = 5;
var y = 6;
var z = x + y;  

## JavaScript Identifiers
- All JavaScript variables must be identified with unique names.

- These unique names are called identifiers.

- Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).

- The general rules for constructing names for variables (unique identifiers) are:

- Names can contain letters, digits, underscores, and dollar signs.
- Names must begin with a letter
- Names can also begin with $ and _ (but we will not use it in this tutorial)
- Names are case sensitive (y and Y are different variables)
Reserved words (like JavaScript keywords) cannot be used as names

![List](https://thecodelearners.com/wp-content/uploads/2020/04/javascript-variables-1280x720.jpg)


# Operators and Loops

## Loop :  When you want to repeat somthing


1- **While :** We dont no how any time the code will run , but for sure we know it well keep running as long as the condition is true . 

2- **For :** We are gonna use When we know how many time the code need to run .  
  
- ## The while() loop

The while() loop has the form:

  while ( expression ) {  
    /* Do something... */  
  }  
  - **The contents of the loop, which as always may be a single statement or a { ... } block, are executed for as long as the controlling expression is true.**  

 - *If the condition is false the body of the loop never executes at all.
This may sound slightly unintuitive (if there's nothing to do, why have a loop?) but when writing a program we often don't know if there will always be something to loop over and it would be really inconvenient to have to wrap every loop inside an if() statement.*  

**Key Point : **If the condition is false the body of the loop never executes at all.  

- ## The for() loop  

The for() loop rolls all these three into one. It has the following format:

for (Initialise; Test; Increment ) {  
    ... /* Loop body */  
  }  

  - **Note that the three expressions are separated by semicolons, not commas, and that they occur in the same order as they are used. **  
- *The steps in the for() loop are done in exactly the same order as in the equivalent while() loop:*  

**Key Point : **
Initialise  
Loop:  
1-Test and if false quit the loop.  
2-Execute the body.  
3-Increment.

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