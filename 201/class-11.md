## Images

### Controlling sizes of images in CSS

- You can control the size of an
image using the width and
height properties in CSS, just
like you can for any other box.
Specifying image sizes helps
pages to load more smoothly
because the HTML and CSS
code will often load before the
images, and telling the browser
how much space to leave for an
image allows it to render the rest
of the page without waiting for
the image to download.

### Aligning images
Using CSS can be used
to move an element to the left or
the right of its containing block,
allowing text to flow around it.
Rather than using the <img>
element's align attribute, web
page authors are increasingly
using the float property to align
images.

- The float property is used for positioning and formatting content e.g. let an image float left to the text in a container.

- The float property can have one of the following values:

**left**  
-The element floats to the left of its container  
**right**  
-The element floats to the right of its container  
**none**  
-The element does not float (will be displayed just where it occurs in the text). This is default  
**inherit**  
-The element inherits the float value of its parent

![Image](https://css-tricks.com/wp-content/uploads/2021/03/print-layout.png)

### Centering images Using css

- By default, images are inline
elements. This means that they
flow within the surrounding text.
In order to center an image, it
should be turned into a blocklevel
element using the display
property with a value of block.
Once it has been made into a
block-level element.  

- There are two common ways in which you
can horizontally center an image:  
**1:** On the containing element,
you can use the text-align
property with a value of center.  
**2:** On the image itself, you can
use the use the margin property
and set the values of the left and
right margins to auto.

### The background-image
- property allows you to place
an image behind any HTML
element. This could be the entire
page or just part of the page. By
default, a background image will
repeat to fill the entire box.
The path to the image follows
the letters url, and it is put
inside parentheses and quotes.

#### background-position

- When an image is not being
repeated, you can use the
background-position
property to specify where in the
browser window the background
image should be placed.
This property usually has a pair
of values. The first represents
the horizontal position and the
second represents the vertical.
**left top,
left center,
left bottom
center top,
center center,
center bottom,
right top,
right center,
right bottom**,
If you only specify one value,
the second value will default to
center.

- You can also use a pair of pixels
or percentages. These represent
the distance from the top left
corner of the browser window
(or containing box). The top left
corner is equal to 0% 0%.

## Practical Information

- In every page of your website there are seven key places where keywords
(the words people might search on to find your site) can appear in order
to improve its findability.

1: Page Title  
2: URL / Web Address  
3: Headings  
4: Text  
5: Link Text  
6: Image Alt Text  
7: Page Descriptions  

### How to Identify Keywords and Phrases

- Determining which keywords to use on your site can be one of the
hardest tasks when you start to think about SEO.
- six steps that
will help you identify the right keywords and phrases for your site..

**1: Brainstorm,
2: Organize,
3: Research,
4: Compare,
5: Refine,
6: Map**



## Analytics: Learning about your Visitors

*As soon as people start coming to your site, you can start analyzing
how they found it, what they were looking at and at what point they are
leaving. One of the best tools for doing this is a free service offered by
Google called Google Analytics.*

### How it Works
Every time someone loads a
page of your site, the tracking
code sends data to the Google
servers where it is stored.
Google then provides a webbased
interface that allows you
to see how visitors use your site.

### Domain Names & Hosting

#### Domain Names
Your domain name is your web
address (e.g. google.com or bbc.
co.uk). There are many websites
that allow you to register domain
names. Usually you will have to
pay an annual fee to keep that
domain name.
These sites usually have a form
that allows you to check whether
your preferred domain name is
available

#### Hosting

So that other people can see
your site, you will need to upload
it to a web server. Web servers
are special computers that are
constantly connected to the
Internet. They are specially set
up to serve web pages when
they are requested.
With the exception of some very
large sites, most websites live on
web servers run by web hosting
companies. This is usually far
cheaper and more reliable than
trying to run your own web
servers.

-------

## Flash

- Flash is a very popular technology used
to add animations, video, and audio to
websites. 

-The most popular way of
adding Flash into a web page
is using JavaScript. There are
several scripts that allow you
to do this without an in-depth
understanding of the JavaScript
language.
The script we will be looking at
here is called **SWFObject**. 

- The SWFObject
script is hosted on Google's
servers. We include the script in
this web page using the first of
the two script elements.
- The type attribute is used on the
script element to indicate
that the script inside is written
in JavaScript. The src attribute
tells the browser where to find
the script.
- The second script element
is used to tell the browser about
the Flash movie, as well as which
element it should replace. This
element is actually telling the
SWFObject script five pieces
of information, which are in the
brackets:

1. The location of the .swf file:
flash/bird.swf
2. The element that the Flash
movie should replace, specified
by the value of the id attribute
on the <div> element:
bird
3. The width of the Flash movie:
400 px
4. The height of the Flash movie:
300 px
5. The minimum version of the
Flash player needed to view the
movie:
Flash Player 8