<h1>CSS</h1>

<h2>CSS Introduction What is CSS?</h2>
• CSS stands for Cascading Style Sheets
• CSS describes how HTML elements are to be displayed on
screen, paper, or in other media
• CSS saves a lot of work. It can control the layout of multiple
web pages all at once
• External stylesheets are stored in CSS files
CSS Demo - One HTML Page - Multiple
Styles!
Here we will show one HTML page displayed with four different stylesheets. Click on the "Stylesheet 1", "Stylesheet 2", "Stylesheet 3", "Stylesheet 4" links below to see the different styles:
Welcome to My Homepage
Use the menu to select different Stylesheets
• • • • •
I will be getting my Beginner's CSS Knowledge from a website called w3schools. Here
  is the link to the CSS Intro: http://www.w3schools.com/css/css_intro.asp
   (GO TO THE WEBSITE TO SEE HOW IT REALLY LOOKS
 [WHICH IS REALLY COOL/AWESOME!]!)
Stylesheet 1
 Stylesheet 2
 Stylesheet 3
 Stylesheet 4
 No Stylesheet
 Same Page Different Stylesheets   • Stylesheet 4
• No Stylesheet
 Same Page Different Stylesheets
This is a demonstration of how different stylesheets can change the layout of your HTML page. You can change the layout of this page by selecting different stylesheets in the menu, or by selecting one of the following links:
Stylesheet1, Stylesheet2, Stylesheet3,Stylesh eet4.
No Styles
This page uses DIV elements to group different sections of the HTML page. Click here to see how the page looks like with no stylesheet:
No Stylesheet.
      Side-Bar
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy
nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi.
Why Use CSS?
CSS is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.
CSS Solved a Big Problem
HTML was NEVER intended to contain tags for formatting a web
page!
HTML was created to describe the content of a web page, like: <h1>This is a heading</h1>
 CSS Solved a Big Problem
HTML was NEVER intended to contain tags for formatting a web
 page!
HTML was created to describe the content of a web page, like: <h1>This is a heading</h1>
<p>This is a paragraph.</p>
When tags like <font>, and color attributes were added to the HTML 3.2 specification, it started a nightmare for web developers. Development of large websites, where fonts and color information were added to every single page, became a long and expensive process.
To solve this problem, the World Wide Web Consortium (W3C) created CSS.
CSS removed the style formatting from the HTML page!
CSS Saves a Lot of Work!
The style definitions are normally saved in external .css files.
With an external stylesheet file, you can change the look of an
entire website by changing just one file!
-----
<h2>CSS Syntax and Selectors</h2>
CSS Syntax
A CSS rule-set consists of a selector and a declaration block:
 The selector points to the HTML element you want to style.
The declaration block contains one or more declarations separated
Each declaration includes a CSS property name and a value, separated by a colon.
by semicolons.
A CSS declaration always ends with a semicolon, and declaration
  The selector points to the HTML element you want to style.
The declaration block contains one or more declarations separated
 Each declaration includes a CSS property name and a value, separated by a colon.
A CSS declaration always ends with a semicolon, and declaration blocks are surrounded by curly braces.
In the following example all <p> elements will be center-aligned, with a red text color:
Example
p{
color: red;
text-align: center; }

<h2>CSS Selectors</h2>
CSS selectors are used to "find" (or select) HTML elements based on their element name, id, class, attribute, and more.
The element Selector
The element selector selects elements based on the element name. You can select all <p> elements on a page like this (in this case, all <p> elements will be center-aligned, with a red text color):
Example
p{
text-align: center;
color: red; }
The id Selector
The id selector uses the id attribute of an HTML element to select a specific element.
The id of an element should be unique within a page, so the id
selector is used to select one unique element!
To select an element with a specific id, write a hash (#) character, followed by the id of the element.
by semicolons.
 specific element.
The id of an element should be unique within a page, so the id
selector is used to select one unique element!
To select an element with a specific id, write a hash (#) character, followed by the id of the element.
The style rule below will be applied to the HTML element with id="para1":
Example
#para1 {
text-align: center; color: red;
}
Note: An id name cannot start with a number! The class Selector
The class selector selects elements with a specific class attribute. To select elements with a specific class, write a period (.) character, followed by the name of the class.
In the example below, all HTML elements with class="center" will be red and center-aligned:
Example
.center {
text-align: center; color: red;
}
You can also specify that only specific HTML elements should be affected by a class.
In the example below, only <p> elements with class="center" will be center-aligned:
Example
p.center {
 text-align: center;
color: red; }
HTML elements can also refer to more than one class.
 Example
p.center {
text-align: center;
color: red; }
HTML elements can also refer to more than one class.
In the example below, the <p> element wil be styled according to class="center" and to class="large":
Example
<p class="center large">This paragraph refers to two classes.</p> Note: A class name cannot start with a number!
Grouping Selectors
If you have elements with the same style definitions, like this: h1 {
text-align: center;
color: red; }
h2 {
text-align: center; color: red;
}
p{
text-align: center; color: red;
}
It will be better to group the selectors, to minimize the code.
To group selectors, separate each selector with a comma.
In the example below we have grouped the selectors from the code above:
Example
h1, h2, p {
 text-align: center;
color: red; }
 Example
h1, h2, p {
text-align: center;
color: red; }

<h2>CSS Comments</h2>
Comments are used to explain the code, and may help when you edit the source code at a later date.
Comments are ignored by browsers.
A CSS comment starts with /* and ends with */. Comments can also span multiple lines:
Example
p{
color: red;
/* This is a single-line comment */
text-align: center; }
/* This is
a multi-line comment */ -----
