## Links

**Links** are created using the <a> element. Users can click on anything
between the opening <a> tag and the closing </a> tag. You specify
which page you want to link to using the href attribute.

- When you link to a different website, the value of the href attribute
 will be the full web address for the site, which is known as an absolute URL.

 - **Linking to Other Pages
on the Sa me Site**

*When you are linking to other
pages within the same site,
you do not need to specify the
domain name in the URL. You
can use a shorthand known as a
relative URL.
If all the pages of the site are in
the same folder, then the value
of the href attribute is just the
name of the file.*

- **Email Links**

**1** - To create a link that starts up
the user's email program and
addresses an email to a specified
email address, you use the <a>
element. However, this time the
value of the href attribute starts
with mailto: and is followed by
the email address you want the
email to be sent to.  
**2** - On the right you can see that
an email link looks just like any
other link but, when it is clicked
on, the user's email program
will open a new email message
and address it to the person
specified in the link.

- **Op ening Links in a New Window**

### target
*If you want a link to open in a
new window, you can use the
target attribute on the opening
<a> tag. The value of this
attribute should be _blank. *   
*One of the most common
reasons a web page author
might want a link to be opened
in a new window is if it points to
another website. In such cases,
they hope the user will return
to the window containing their
site after finishing looking at the
other one.*  

### Summary LINKS
- Links are created using the <a> element.
- The <a> element uses the href attribute to indicate
the page you are linking to.
- If you are linking to a page within your own site, it is
best to use relative links rather than qualified URLs.
- You can create links to open email programs with an
email address in the "to" field.
- You can use the id attribute to target elements within
a page that can be linked to.

## Layout

### Building Blocks
- CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.
- Block-level boxes start on a new line and act as the main building blocks
of any layout, while inline boxes flow between surrounding text. You can
control how much space each box takes up by setting the width of the
boxes (and sometimes the height, too). To separate boxes, you can use
borders, margins, padding, and background colors.

#### Block-level elements
start on a new line
Examples include: <h1> <p> <ul> <li>  
#### Inline elements
flow in between
surrounding text
Examples include: <img> <b> <i>

![Layout](https://www.practicalecommerce.com/wp-content/uploads/2017/10/101217-complex-layout-570x293.png)


### Normal Flow

**position : static**

In normal flow, each block-level
element sits on top of the next
one. Since this is the default
way in which browsers treat
HTML elements, you do not
need a CSS property to indicate
that elements should appear
in normal flow, but the syntax
would be:  
**position: static**;
I have not specified a width
property for the heading
element,  it
stretches the width of the entire
browser window by default.

### Relative Positioning

**position : relative**

- Relative positioning moves an
element in relation to where it
would have been in normal flow.
For example, you can move it 10
pixels lower than it would have
been in normal flow or 20% to
the right.
- You can indicate that an element
should be relatively positioned
using the position property
with a value of relative.
- You then use the offset
properties (top or bottom and
left or right) to indicate how
far to move the element from
where it would have been in
normal flow.

### Absolute Positioning

**position : absolute**

- When the position property
is given a value of absolute,
the box is taken out of normal
flow and no longer affects the
position of other elements on
the page. (They act like it is not
there.)
- The box offset properties (top
or bottom and left or right)
specify where the element
should appear in relation to its
containing element.

### Fixed Positioning
**position : fixed**

- Fixed positioning is a type
of absolute positioning that
requires the position property
to have a value of fixed.
- It positions the element in
relation to the browser window.
Therefore, when a user scrolls
down the page, it stays in the
exact same place. It is a good
idea to try this example in your
browser to see the effect.
- To control where the fixed
position box appears in relation
to the browser window, the box
offset properties are used.

## Functions, Methods, and Objects
![Layout](https://cdn.educba.com/academy/wp-content/uploads/2020/02/JavaScript-Function-Declaration.jpg)

### Functions
- Self-contained bits of JS code that allow us to  
• Organize code  
• Reuse the same code any number of times, from different
parts of the script  
- JS supports several types of function. Commonly used types are:  
• Named function declaration  
• Anonymous functions  

| What | Why | How
| :---: | :---: | :---:
| block of code that does something | re-use the code| Function Decleration
|  | Organize our code | Function Expression

## syntax
**function square(number) {  
  return number * number;  
}**

![Layout](https://cdn-media-1.freecodecamp.org/images/0*wy_bAnMM-coF9cep.png)


## JavaScript Objects
• JavaScript is an object-based language  
• It supports for object-oriented programming but not at the same level as
other languages (ES6: introduced class – still lacks private property  )
• Objects are represented as property-value pair  
• The property values can be data or functions (methods)  
• A property is something that can be modified :  
• Data properties : primitive values or references to objects  
• Method properties : can be executed  
• Objects can be created and their properties can be changed
dynamically  
• JS is not really typed .. If it doesn’t care between a number and a string, why
care between two kinds of objects?

### Creating Objects  
Create an object and assign variables and functions directly by using  
**{ }** syntax

### Accessing Objects
• Access properties or methods of an object using dot notation  
-example: var hotelname = hotel.name  
• Access properties or methods using square brackets  
-example: var hotelname = hotel["name"]  

### 6 Reasons for Pair Programming

**pair programming**  
 is the practice of two developers sharing a single workstation to interactively tackle a coding task together. At Code Fellows, pair programing is one way we foster a collaborative environment while developing key industry skills.

### How does pair programming work?
While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

### benefits pair programming

1. Greater efficiency

2. Engaged collaboration

3. Learning from fellow students

4. Social skills

5. Job interview readiness

6. Work environment readiness
