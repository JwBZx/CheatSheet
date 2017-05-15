<h1>HTML</h1>

<h2>What is HTML?</h2>
HTML is a markup language for describing web documents (web
pages).
• HTML stands for Hyper Text Markup Language
• A markup language is a set of markup tags
• HTML documents are described by HTML tags
• Each HTML tag describes different document content
A small HTML document:
<!DOCTYPE html> <html>
<head>
<title>Page Title</title> </head>
<body>
<h1>My First Heading</h1>
<p>My first paragraph.</p> </body>
</html>
Example Explained
• The DOCTYPE declaration defines the document type to be HTML
• The text between <html> and </html> describes an HTML document
• The text between <head> and </head> provides
I will be getting my Beginner's HTML Knowledge from a website called w3schools.
  Here is the link to the HTML Intro: http://www.w3schools.com/html/html_intro.asp
  information about the document
• The text between <title> and </title> provides a title
for the document
• The text between <body> and </body> describes the • The text between <html> and </html> describes an
HTML document
• The text between <head> and </head> provides
 information about the document
• The text between <title> and </title> provides a title
for the document
• The text between <body> and </body> describes the
visible page content
• The text between <h1> and </h1> describes a heading
• The text between <p> and </p> describes a paragraph
Using this description, a web browser can display a document with a heading and a paragraph.

<h2>HTML Tags</h2>
HTML tags are keywords (tag names) surrounded by angle brackets:
<tagname>content</tagname>
• HTML tags normally come in pairs like <p> and </p>
• The first tag in a pair is the start tag, the second tag is
the end tag
• The end tag is written like the start tag, but with
a slash before the tag name
Web Browsers
The purpose of a web browser (Chrome, IE, Firefox, Safari) is to read HTML documents and display them.
The browser does not display the HTML tags, but uses them to determine how to display the document:
    The start tag is often called the opening tag. The end tag is often called the closing tag.
             HTML Page Structure
Below is a visualization of an HTML page structure: <html>
<head>
<title>Page title</title>
</head> <body>
<h1>This is a heading</h1> <p>This is a paragraph.</p> <p>This is another paragraph.</p>
</body>
</html>
Only the <body> area (the white area) is displayed by the browser.
  </body>
</html>
    Only the <body> area (the white area) is displayed by the browser.
 The <!DOCTYPE> Declaration
The <!DOCTYPE> declaration helps the browser to display a web page correctly.
There are different document types on the web.
To display a document correctly, the browser must know both type and version.
The doctype declaration is not case sensitive. All cases are acceptable:
<!DOCTYPE html> <!DOCTYPE HTML> <!doctype html> <!Doctype Html>
Common Declarations
HTML5
<!DOCTYPE html>
(Example declarations for HTML 4.01 and XHTML 1.0 are on the tutorial page, but I didn't write them down because w3schools uses HTML5 and I won't need the older versions.)
HTML Versions
Since the early days of the web, there have been many versions of HTML:
 Version
 Year
HTML 1991 HTML 2.0 1995
                   HTML 3.2 1997
   Since the early days of the web, there have been many versions of
 HTML:
Version Year
          HTML
HTML 2.0
1991
    1995
     HTML 3.2
1997
  HTML 4.01
1999
     XHTML
2000
    HTML5
2014
 -----

<h2>HTML Basic Examples</h2>
Don't worry if these examples use tags you have not learned. You will learn about them in the next chapters.

HTML Documents
All HTML documents must start with a type declaration: <! DOCTYPE html>.
The HTML document itself begins with <html> and ends with </html>.
The visible part of the HTML document is between <body> and </body>.
Example
<!DOCTYPE html> <html>
<body>
<h1>My First Heading</h1>
<p>My first paragraph.</p>
</body> </html>

HTML Headings
HTML headings are defined with the <h1> to <h6> tags:
 </body>
</html>
HTML Headings
HTML headings are defined with the <h1> to <h6> tags: Example
<h1>This is a heading</h1> <h2>This is a heading</h2> <h3>This is a heading</h3>

HTML Paragraphs
HTML paragraphs are defined with the <p> tag: Example
<p>This is a paragraph.</p> <p>This is another paragraph.</p>

HTML Links
HTML links are defined with the <a> tag: Example
<a href="http://www.w3schools.com">This is a link</a>
The link's destination is specified in the href attribute. Attributes are used to provide additional information about HTML elements.

HTML Images
HTML images are defined with the <img> tag.
The source file (src), alternative text (alt), and size (width and height) are provided as attributes:
 <img src="w3schools.jpg" alt="W3Schools.com" width="104" heig ht="142">
Example
You will learn more about attributes in a later chapter.
 (width and height) are provided as attributes:
 <img src="w3schools.jpg" alt="W3Schools.com" width="104" heig ht="142">
You will learn more about attributes in a later chapter.

HTML Elements
HTML documents are made up by HTML elements. HTML Elements
HTML elements are written with a start tag, with an end tag, with the content in between: <tagname>content</tagname>
The HTML element is everything from the start tag to the end tag: <p>My first HTML paragraph.</p>
Some HTML elements do not have an end tag. Nested HTML Elements
HTML elements can be nested (elements can contain elements). All HTML documents consist of nested HTML elements.
This example contains 4 HTML elements:
Example
<!DOCTYPE html> <html>
<body>
  Start tag
  Element content
  End tag
  <h1>
 My First Heading
  </h1>
   <p>
My first paragraph.
 </p>
 <br>
     <h1>My First Heading</h1> <p>My first paragraph.</p>
Example
 <!DOCTYPE html> <html>
<body>
 <h1>My First Heading</h1> <p>My first paragraph.</p>
