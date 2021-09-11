# Introductory HTML and JavaScript

## HTML Book ( Chapters:1,8,17,18)

### What is HTML?
- HTML stands for Hyper Text Markup Language
- HTML is the standard markup language for creating Web pages
- HTML describes the structure of a Web page
- HTML consists of a series of elements
- HTML elements tell the browser how to display the content
- HTML elements label pieces of content such as "this is a heading", "this is a paragraph", "this is a link", etc.

### A Simple HTML Document
    <!DOCTYPE html>    
    <html>    
    <head>    
    <title>Page Title</title>
    </head>
    <body>

    <h1>My First Heading</h1>
    <p>My first paragraph.</p>

    </body>
     </html>

-     The <!DOCTYPE html> declaration defines that this document is an HTML5 document
-     The <html> element is the root element of an HTML page
-     The <head> element contains meta information about the HTML page
-     The <title> element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
-     The <body> element defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
-     The <h1> element defines a large heading
-     The <p> element defines a paragraph

### What is an HTML Element?
An HTML element is defined by a start tag, some content, and an end tag:

    <tagname>Content goes here...</tagname>
The HTML element is everything from the start tag to the end tag:

    <h1>My First Heading</h1>
    <p>My first paragraph.</p>

### HTML versions 

#### HTML 4
This version is very stable, having been released in December 1999. This version added support for style sheets and scripting ability for multimedia elements.

#### XHTML
 XHTML is an application of XML, a more restrictive subset of SGML. XHTML documents are well-formed and may therefore be parsed using standard XML parsers, unlike HTML, which requires a lenient HTML-specific parser

#### HTML 5
HTML5 is still a work in progress, and all major browsers support many of the new HTML5 elements and APIs. Its core aim have been to improve the language with support for the latest multimedia while keeping it easily readable by humans and consistently understood by computers and devices.

### Comments in HTML
    Comment is a piece of code which is ignored by any web browser. It is a good practice to add comments into your HTML code, especially in complex documents, to indicate sections of a document, and any other notes to anyone looking at the code. Comments help you and others understand your code and increases code readability.

    HTML comments are placed in between <!-- ... --> tags. So, any content placed with-in <!-- ... --> tags will be treated as comment and will be completely ignored by the browser.
 
![comments in html](https://www.w3resource.com/w3r_images/html-comment.png)

### ID Attribute & Class Attribute
| Id | Class |
| --- | ----- |
| It is used to uniquely identify that element from other elements on the page. Its value should start with a letter or an underscore (not a number or any other character). | identify several elements as being different from the other elements on the page 

###  Elements

    Block Elements :   <h1>,     <p>,     <ul>, and     <li>. 
     Inline Elements :     <a>,     <b>,     <em>, and     <img>.
     Grouping Text & Elements In a Block :     <div> 
    Grouping Text & Elements Inline :     <span>  

### HTML5
 The tags (elements) have been introduced in HTML5:

| tag | Description |
| ------ | --------- | 
| '<'rticle'>' | Represents an independent piece of content of a document, such as a blog entry or newspaper article |
| '<'aside '>' | Represents a piece of content that is only slightly related to the rest of the page |
| '<'embed'>' | Defines external interactive content or plugin. |
| '<'footer'>' | Represents a footer for a section and can contain information about the author, copyright information, et cetera | 
| '<'header'>' | Represents a group of introductory or navigational aids |
| '<'hgroup'>' | Represents the header of a section. |
| '<'nav'>' | Represents a section of the document intended for navigation. |
| '<'section'>' | Represents a generic document or application section |

![Html5](https://www.freetimelearning.com/html5/images/html5-basic-Layout.jpg)

## JavaScript Book (Chapter 1)

### The ABC of programming 

#### A : What is a script and how do i creat one ? 
- A script is a series of instructions that the computer can follow to achieve a task or goal.
- TO write a script break your idea or your goal to a set of tasks, that will make it esier to build and you can also use a flowchart to help!

#### B : How do computers fit in with the world around them ?
- Computers creat models of the world using data
- Programms can write the code to say " when this event occurs run the code "
- Web browsers use HTMl to create a model of the web page.
- To make eb pages interactive you write code that uses the browser's model of the web page.

#### C : How do i write a script fo a wep page ?
- It is best to keep JavaScript code in its own JavaScript file. JavaScript files are text files (like HTML pages and CSS style sheets), but they have the . j s extension
- The HTML '<'script'>' element is used in HTML pages
to tell the browser to load the JavaScript file (rather like the '<'link'>' element can be used to load a CSS file).
- If you view the source code of the page in the browser, the JavaScript will not have changed the HTML, because the script works with the model of the web page that the browser has created.

![ABC of programming](https://sonsuzdesign.files.wordpress.com/2020/04/javascript-lessons-1.jpg?w=1200)
