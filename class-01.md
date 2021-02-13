## Class- 01 Read :
### How the Web Works

- connect to the web, you do so via an Internet Service Provider (ISP).
- Your computer contacts a network of servers called Domain Name System (DNS), then tell your computer the IP address associated with the requested domain name.

- IP address allows your browser to contact the web server that hosts the website you requested.

- The web server then sends the page you requested back to your web browser.


## HTML Describes the Structure of Pages

**Ex:**

<html>
<body>
<h1>This is the Main Heading</h1>
<p>This text might be an introduction to the rest of
the page. And if the page is a long one it might
be split up into several sub-headings.<p>
<h2>This is a Sub-Heading</h2>
<p>Many long articles have sub-headings so to help
you follow the structure of what is being written.
There may even be sub-sub-headings (or lower-level
headings).</p>
<h2>Another Sub-Heading</h2>
<p>Here you can see another sub-heading.</p>
</body>
</html>



## HTML Uses Elements to Describe the Structure of Pages called Tags 

Tags act like containers.
 They tell you something about the information that lies between their opening and closing tags.
- Tags has attributes: 
Attributes provide additional information about the contents of an element. They appear on the opening tag of the element and are made up of two parts: a name and a value, separated by an equals sign.
**Ex:** <p lang="en-us">Paragraph in English</p>

## HTML files should saved with ( .html ) extension

**Summary**
-	HTML pages are text documents.
-	HTML uses tags (characters that sit inside angled brackets) to give the information they surround special meaning.
-	Tags are often referred to as elements.
-	Tags usually come in pairs. The opening tag denotes the start of a piece of content; the closing tag denotes the end.
-	Opening tags can carry attributes, which tell us more about the content of that element.
-	Attributes require a name and a value.
-	To learn HTML you need to know what tags are available for you to use, what they do, and where they can go.

- in html <!-- comment goes here -->
- DOCTYPES tell browsers which version of HTML you are using.
 - The id and class attributes allow you to identify particular elements.

**Ex:** <p class="important">

*Block Elements:*

Some elements will always appear to start on a new line in the browser window. These are known as block level elements.
Examples of block elements are
<h1>, <p>, <ul>, and <li>.

*Inline Elements:*

Some elements will always appear to continue on the same line as their neighbouring elements. These are known as inline elements.
Examples of inline elements are
<a>, <b>, <em>, and <img>.

## Grouping Text & Elements In a Block
<div>
The <div> element allows you to group a set of elements together in one block-level box.

**Ex:** 
<div id="header">
<img src="images/logo.gif" alt="Anish Kapoor" />
<ul>
<li><a href="index.html">Home</a></li>
<li><a href="biography.html">Biography</a></li>
<li><a href="works.html">Works</a></li>
<li><a href="contact.html">Contact</a></li>
</ul>
</div><!-- end of header -->

## Grouping Text & Elements Inline:
<span> 
The <span> element acts like an inline equivalent of the <div> element. It is used to either:
1. Contain a section of text where there is no other suitable element to differentiate it from its surrounding text
2. Contain a number of inline elements.
Ex:
<p>Anish Kapoor won the Turner Prize in 1991 and
exhibited at the <span class="gallery">Tate
Modern</span> gallery in London in 2003.</p>

**Iframes:**
An iframe is like a little window that has been cut into your page — and in that window you can see another page. The term iframe is an abbreviation of inline frame.

**Ex:**
<iframe
width="450"
height="350"
src="http://maps.google.co.uk/maps?q=moma+new+york
&amp;output=embed">
</iframe>


- The <meta> tag allows you to supply all kinds of information about your web page.
Escape characters are used to include special characters in your pages such as <, >, and ©.


**Example**
### HTML5 LAYOUT


margin: 10px 0px 5px 0px;
padding: 0px;}
h3 {
margin: 0px 0px 10px 0px;
color: #de6581;}
aside h2 {
padding: 30px 0px 10px 0px;
color: #de6581;}
footer {
font-size: 80%;
padding: 7px 0px 0px 20px;}
</style>
<!--[if lt IE 9]>
<script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
<![endif]-->
</head>
<body>
<div class="wrapper">
<header>
<h1>Yoko's Kitchen</h1>
<nav>
<ul>
<li><a href="" class="current">home</a></li>
<li><a href="">classes</a></li>
<li><a href="">catering</a></li>
<li><a href="">about</a></li>
<li><a href="">contact</a></li>
</ul>
</nav>
</header>
<section class="courses">
<article>
<figure>
<img src="images/bok-choi.jpg" alt="Bok Choi" />
<figcaption>Bok Choi</figcaption>
</figure>
<hgroup>
<h2>Japanese Vegetarian</h2>
<h3>Five week course in London</h3>
</hgroup>


## HTML5 Layout:
HTML has several semantic elements that define the different parts of a web page:
-	<header> - Defines a header for a document or a section
-	<nav> - Defines a set of navigation links
-	<section> - Defines a section in a document
-	<article> - Defines an independent, self-contained content
-	<aside> - Defines content aside from the content (like a sidebar)
-	<footer> - Defines a footer for a document or a section
-	<details> - Defines additional details that the user can open and close on demand
-	<summary> - Defines a heading for the <details> element

•	The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure.
•	 The new elements provide clearer code (compared with using multiple
elements).
•	 Older browsers that do not understand HTML5 elements need to be told which elements are block-level elements.
•	To make HTML5 elements work in Internet Explorer 8 (and older versions of IE), extra JavaScript is needed, which is available free from Google.

### WireFrame:
A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require.

### Summary:
-	It's important to understand who your target audience is, why they would come to your site, what information they want to find and when they are likely to return.
-	 Site maps allow you to plan the structure of a site.
-	 Wireframes allow you to organize the information that will need to go on each page.
-	 Design is about communication. Visual hierarchy helps visitors understand what you are trying to tell them.
-	 You can differentiate between pieces of information using size, color, and style.
-	 You can use grouping and similarity to help simplify the information you present.


## javascript
You can use JavaScript to add or select elements, attributes, and text to the page, or remove them.
- REACT TO EVENTS You can specify that a script should run when a specific event has occurred.
- JavaScript language can be used to tell browsers what you want them to do.
- A script is a series of instructions that a computer can follow to achieve a goal.
### WRITING A SCRIPT

 To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it.

Start with the big picture of what you want to achieve, and break that down into smaller steps:
1. DEFINE THE GOAL 
2. DESIGN THE SCRIPT 
3. CODE EACH STEP

### RULES FOR NAMING VARIABLES:
1.	The name must begin with a letter, dollar sign ($),or anunderscore (_).
2.	The name can contain letters,numbers, dollar sign ($), or an underscore (_).
3.	You cannot use keywords or reserved words.
4.	All variables are case sensitive.
5.	Use a name that describes the kind of information that the variable stores.
6.	If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word.

### Types of operator:
•	ASSIGNMENT OPERATORS
•	COMPARISON OPERATORS
•	ARITHMETIC OPERATORS
•	LOGICAL OPERATORS
•	STRING OPERATORS

### summary:
•	A script is made up of a series of statements. Each statement is like a step in a recipe.
•	Scripts contain very precise instructions. For example,you might specify that a value must be remembered before creating a calculation using that value.
•	Variables are used to temporarily store pieces of information used in the script.
•	Arrays are special types of variables that store more than one piece of related information.
•	JavaScript distinguishes between numbers (0-9),strings (text), and Boolean values (true or false).
•	Expressions evaluate into a single value.
•	Expressions rely on operators to calculate a value.