</body> </html>
HTML Example Explained
The <html> element defines the whole document.
It has a start tag <html> and an end tag </html>.
The element content is another HTML element (the <body>
element).
<html>
<body>
<h1>My First Heading</h1> <p>My first paragraph.</p>
</body> </html>
The <body> element defines the document body.
It has a start tag <body> and an end tag </body>.
The element content is two other HTML elements (<h1> and
<p>).
<body>
<h1>My First Heading</h1>
<p>My first paragraph.</p>
</body>
The <h1> element defines a heading.
It has a start tag <h1> and an end tag </h1>. The element content is: My First Heading.
<h1>My First Heading</h1>
The <p> element defines a paragraph.
It has a start tag <p> and an end tag </p>.
The element content is: My first paragraph. <p>My first paragraph.</p>
 The element content is: My First Heading.
<h1>My First Heading</h1>
The <p> element defines a paragraph.
 It has a start tag <p> and an end tag </p>. The element content is: My first paragraph.
<p>My first paragraph.</p>

Don't Forget the End Tag
Some HTML elements will display correctly, even if you forget the end tag:
Example
<html> <body>
<p>This is a paragraph <p>This is a paragraph
</body> </html>
The example above works in all browsers, because the closing tag is considered optional.
Never rely on this. It might produce unexpected results and/or errors if you forget the end tag.

Empty HTML Elements
HTML elements with no content are called empty elements. <br> is an empty element without a closing tag (the <br> tag defines a line break).
Empty elements can be "closed" in the opening tag like this: <br />.
HTML5 does not require empty elements to be closed. But if you want stricter validation, or you need to make your document readable by XML parsers, you should close all HTML elements.
HTML tags are not case sensitive: <P> means the same as <p>.
HTML Tip: Use Lowercase Tags
The HTML5 standard does not require lowercase tags, but
 want stricter validation, or you need to make your document
readable by XML parsers, you should close all HTML elements.
 HTML tags are not case sensitive: <P> means the same as <p>. The HTML5 standard does not require lowercase tags, but
W3C recommends lowercase in HTML4, and demands lowercase
for stricter document types like XHTML.
At W3Schools we always use lowercase tags. -----
HTML Attributes
Attributes provide additional information about HTML elements.

<h2>HTML Attributes</h2>
• HTML elements can have attributes
• Attributes provide additional information about an element
• Attributes are always specified in the start tag
• Attributes come in name/value pairs like: name="value"

The lang Attribute
The document language can be declared in the <html> tag. The language is declared in the lang attribute.
Declaring a language is important for accessibility applications
(screen readers) and search engines:
<!DOCTYPE html> <html lang="en-US"> <body>
<h1>My First Heading</h1> <p>My first paragraph.</p>
</body> </html>
The first two letters specify the language (en). If there is a dialect, use two more letters (US).
HTML Tip: Use Lowercase Tags

The title Attribute
 </body> </html>
 The first two letters specify the language (en). If there is a dialect, use two more letters (US).
The title Attribute
HTML paragraphs are defined with the <p> tag.
In this example, the <p> element has a title attribute. The value of the attribute is "About W3Schools":
Example
<p title="About W3Schools">
W3Schools is a web developer's site.
It provides tutorials and references covering
many aspects of web programming,
including HTML, CSS, JavaScript, XML, SQL, PHP, ASP, etc.
</p>
When you move the mouse over the element, the title will be displayed as a tooltip.

The href Attribute
HTML links are defined with the <a> tag. The link address is specified in the href attribute:
Example
<a href="http://www.w3schools.com">This is a link</a> You will learn more about links and the <a> tag later in this tutorial.

Size Attributes
HTML images are defined with the <img> tag.
The filename of the source (src), and the size of the image (width and height) are all provided asattributes:
<img src="w3schools.jpg" width="104" height="142">
The image size is specified in pixels: width="104" means 104
Example
 (width and height) are all provided asattributes:
 <img src="w3schools.jpg" width="104" height="142">
The image size is specified in pixels: width="104" means 104 screen pixels wide.
You will learn more about images and the <img> tag later in this tutorial.

The alt Attribute
The alt attribute specifies an alternative text to be used, when an HTML element cannot be displayed.
The value of the attribute can be read by "screen readers". This way, someone "listening" to the webpage, i.e. a blind person, can "hear" the element.
Example
<img src="w3schools.jpg" alt="W3Schools.com" width="104" heig ht="142">

<h2>We Suggest: Always Use Lowercase</h2>
Attributes
The HTML5 standard does not require lower case attribute names. The title attribute can be written with upper or lower case
like Title and/or TITLE.
W3C recommends lowercase in HTML4, and demands lowercase for stricter document types like XHTML.
Lower case is the most common. Lower case is easier to type. At W3Schools we always use lower case attribute names.
We Suggest: Always Quote Attribute Values
The HTML5 standard does not require quotes around attribute values.
Example
 We Suggest: Always Quote Attribute
Values
 The HTML5 standard does not require quotes around attribute values.
The href attribute, demonstrated above, can be written as:
Example
<a href=http://www.w3schools.com>
W3C recommends quotes in HTML4, and demands quotes for stricter document types like XHTML.
Sometimes it is necessary to use quotes. This will not display correctly, because it contains a space:
Example
<p title=About W3Schools>
Using quotes are the most common. Omitting quotes can produce errors. At W3Schools we always use quotes around attribute values.
Single or Double Quotes?
Double style quotes are the most common in HTML, but single
style can also be used.
In some situations, when the attribute value itself contains double
quotes, it is necessary to use single quotes:
<p title='John "ShotGun" Nelson'> Or vice versa:
<p title="John 'ShotGun' Nelson"> Chapter Summary
• All HTML elements can have attributes
• The HTML title attribute provides additional "tool-tip"
information
• The HTML href attribute provides address information for links
• The HTML width and height attributes provide size
information for images
• The HTML alt attribute provides text for screen readers
• At W3Schools we always use lowercase HTML attribute
names
                                                    information
