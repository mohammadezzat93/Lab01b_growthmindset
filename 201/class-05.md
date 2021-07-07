## Images

![Image](https://i.ytimg.com/vi/Bor5lkRyeGo/hqdefault.jpg)

*There are many reasons why you might
want to add an image to a web page: you
might want to include a logo, photograph,
illustration, diagram, or chart.*

### <img>
- To add an image into the page
you need to use an <img>
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:
src
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site.

### alt
- This provides a text description
of the image which describes the
image if you cannot see it.

### Height & Width of Images
- You will also often see an <img>
element use two other attributes
that specify its size:  
**height**  
This specifies the height of the
image in pixels.  
**width**  
This specifies the width of the
image in pixels.

### Aligning Images Horizontally

**align**  
-The align attribute was
commonly used to indicate how
the other parts of a page should
flow around an image.

**left**  
This aligns the image to the left
(allowing text to flow around its
right-hand side).  
**right**  
This aligns the image to the right
(allowing text to flow around its
left-hand side).

### Aligning Images Vertically

**top**  
This aligns the first line of the
surrounding text with the top of
the image.  
**middle**  
This aligns the first line of the
surrounding text with the middle
of the image.  
**bottom**  
This aligns the first line of the
surrounding text with the bottom
of the image.

-------

## Color

### Foreground Color

- The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:  

**rgb values**  
These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)  

**hex codes**  
These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80  

**color names**  
There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan  

### background Color

- *treats each HTML element
as if it appears in a box, and the
background-color property
sets the color of the background
for that box.
You can specify your choice of
background color in the same
three ways you can specify
foreground colors: RGB values,
hex codes, and color names*

### Summary COLOR
- Color not only brings your site to life, but also helps
convey the mood and evokes reactions.  
- There are three ways to specify colors in CSS:
RGB values, hex codes, and color names.
- Color pickers can help you find the color you want.
- It is important to ensure that there is enough contrast
between any text and the background color (otherwise
people will not be able to read your content).
- CSS3 has introduced an extra value for RGB colors to
indicate opacity. It is known as RGBA.
- CSS3 also allows you to specify colors as HSL values,
with an optional opacity value. It is known as HSLA.

--------

## Text

### HTML contains several elements for defining text with a special meaning.

### Specifying Typefaces

**font-family**
- The font-family property
allows you to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.
The value of this property is the
name of the typeface you want
to use.

**font-size**
- The font-size property enables
you to specify a size for the
font. There are several ways to
specify the size of a font. The
most common are:  
pixels , percentages , ems  

### **text-transform**

**uppercase**  
This causes the text to appear
uppercase.  
**lowercase**   
This causes the text to appear
lowercase.  
**capitalize**  
This causes the first letter of
each word to appear capitalized.


### **text-align**

**left**  
This indicates that the text
should be left-aligned.  
**right**  
This indicates that the text
should be right-aligned.  
**center**  
This allows you to center text.  
**justify**  
This indicates that every line in
a paragraph, except the last line,
should be set to take up the full
width of the containing box.

*HTML Formatting Elements
Formatting elements were designed to display special types of text:*

**<b>** - Bold text  
**<strong>** - Important text  
**<i>** - Italic text  
**<em>** - Emphasized text  
**<mark>** - Marked text  
**<small>** - Smaller text  
**<del>** - Deleted text  
**<ins>** - Inserted text  
**<sub>** - Subscript text  
**<sup>** - Superscript text  

### Summary TEXT
- There are properties to control the choice of font, size,
weight, style, and spacing.  
- There is a limited choice of fonts that you can assume
most people will have installed.
- If you want to use a wider range of typefaces there are
several options, but you need to have the right license
to use them.
- You can control the space between lines of text,
individual letters, and words. Text can also be aligned
to the left, right, center, or justified. It can also be
indented.
- You can use pseudo-classes to change the style of an
element when a user hovers over or clicks on text, or
when they have visited a link.

## JPEG vs PNG vs GIF
- we would only be looking at the three most commonly used image formats in websites and mobile applications — JPEG, PNG and GIF. Several statistics reports, including the one from HTTP Archive, indicate that these 3 formats together comprise of more than 95% of all images loaded on websites. However, these 3 image formats have significant differences amongst themselves thus making each of them suitable for specific use cases. Understanding these major differences would help us deliver the best possible images to our website and mobile app users.

**TL;DR**  
Use **JPEG** format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use **PNG** format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use **GIF** format for images that contain animations.

**Compression**  
Almost all forms of data that we see on the internet — text, image, video etc. — are compressed to reduce the size of data and ensure faster transmission. Choosing the correct format and compression is a major factor that determines image size.

**Colours**  
There is a significant difference in the number of colours that can be supported by these 3 formats.  
**JPEG** images can support around 16 million colours. This is what makes them suitable for storing images of natural scenes.  
**PNG** images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image. Use PNG8 for simple shapes with fewer colours and PNG24 for high quality, complex logos and shapes with rounded corners on a transparent background.
**GIF** images are limited to 256 colours. If index transparency is used, then one of these 256 colours is assigned as transparent and the remaining 255 are used for other colours.

![JPEG & png & gif](https://www.kindpng.com/picc/m/10-105494_jpeg-png-gif-lossy-vs-lossless-venn-diagram.png)