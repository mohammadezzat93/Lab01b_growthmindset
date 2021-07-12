# Layout

## Continue to the previous lesson

#### As we previously talked about in Read 04 :
- CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

### Overlapping Elements

- *When you use relative, fixed, or
absolute positioning, boxes can
overlap. If boxes do overlap, the
elements that appear later in the
HTML code sit on top of those
that are earlier in the page.
If you want to control which
element sits on top, you can use
the z-index property. Its value
is a number, and the higher the
number the closer that element
is to the front. For example, an
element with a z-index of 10
will appear over the top* 

- *To ensure that the
h1 element stays on top, we
use the z-index property on the
rule for the h1 element.
The z-index is sometimes
referred to as the stacking
context (as if the blocks have
been stacked on top of each
other on a z axis).*


### Floating Elements

*The float property allows you
to take an element in normal
flow and place it as far to the
left or right of the containing
element as possible.
Anything else that sits inside
the containing element will
flow around the element that is
floated.
When you use the float
property, you should also use the
width property to indicate how
wide the floated element should
be. If you do not, results can be
inconsistent but the box is likely
to take up the full width of the
containing element (just like it
would in normal flow).*

### Clearing Floats

### **Clear**  
The clear property allows you
to say that no element (within
the same containing element)
should touch the left or righthand
sides of a box. It can take
the following values:  
**left**  
The left-hand side of the box
should not touch any other
elements appearing in the same
containing element.  
**right**  
The right-hand side of the
box will not touch elements
appearing in the same containing
element.  
**both**  
Neither the left nor right-hand
sides of the box will touch
elements appearing in the same
containing element.  
**none**  
Elements can touch either side.

![Image](https://www.1keydata.com/css-tutorial/example-float-right-float-left.jpg)


## Screen Sizes

- Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide
(since most users will be able to see designs this wide on their screens).

### Fixed Width Layouts

*To create a fixed width layout,
the width of the main boxes on
a page will usually be specified
in pixels (and sometimes their
height, too).
Here you can see several <div>
elements, each of which uses an
id or class attribute to indicate
its purpose on the page.
In a book like this, the result of
both the fixed and liquid layouts
look similar. To get a real feel for
them, you need to view them in
your browser and see how they
react when you adjust the size of
the browser window.
The fixed width layout will stay
the same width no matter what
size the browser window is,
whereas the liquid layout will
stretch (or shrink) to fill the
screen.*

![Image](https://i.stack.imgur.com/eSSfS.png)


### A Liquid Layout

*The liquid layout uses
percentages to specify the width
of each box so that the design
will stretch to fit the size of the
screen.
When trying this in your
browser, remember to make the
window smaller and larger.*


## CSS Frameworks

- **CSS frameworks aim to make your life easier by providing the code for
common tasks, such as creating layout grids, styling forms, creating
printer-friendly versions of pages and so on. You can include the CSS
framework code in your projects rather than writing the CSS from scratch.**

![Image](https://www.roxunlimited.com/blog/wp-content/uploads/top-css-frameworks-you-should-use-in-your-projects.jpg)

## Summary Layout

- <div> elements are often used as containing elements
to group together sections of a page.
- Browsers display pages in normal flow unless you
specify relative, absolute, or fixed positioning.
- The float property moves content to the left or right
of the page and can be used to create multi-column
layouts. (Floated items require a defined width.)
- Pages can be fixed width or liquid (stretchy) layouts.
- Designers keep pages within 960-1000 pixels wide,
and indicate what the site is about within the top 600
pixels (to demonstrate its relevance without scrolling).
- Grids help create professional and flexible designs.
- CSS Frameworks provide rules for common tasks.
- You can include multiple CSS files in one page. 