• The HTML href attribute provides address information for links
• The HTML width and height attributes provide size
 information for images
• The HTML alt attribute provides text for screen readers
• At W3Schools we always use lowercase HTML attribute
names
• At W3Schools we always quote attributes with double quotes
HTML Attributes
Below is an alphabetical list of some attributes often used in HTML:
Attribut Description e
alt Specifies an alternative text for an image
disabled Specifies that an input element should be disabled
href Specifies the URL (web address) for a link
id Specifies a unique id for an element
src Specifies the URL (web address) for an image
style Specifies an inline CSS style for an element
title Specifies extra information about an element (displayed as a tool tip)
A complete list of all attributes for each HTML element, is listed in
our: HTML Tag Reference. -----

<h2>HTML Headings</h2>
Headings are important in HTML documents.
HTML Headings
Headings are defined with the <h1> to <h6> tags.
<h1> defines the most important heading. <h6> defines the least important heading.
Example
<h1>This is a heading</h1> <h2>This is a heading</h2>
<h3>This is a heading</h3>
 important heading.
Example
 <h1>This is a heading</h1> <h2>This is a heading</h2> <h3>This is a heading</h3>
Note: Browsers automatically add some empty space (a margin) before and after each heading.
Headings Are Important
Use HTML headings for headings only. Don't use headings to make text BIG or bold.
Search engines use your headings to index the structure and content of your web pages.
Users skim your pages by its headings. It is important to use headings to show the document structure.
h1 headings should be main headings, followed by h2 headings, then the less important h3, and so on.

HTML Horizontal Rules
The <hr> tag creates a horizontal line in an HTML page. The hr element can be used to separate content:
Example
<p>This is a paragraph.</p> <hr>
<p>This is a paragraph.</p> <hr>
<p>This is a paragraph.</p>

The HTML <head> Element
The HTML <head> element has nothing to do with HTML headings.
displayed.
The HTML <head> element is placed between the <html> tag and
The HTML <head> element contains meta data. Meta data are not the <body> tag:
 The HTML <head> element has nothing to do with HTML headings.
 displayed.
The HTML <head> element is placed between the <html> tag and the <body> tag:
Example
<!DOCTYPE html> <html>
<head>
<title>My First HTML</title> <meta charset="UTF-8">
</head>
<body> .
.
.
Meta data means data about data. HTML meta data is data about the HTML document.

The HTML <title> Element
The HTML <title> element is meta data. It defines the HTML document's title.
The title will not be displayed in the document, but might be displayed in the browser tab.

The HTML <meta> Element
The HTML <meta> element is also meta data.
It can be used to define the character set, and other information about the HTML document.
More Meta Elements
The HTML <head> element contains meta data. Meta data are not
In the chapter about HTML styles you discover more meta
                                            about the HTML document.
 More Meta Elements
In the chapter about HTML styles you discover more meta elements:
The HTML <style> element is used to define internal CSS style sheets.
The HTML <link> element is used to define external CSS style sheets.
HTML Tip - How to View HTML Source
Have you ever seen a Web page and wondered "Hey! How did they do that?"
To find out, right-click in the page and select "View Page Source" (in Chrome) or "View Source" (in IE), or similar in another browser. This will open a window containing the HTML code of the page.

HTML Tag Reference
W3Schools' tag reference contains additional information about these tags and their attributes.
You will learn more about HTML tags and attributes in the next chapters of this tutorial.
Tag
<html> <body> <head>
<h1> to <h6>
<hr>
-----
Description
Defines an HTML document
Defines the document's body
Defines the document's head element Defines HTML headings
Defines a horizontal line

HTML Paragraphs
HTML documents are divided into paragraphs.
              <h1> to <h6> Defines HTML headings
<hr> Defines a horizontal line -----
 HTML Paragraphs
HTML documents are divided into paragraphs.
HTML Paragraphs
The HTML <p> element defines a paragraph. Example
<p>This is a paragraph</p> <p>This is another paragraph</p>
Browsers automatically add some white space before and after a paragraph. HTML Display
You cannot be sure how HTML will be displayed.
Large or small screens, and resized windows will create different results.
With HTML, you cannot change the output by adding extra spaces or extra lines in your HTML code.
The browser will remove extra spaces and extra lines when the page is displayed.
Any number of spaces, and any number of new lines, count
as only one space.
Example
<p>
This paragraph contains a lot of lines in the source code, but the browser ignores it.
</p>
<p>
This paragraph
      but the browser ignores it. </p>
 <p>
This paragraph
contains a lot of spaces in the source code,
but the browser
ignores it.
</p>
Don't Forget the End Tag
Most browsers will display HTML correctly even if you forget the end tag:
Example
<p>This is a paragraph <p>This is another paragraph
The example above will work in most browsers, but do not rely on it.
Forgetting the end tag can produce unexpected results or errors.
Stricter versions of HTML, like XHTML, do not allow you to skip the end tag.

HTML Line Breaks
The HTML <br> element defines a line break.
Use <br> if you want a line break (a new line) without starting a new paragraph:
Example
<p>This is<br>a para<br>graph with line breaks</p>
The <br> element is an empty HTML element. It has no end tag.
This poem will display as one line:
The Poem Problem Example
                     The <br> element is an empty HTML element. It has no end tag.
 This poem will display as one line:
Example
<p>
My Bonnie lies over the ocean.
My Bonnie lies over the sea.
My Bonnie lies over the ocean.
Oh, bring back my Bonnie to me.
</p>

