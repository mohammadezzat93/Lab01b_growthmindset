# Summary of today's lecture

## CSS : Cascading Style Sheets

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

- *he name cascading comes from the specified priority scheme to determine which style rule applies if more than one rule matches a particular element. This cascading priority scheme is predictable.*  


### CSS priority scheme (highest to lowest)

| Priority | CSS source type	 | Description
| :---: | :---: | :---:
| 1 |	Importance |	The "!important" annotation overwrites the previous priority types
|2 |	Inline |	A style applied to an HTML element via HTML "style" attribute
|3|	Media Type |	A property definition applies to all media types, unless a media specific CSS is defined
|4 |	User defined |	Most browsers have the accessibility feature: a user defined CSS
|5 |	Selector specificity |	A specific contextual selector (#heading p) overwrites generic definition
|6 |	Rule order |	Last rule declaration has a higher priority
|7	|Parent |inheritance	If a property is not specified, it is inherited from a parent element
|8	|CSS property definition in HTML document |	CSS rule or CSS inline style overwrites a default browser value
|9	|Browser default	|The lowest priority: browser default value is determined by W3C initial value specifications