The HTML <pre> Element
The HTML <pre> element defines preformatted text.
The text inside a <pre> element is displayed in a fixed-width font (usually Courier), and it preserves both spaces and line breaks:
Example
<pre>
My Bonnie lies over the ocean.
My Bonnie lies over the sea.
My Bonnie lies over the ocean.
Oh, bring back my Bonnie to me.
</pre>
HTML Tag Reference
W3Schools' tag reference contains additional information about HTML elements and their attributes.
Tag Description
<p> Defines a paragraph
The Poem Problem
<br> Inserts a single line break
                              W3Schools' tag reference contains additional information about HTML elements and their attributes.
 Tag Description
<p> Defines a paragraph
<br> Inserts a single line break <pre> Defines pre-formatted text -----

<h2>HTML Styles HTML Styles</h2>
I am red
I am blue
<!DOCTYPE html> <html>
<body>
<h2 style="color:red;">I am red</h2> <h2 style="color:blue;">I am blue</h2>
</body> </html>
The HTML Style Attribute
Setting the style of an HTML element, can be done with the style attribute.
The HTML style attribute has the following syntax: style="property:value;"
The property is a CSS property. The value is a CSS value. You will learn more about CSS later in this tutorial.

HTML Background Color
The background-color property defines the background color for an HTML element:
 You will learn more about CSS later in this tutorial.
HTML Background Color
 The background-color property defines the background color for an HTML element:
This example sets the background for a page to lightgrey:
Example
<body style="background-color:lightgrey;"> <h1>This is a heading</h1>
<p>This is a paragraph.</p> </body>
HTML Text Color
The color property defines the text color for an HTML element: Example
<h1 style="color:blue;">This is a heading</h1> <p style="color:red;">This is a paragraph.</p>

HTML Fonts
The font-family property defines the font to be used for an HTML element:
Example
<h1 style="font-family:verdana;">This is a heading</h1> <p style="font-family:courier;">This is a paragraph.</p>

HTML Text Size
The font-size property defines the text size for an HTML element:
<h1 style="font-size:300%;">This is a heading</h1> <p style="font-size:160%;">This is a paragraph.</p>
Example
 The font-size property defines the text size for an HTML element:
 <h1 style="font-size:300%;">This is a heading</h1> <p style="font-size:160%;">This is a paragraph.</p>

HTML Text Alignment
The text-align property defines the horizontal text alignment for an HTML element:
Example
<h1 style="text-align:center;">Centered Heading</h1> <p>This is a paragraph.</p>
Chapter Summary
• Use the style attribute for styling HTML elements
• Use background-color for background color
• Use color for text colors
• Use font-family for text fonts
• Use font-size for text sizes
• Use text-align for text alignment
-----
HTML Text Formatting Elements
Text Formatting
This text is bold
This text is italic
This is superscript

HTML Formatting Elements
In the previous chapter, you learned about HTML styling, using the HTML style attribute.
HTML also defines special elements for defining text with a
Example
 HTML Formatting Elements
In the previous chapter, you learned about HTML styling, using the HTML style attribute.
HTML also defines special elements for defining text with a special meaning.
HTML uses elements like <b> and <i> for formatting output, like bold or italic text.
Formatting elements were designed to display special types of
text:
• Bold text
• Important text
• Italic text
• Emphasized text
• Marked text
• Small text
• Deleted text
• Inserted text
• Subscripts
• Superscripts

HTML Bold and Strong Formatting
The HTML <b> element defines bold text, without any extra
importance.
Example
<p>This text is normal.</p>
<p><b>This text is bold.</b></p>
The HTML <strong> element defines strong text, with added semantic "strong" importance.
Example
<p>This text is normal.</p>
 HTML Italic and Emphasized Formatting
<p><strong>This text is strong</strong>.</p>
 <p>This text is normal.</p>
 HTML Italic and Emphasized Formatting The HTML <i> element defines italic text, without any extra importance.
Example
<p>This text is normal.</p>
<p><i>This text is italic</i>.</p>
The HTML <em> element defines emphasized text, with added semantic importance.
Example
<p>This text is normal.</p>
<p><em>This text is emphasized</em>.</p>
Browsers display <strong> as <b>, and <em> as <i>.
However, there is a difference in the meaning of these tags: <b> and <i> defines bold and italic text,
but <strong> and <em> means that the text is "important".
HTML Small Formatting
The HTML <small> element defines small text: Example
<h2>HTML <small>Small</small> Formatting</h2>
HTML Marked Formatting
The HTML <mark> element defines marked or highlighted text: Example
<h2>HTML <mark>Marked</mark> Formatting</h2> HTML Deleted Formatting
<p><strong>This text is strong</strong>.</p>
                            The HTML <mark> element defines marked or highlighted text:
Example
 <h2>HTML <mark>Marked</mark> Formatting</h2>
HTML Deleted Formatting
The HTML <del> element defines deleted (removed) text. Example
<p>My favorite color is <del>blue</del> red.</p>
HTML Inserted Formatting
The HTML <ins> element defines inserted (added) text. Example
<p>My favorite <ins>color</ins> is red.</p>
HTML Subscript Formatting
The HTML <sub> element defines subscripted text. Example
<p>This is <sub>subscripted</sub> text.</p>
HTML Superscript Formatting
The HTML <sup> element defines superscripted text. Example
<p>This is <sup>superscripted</sup> text.</p> HTML Text Formatting Elements Tag Description
<b> Defines bold text
<em> Defines emphasized text
<i> Defines italic text
                                                                               HTML Text Formatting Elements
Tag Description
 <b> <em> <i> <small> <strong> <sub> <sup> <ins> <del> <mark> -----
Defines bold text
Defines emphasized text Defines italic text
Defines smaller text
Defines important text
Defines subscripted text Defines superscripted text Defines inserted text
Defines deleted text
Defines marked/highlighted text
HTML Quotation and Citation
Elements
Quotation
Here is a quote from WWF's website:
For 50 years, WWF has been protecting the future of nature. The world's leading conservation organization, WWF works in 100 countries and is supported by 1.2 million members in the United States and close to 5 million globally.
HTML <q> for Short Quotations
The HTML <q> element defines a short quotation.
Browsers usually insert quotation marks around the <q> element.
Example
<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>
HTML <blockquote> for Long Quotations
The HTML <blockquote> element defines a quoted section.
 <p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>
 HTML <blockquote> for Long Quotations
The HTML <blockquote> element defines a quoted section. Browsers usually indent <blockquote> elements.
Example
<p>Here is a quote from WWF's website:</p>
<blockquote cite="http://www.worldwildlife.org/who/index.html"> For 50 years, WWF has been protecting the future of nature.
The world's leading conservation organization,
WWF works in 100 countries and is supported by
1.2 million members in the United States and
close to 5 million globally.
</blockquote>
HTML <abbr> for Abbreviations
The HTML <abbr> element defines an abbreviation or an acronym.
Marking abbreviations can give useful information to browsers, translation systems and search-engines.
Example
<p>The <abbr title="World Health Organization"> WHO</abbr> was founded in 1948.</p>
HTML <address> for Contact Information
The HTML <address> element defines contact information (author/owner) of a document or article.
The <address> element is usually displayed in italic. Most browsers will add a line break before and after the element.
<address>
Written by John Doe.<br>
Example
                                            browsers will add a line break before and after the element.
 <address>
Written by John Doe.<br> Visit us at:<br> Example.com<br>
Box 564, Disneyland<br> USA
</address>
HTML <cite> for Work Title
The HTML <cite> element defines the title of a work. Browsers usually display <cite> elements in italic.
Example
<p><cite>The Scream</cite> by Edward Munch. Painted in 1893.</p>
HTML <bdo> for Bi-Directional Override
The HTML <bdo> element defines bi-directional override.
The <bdo> element is used to override the current text direction:
Example
<bdo dir="rtl">This text will be written from right to left</bdo> HTML Quotation and Citation Elements
Tag
<abbr> <address>
<bdo>
Description
Defines an abbreviation or acronym
Defines contact information for the author/owner of a document
Defines the text direction
<blockquote Defines a section that is quoted from another source >
<cite> Defines the title of a work
Example
                                    a document
<bdo> Defines the text direction
<blockquote >
<cite> <q>
Defines a section that is quoted from another source
Defines the title of a work Defines a short inline quotation
 -----
<h2>HTML Computer Code Elements</h2>
Computer Code Element
<code>
var x = 5;
var y = 6; document.getElementById("demo").innerHTML = x + y; </code>
HTML Computer Code Formatting
HTML normally uses variable letter size and spacing.
This is not wanted when displaying examples of computer code. The <kbd>, <samp>, and <code> elements all support fixed letter size and spacing.
HTML <kbd> For Keyboard Input
The HTML <kbd> element defines keyboard input: Example
<kbd>File | Open...</kbd> Result:
File | Open...
HTML <samp> For Computer Output
The HTML <samp> element defines sample output from a
computer program:
Example
 HTML <samp> For Computer Output
The HTML <samp> element defines sample output from a
 computer program:
Example
<samp>
demo.example.com login: Apr 12 09:10:17
Linux 2.6.10-grsec+gg3+e+fhs6b+nfs+gr0501+++p3+c4a+gr2b- reslog-v6.189
</samp>
Result:
demo.example.com login: Apr 12 09:10:17 Linux 2.6.10- grsec+gg3+e+fhs6b+nfs+gr0501+++p3+c4a+gr2b-reslog-v6.189
HTML <code> For Computer Code The HTML <code> element defines a piece of programming code:
Example
<code>
var x = 5;
var y = 6; document.getElementById("demo").innerHTML = x + y; </code>
Result:
var x = 5; var y = 6; document.getElementById("demo").innerHTML = x + y;
Notice that the <code> element does not preserve extra whitespace and line-breaks.
To fix this, you can put the <code> element inside
a <pre> element:
Example
<pre> <code> var x = 5; var y = 6;
document.getElementById("demo").innerHTML = x + y;
</code> </pre>
Result:
                                            <code>
var x = 5; var y = 6;
document.getElementById("demo").innerHTML = x + y;
</code> </pre>
Result:
var x = 5;
var y = 6; document.getElementById("demo").innerHTML = x + y;
HTML <var> For Variables
The HTML <var> element defines a variable.
The variable could be a variable in a mathematical expression or a variable in programming context:
Example
Einstein wrote: <var>E</var> = <var>m</var><var>c</var> <sup>2</sup>.
Result:
Einstein wrote: E = mc2.
HTML Computer Code Elements
 Tag
<code>
<kbd>
<samp>
<var>
<pre>
-----
<h2>Description</h2>
Defines programming code Defines keyboard input Definescomputeroutput Defines a variable
Defines preformatted text
HTML Comments
Comment tags <!-- and --> are used to insert comments in HTML.
HTML Comment Tags
You can add comments to your HTML source by using the following syntax:
 Comment tags <!-- and --> are used to insert comments in HTML.
HTML Comment Tags
 You can add comments to your HTML source by using the following
syntax:
<!-- Write your comments here -->
Note: There is an exclamation point (!) in the opening tag, but not in the closing tag. Comments are not displayed by the browser, but they can help
document your HTML.
With comments you can place notifications and reminders in your HTML:
Example
<!-- This is a comment -->
<p>This is a paragraph.</p>
<!-- Remember to add more information here -->
Comments are also great for debugging HTML, because you can comment out HTML lines of code, one at a time, to search for errors:
Example
<!-- Do not display this at the moment
<img border="0" src="pic_mountain.jpg" alt="Mountain"> -->
Conditional Comments
You might stumble upon conditional comments in HTML:
<!--[if IE 8]>
.... some HTML here ....
<![endif]-->
Conditional comments defines HTML tags to be executed by Internet Explorer only.
Software Program Tags
HTML comments tags can also be generated by various HTML
                                        Conditional comments defines HTML tags to be executed by
Internet Explorer only.
Software Program Tags
HTML comments tags can also be generated by various HTML software programs.
For example <!--webbot bot--> tags wrapped inside HTML comments by FrontPage and Expression Web.
As a rule, let these tags stay, to help support the software that created them.
-----
<h2>HTML Colors</h2>
TVs and computer screens display colors by combining Red, Green, and Blue light.
Color Names
With CSS, colors can be set by using color names:
Example
Color Name
Red Orange Yellow Cyan Blue
CSS supports 140 standard color names.
RGB (Red, Green, Blue)
With HTML, RGB color values can be specified using this formula:
 rgb(red, green, blue)
Each parameter (red, green, and blue) defines the intensity of the color between 0 and 255.
For example, rgb(255,0,0) is displayed as red, because red is set
                                                                               RGB (Red, Green, Blue)
With HTML, RGB color values can be specified using this formula:
rgb(red, green, blue)
Each parameter (red, green, and blue) defines the intensity of the color between 0 and 255.
For example, rgb(255,0,0) is displayed as red, because red is set to its highest value (255) and the others are set to 0. Experiment by mixing the RGB values below:
Red Green Blue
255 0 0 rgb(255, 0, 0)
Example
Color RGB
rgb(255,0,0) rgb(255,255,0) rgb(0,255,0) rgb(0,255,255) rgb(0,0,255)
Shades of gray are often defined using equal values for all the 3 light sources:
Example
Color RGB
rgb(0,0,0) rgb(128,128,128) rgb(255,255,255)
Hexadecimal Colors
With HTML, RGB values can also be specified using hexadecimal color values in the form: #RRGGBB, where RR (red), GG (green)
 and BB (blue) are hexadecimal values between 00 and FF (same as decimal 0-255).
For example, #FF0000 is displayed as red, because red is set to its
                                                                   With HTML, RGB values can also be specified using hexadecimal color values in the form: #RRGGBB, where RR (red), GG (green)
 and BB (blue) are hexadecimal values between 00 and FF (same as decimal 0-255).
For example, #FF0000 is displayed as red, because red is set to its highest value (FF) and the others are set to the lowest value (00).
Example
Color HEX
#FF0000 #FFFF00 #00FF00 #00FFFF #0000FF
Shades of gray are often defined using equal values for all the 3 light sources:
Example
Color HEX
#000000 #808080 #FFFFFF
-----
<h2>HTML Styles - CSS</h2>
CSS = Styles and Colors
Manipulate Text
Colors, Boxes
Styling HTML with CSS
CSS stands for Cascading Style Sheets
    Colors, Boxes
Styling HTML with CSS
CSS stands for Cascading Style Sheets
Styling can be added to HTML elements in 3 ways:
• Inline - using a style attribute in HTML elements
• Internal - using a <style> element in the HTML <head>
section
• External - using one or more external CSS files
The most common way to add styling, is to keep the styles in separate CSS files. But, in this tutorial, we use internal styling, because it is easier to demonstrate, and easier for you to try it yourself.
You can learn much more about CSS in our CSS Tutorial. Inline Styling (Inline CSS)
Inline styling is used to apply a unique style to a single HTML element:
Inline styling uses the style attribute.
This example changes the text color of the <h1> element to blue:
Example
<h1 style="color:blue;">This is a Blue Heading</h1> Internal Styling (Internal CSS)
Internal styling is used to define a style for one HTML page. Internal styling is defined in the <head> section of an HTML page, within a <style> element:
Example
<!DOCTYPE html> <html>
<head>
 <style>
body {background-color:lightgrey;} h1 {color:blue;}
p {color:green;}
 <!DOCTYPE html> <html>
<head>
 <style>
body {background-color:lightgrey;} h1 {color:blue;}
p {color:green;}
</style>
</head>
<body>
<h1>This is a heading</h1> <p>This is a paragraph.</p>
</body> </html>
External Styling (External CSS)
An external style sheet is used to define the style for many pages. With an external style sheet, you can change the look of an entire web site by changing one file!
To use an external style sheet, add a link to it in
the <head> section of the HTML page: Example
<!DOCTYPE html> <html>
<head>
<link rel="stylesheet" href="styles.css"> </head>
<body>
<h1>This is a heading</h1> <p>This is a paragraph.</p>
</body> </html>
An external style sheet can be written in any text editor. The file
should not contain any html tags. The style sheet file must be saved with a .css extension.
Here is how the "styles.css" looks:
 </body>
</html>
An external style sheet can be written in any text editor. The file
 should not contain any html tags. The style sheet file must be
saved with a .css extension.
Here is how the "styles.css" looks: body {
background-color: lightgrey; }
h1 {
color: blue;
}
p{ color:green;
}
CSS Fonts
The CSS color property defines the text color to be used for the HTML element.
The CSS font-family property defines the font to be used for the HTML element.
The CSS font-size property defines the text size to be used for the HTML element.
Example
<!DOCTYPE html> <html>
<head>
<style>
h1 {
color: blue; font-family: verdana; font-size: 300%;
} p{
color: red; font-family: courier; font-size: 160%;
}
 font-size: 300%;
} p{
color: red; font-family: courier; font-size: 160%;
}
</style> </head> <body>
<h1>This is a heading</h1> <p>This is a paragraph.</p>
</body> </html>
The CSS Box Model
Every HTML element has a box around it, even if you cannot see it.
The CSS border property defines a visible border around an HTML element: Example
p{
border: 1px solid black; }
The CSS padding property defines a padding (space) inside the border:
Example
p{
border: 1px solid black; padding: 10px;
}
The CSS margin property defines a margin (space) outside the border:
Example
 p{
border: 1px solid black; padding: 10px;
margin: 30px;
 Example
 p{
border: 1px solid black; padding: 10px; margin: 30px;
}
The CSS examples above use px to define sizes in pixels. The id Attribute
All the examples above use CSS to style HTML elements in a general way.
To define a special style for one special element, first add an id attribute to the element:
<p id="p01">I am different</p>
then define a style for the element with the specific id:
Example
#p01 {
color: blue;
}
The class Attribute
To define a style for a special type (class) of elements, add a class attribute to the element:
<p class="error">I am different</p>
Now you can define a different style for elements with the specific class:
Example
p.error { color: red;
}
Use id to address a single element. Use class to address groups of elements.
Chapter Summary
• Use the HTML style attribute for inline styling
                       }
Use id to address a single element. Use class to address groups of elements.
 Chapter Summary
• Use the HTML style attribute for inline styling
• Use the HTML <style> element to define internal CSS
• Use the HTML <link> element to refer to an external CSS file
• Use the HTML <head> element to store <style> and <link>
elements
• Use the CSS color property for text colors
• Use the CSS font-family property for text fonts
• Use the CSS font-size property for text sizes
• Use the CSS border property for visible element borders
• Use the CSS padding property for space inside the border
• Use the CSS margin property for space outside the border
HTML Style Tags
Tag Description
<style> Defines style information for an HTML document <link> Defines a link between a document and an external
resource
-----
<h2>HTML Links</h2>
Links are found in nearly all web pages. Links allow users to click their way from page to page.
HTML Links - Hyperlinks
HTML links are hyperlinks.
A hyperlink is a text or an image you can click on, and jump to another document.
HTML Links - Syntax
In HTML, links are defined with the <a> tag:
<a href="url">link text</a>
   another document.
HTML Links - Syntax
In HTML, links are defined with the <a> tag: <a href="url">link text</a>
Example
<a href="http://www.w3schools.com/html/">Visit our HTML tutorial</a>
The href attribute specifies the destination address (http://www.w3schools.com/html/)
The link text is the visible part (Visit our HTML tutorial). Clicking on the link text, will send you to the specified address.
The link text does not have to be text. It can be an HTML image or any other HTML element.
Without a trailing slash on subfolder addresses, you might generate two requests to the server. Many servers will automatically add a trailing slash to the address, and then create a new request.
Local Links
The example above used an absolute URL (A full web address). A local link (link to the same web site) is specified with a relative URL (without http://www....).
Example
<a href="html_images.asp">HTML Images</a> HTML Links - Colors
When you move the mouse over a link, two things will normally
happen:
• The mouse arrow will turn into a little hand
• The color of the link element will change
By default, a link will appear like this (in all browsers):
 • An unvisited link is underlined and blue
• A visited link is underlined and purple
• An active link is underlined and red
                                       • The mouse arrow will turn into a little hand
• The color of the link element will change
By default, a link will appear like this (in all browsers):
 • An unvisited link is underlined and blue
• A visited link is underlined and purple
• An active link is underlined and red
You can change the default colors, by using styles:
Example
<style>
a:link {color:green; background-color:transparent; text- decoration:none}
a:visited {color:pink; background-color:transparent; text- decoration:none}
a:hover {color:red; background-color:transparent; text- decoration:underline}
a:active {color:yellow; background-color:transparent; text- decoration:underline}
</style>
HTML Links - The target Attribute
The target attribute specifies where to open the linked document. This example will open the linked document in a new browser window or in a new tab:
Example
<a href="http://www.w3schools.com/" target="_blank">Visit W3Schools!</a>
Target Value
_blank _self
_parent _top
Description
Opens the linked document in a new window or tab
Opens the linked document in the same frame as it was clicked (this is default)
Opens the linked document in the parent frame Opens the linked document in the full body of the
framename Opens the linked document in a named frame
If your webpage is locked in a frame, you can use target="_top" to
window
                   _parent Opens the linked document in the parent frame window
_top Opens the linked document in the full body of the
 framename Opens the linked document in a named frame
If your webpage is locked in a frame, you can use target="_top" to
break out of the frame:
Example
<a href="http://www.w3schools.com/html/" target="_top">HTML5 tutorial!</a>
HTML Links - Image as Link
It is common to use images as links:
Example
<a href="default.asp">
<img src="smiley.gif" alt="HTML
tutorial"style="width:42px;height:42px;border:0">
</a>
border:0 is added to prevent IE9 (and earlier) from displaying a border around the image.
HTML Links - Create a Bookmark
HTML bookmarks are used to allow readers to jump to specific parts of a Web page.
Bookmarks are practical if your website has long pages.
To make a bookmark, you must first create the bookmark, and then add a link to it.
When the link is clicked, the page will scroll to the location with the bookmark.
Example
First, create a bookmark with the id attribute:
<h2 id="tips">Useful Tips Section</h2>
Then, add a link to the bookmark ("Useful Tips Section"), from within the same page:
                Example
First, create a bookmark with the id attribute:
<h2 id="tips">Useful Tips Section</h2>
Then, add a link to the bookmark ("Useful Tips Section"), from
within the same page:
<a href="#tips">Visit the Useful Tips Section</a>
Or, add a link to the bookmark ("Useful Tips Section"), from another page:
Example
<a href="html_tips.html#tips">Visit the Useful Tips Section</a> Chapter Summary
• Use the HTML <a> element to define a link
• Use the HTML href attribute to define the link address
• Use the HTML target attribute to define where to open the
linked document
• Use the HTML <img> element (inside <a>) to use an image
as a link
• Use the HTML id attribute (id="value") to define bookmarks in
a page
• Use the HTML href attribute (href="#value") to link to the
bookmark
HTML Link Tags
Tag Description
<a> Defines a hyperlink -----
HTML Images Example
<!DOCTYPE html> <html>
 <body>
<h2>Spectacular Mountain</h2>
<img src="pic_mountain.jpg" alt="Mountain
 <!DOCTYPE html> <html>
<body>
<h2>Spectacular Mountain</h2>
<img src="pic_mountain.jpg" alt="Mountain View"style="width:304px;height:228px;">
</body>
</html>
Always specify the width and height of an image. If width and height are not specified, the page will flicker while the image loads.
HTML Images Syntax
In HTML, images are defined with the <img> tag.
The <img> tag is empty, it contains attributes only, and does not
have a closing tag.
The src attribute specifies the URL (web address) of the image:
<img src="url" alt="some_text"> The alt Attribute
The alt attribute specifies an alternate text for an image, if the image cannot be displayed.
The alt attribute provides alternative information for an image if a user for some reason cannot view it (because of slow connection, an error in the src attribute, or if the user uses a screen reader). If a browser cannot find an image, it will display the alt text:
Example
<img src="wrongname.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
The alt attribute is required. A web page will not validate correctly without it.
 HTML Screen Readers
 The alt attribute is required. A web page will not validate correctly
without it.
 HTML Screen Readers
A screen reader is a software program that can read what is displayed on a screen.
Screen readers are useful to people who are blind, visually impaired, or learning disabled.
Screen readers can read the alt attribute.
Image Size - Width and Height
You can use the style attribute to specify the width and height of an image.
The values are specified in pixels (use px after the value):
Example
<img src="html5.gif" alt="HTML5
Icon" style="width:128px;height:128px;">
Alternatively, you can use width and height attributes. Here, the values are specified in pixels by default:
Example
<img src="html5.gif" alt="HTML5 Icon" width="128" height="128">
Width and Height or Style?
Both the width, height, and style attributes are valid in the latest HTML5 standard.
We suggest you use the style attribute. It prevents styles sheets from changing the original size of images:
Example
<!DOCTYPE html> <html>
<head>
<style>
 Example
 <!DOCTYPE html> <html>
<head>
<style>
img { width:100%;
}
</style> </head> <body>
<img src="html5.gif" alt="HTML5
Icon" style="width:128px;height:128px;"> <img src="html5.gif" alt="HTML5
Icon" width="128" height="128">
</body> </html>
Images in Another Folder
If not specified, the browser expects to find the image in the same folder as the web page.
However, it is common to store images in a sub-folder. You must then include the folder name in the src attribute:
Example
<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
Images on Another Server
Some web sites store their images on image servers. Actually, you can access images from any web address in the world:
Example
<img src="http://www.w3schools.com/images/w3schools_green.jp
g"alt="W3Schools.com">
 Actually, you can access images from any web address in the world:
Example
<img src="http://www.w3schools.com/images/w3schools_green.jp g"alt="W3Schools.com">
Animated Images
The GIF standard allows animated images:
Example
<img src="programming.gif" alt="Computer Man" style="width:48px;height:48px;">
Note that the syntax of inserting animated images is no different from non-animated images.
Using an Image as a Link
To use an image as a link, simply nest the <img> tag inside the <a> tag:
Example
<a href="default.asp">
<img src="smiley.gif" alt="HTML
tutorial"style="width:42px;height:42px;border:0;">
</a>
Add "border:0;" to prevent IE9 (and earlier) from displaying a border around the image.
Image Floating
Use the CSS float property to let the image float.
The image can float to the right or to the left of a text:
Example
 <p>
<img src="smiley.gif" alt="Smiley
face"style="float:right;width:42px;height:42px;">
 The image can float to the right or to the left of a text:
Example
 <p>
<img src="smiley.gif" alt="Smiley face"style="float:right;width:42px;height:42px;"> The image will float to the right of the text.
</p>
<p>
<img src="smiley.gif" alt="Smiley face"style="float:left;width:42px;height:42px;"> The image will float to the left of the text.
</p>
Image Maps
Use the <map> tag to define an image-map. An image-map is an image with clickable areas.
The name attribute of the <map> tag is associated with the <img>'s usemap attribute and creates a relationship between the image and the map.
The <map> tag contains a number of <area> tags, that defines the clickable areas in the image-map:
Example
<img src="planets.gif" alt="Planets" usemap="#planetmap"style= "width:145px;height:126px;">
<map name="planetmap">
<area shape="rect" coords="0,0,82,126" alt="Sun" href="sun.ht
m">
<area shape="circle" coords="90,58,3" alt="Mercury" href="mer
cur.htm">
<area shape="circle" coords="124,58,8" alt="Venus" href="venu
s.htm"> </map>
Chapter Summary
• Use the HTML <img> element to define an image
                               s.htm"> </map>
Chapter Summary
• Use the HTML <img> element to define an image
• Use the HTML src attribute to define the URL of the image
• Use the HTML alt attribute to define an alternate text for an
image, if it cannot be displayed
• Use the HTML width and height attributes to define the size
of the image
• Use the CSS width and height properties to define the size of
the image (alternatively)
• Use the CSS float property to let the image float
• Use the HTML <map> element to define an image-map
• Use the HTML <area> element to define the clickable areas in
the image-map
• Use the HTML <img>'s element usemap attribute to point to
an image-map
Loading images takes time. Large images can slow down your page. Use images carefully.
HTML Image Tags
Tag
<img>
<map>
<area>
Description
Defines an image
Defines an image-map
Defines a clickable area inside an image-map
-----
(STOPPED AT "HTML Tables" on 02/03/16)
