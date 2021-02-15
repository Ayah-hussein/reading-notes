# HTML and JAVASCRIPT
we have two kinds of markup:

● Structural markup: the elements that you can use to describe both headings and paragraphs.

● Semantic markup: which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms, and so on.

**HTML has six "levels" of headings:**
Browsers display the contents of headings at different sizes. The contents of an < h1> element is the largest, and the contents of an < h6> element is the smallest.

**< p> : paragraph**
By default, a browser will show each paragraph on a new line with some space between it and any subsequent paragraphs.

**Bold & Italic:**

-	Bold: By enclosing words in the tags < b> we can make characters appear bold.

-	Italic: By enclosing words in the tags < i > and </ i> we can make characters appear italic.


**Superscript & Subscript:**

**Superscript:** The < sup> element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power such as 22.

**Subscript:** The < sub> element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20.

**White Space:**

When the browser comes across two or more spaces next to each other, it only displays one space. Similarly if it comes across a line break, it treats that as a single space too. This is known as white space collapsing.

**Line break and Horizontal rule:**

**< /br>:** if you wanted to add a line break inside the middle of a paragraph you can use the line break tag < br />.
**< hr/>:** you can add a horizontal rule between sections using the < hr /> tag.

***Visual Editors & Their Code views***

- *Visual editors* often resemble word processors. Although each editor will differ slightly, there are some features that are common to most editors that allow you to control the presentation of text.

- *Code views* show you the code created by the visual editor so you can manually edit it, or so you can just enter new code yourself. It is often activated using a button with an icon that says HTML or has angled brackets. White space may be added to the code by the editor to make the code easier to read.

**Strong & Emphasis:**
The use of the < strong> element indicates that its content has strong importance. By default browsers will show the contents of an < strong> element in bold.

**< em>:** The < em> element indicates emphasis that subtly changes the meaning of a sentence. By default browsers will show the contents of an < em> element in italic.

**Semantic Markup**

There are elements that are not intended to affect the structure of your web pages, but they do add extra information to the pages — they are known as semantic markup.
Em, blockqoute, strong, main, footer, header >>> considered as semantic tags.

- < blockquote>
The < blockquote> element is used for longer quotes that take up an entire paragraph. Note how the < p> element is still used inside the < blockquote> element.

- < q>
The < q> element is used for shorter quotes that sit within a paragraph.

***Abbreviations***

If you use an abbreviation or an acronym, then the < abbr> element can be used. A title attribute on the opening tag is used to specify the full term.

- < cite>
When you are referencing a piece of work such as a book, film or research paper, the < cite> element can be used to indicate where the citation is from.

- < dfn> 
The < dfn> element is used to indicate the defining instance of a new term.

**Author Details**

The < address> element has quite a specific use: to contain contact details for the author of the page.

**Changes to Content**

- < ins>/  < del> :
The < ins> element can be used to show content that has been inserted into a document, while the < del> element can show text that has been deleted from it.

- < s>
The < s> element indicates something that is no longer accurate or relevant (but that should not be deleted). Visually the content of an < s> element will usually be displayed with a line through the center.


**Understanding CSS:**

The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element.

**CSS could used:**
1.	Inline    - inside the tag using the style attribute.
2.	Internal - should placed in the head
3.	External  ex: < link href="css/styles.css" type="text/css" rel="stylesheet" /> this tag placed inside the head.

-	CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

-	CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.

-	CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.


**CSS Selectors:**
-	CSS selector allow you to target rules to specific elements in an HTML document.
-	CSS selectors are case sensitive, so they must match element names and attribute values exactly.


**Inheritance:**
If you specify the font-family or color properties on the element, they will apply to most child elements. This is because the value of the font-family property is inherited by child elements. It saves you from having to apply these properties to as many elements (and results in simpler style sheets).

**CSS Summary:**
1.	CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that  element should look.
2.	 Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like).
3.	 Different types of selectors allow you to target your rules at different elements.
4.	 Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.
5.	 CSS rules usually appear in a separate document, although they may appear within an HTML page.



# The A B C of programming:

**PLACING THE SCRIPT IN THE PAGE**

You may see JavaScript in the HTML between opening < script> and closing < /script> tags (but it is better to put scripts in their own files).

-	JAVASCRIPT RUNS WHERE IT IS FOUND IN THE HTML
-	When the browser comes across a < script> element, it stops to load the script and then checks to see if it needs to do anything.

***How do I write a script in a web page?***

1.	It is best to keep JavaScript code in its own JavaScript file. JavaScript files are text files (like HTML pages and CSS style sheets), but they have the . j s extension . 

2.	The HTML < script> element is used in HTML pages to tell the browser to load the JavaScript file (rather like the < link> element can be used to load a CSS file).

3.	If you view the source code of the page in the browser, the JavaScript will not have changed the HTML, because the script works with the model of the web page that the browser has created.

**STATEMENTS**

A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon.

-	JAVASCRIPT IS CASE SENSITIVE
-	STATEMENTS ARE INSTRUCTIONS AND EACH ONE STARTS ON A NEW LINE.
-	STATEMENTS CAN BE ORGANIZED INTO CODE BLOCKS
-	Comments in javascript : /* This script displays a greeting to the user based upon the current time. It is an example from JavaScript & jQuery book */ - this is for multi-line comments
-	SINGLE-LINE COMMENTS we use //
-	A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.
-	Variables declared as :
Var name= “ahmad” 


**RULES FOR NAMING VARIABLES:**

1.	The name must begin with a letter, dollar sign ($),or anunderscore (_).

2.	The name can contain letters,numbers, dollar sign ($), or an underscore (_).

3.	You cannot use keywords or reserved words.

4.	All variables are case sensitive.

5.	Use a name that describes the kind of information that the variable stores.

6.	If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word.

### Javascript data types are:
1.	Boolean data type 
2.	string data type 
3.	numeric data type 

### ARRAYS

An array is a special type of variable. It doesn't just store one value; it stores a list of values.

### EXPRESSIONS

An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions.

1.	EXPRESSIONS THAT JUST ASSIGN  a VALUE TO A VARIABLE
2.	EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE

JavaScript includes following categories of operators.
1.	Arithmetic Operators  (+ , - , *  , ++ , -- , / , % )
2.	Comparison Operators ( > , < , == , === , ! = , > = , < = )
3.	Logical Operators          (  && , || , ! )
4.	Assignment Operators  ( = ,  += ,  - = , * = , / = , % =  )
5.	Conditional Operators   

### CREATING A DATE OBJECT:

-	The getTime() Method
             The getTime() method returns the number of milliseconds since January 1, 1970
-	The getFullYear() Method
             The getFullYear() method returns the year of a date as a four digit number.
**Summary:**
-	Functions allow you to group a set of related statements together that represent a single task.
-	Functions can take parameters (information required to do their job) and may return a value.
-	An object is a series of variables and functions that represent something from the world around you.
-	In an object, variables are known as properties of the object; functions are known as methods of the object.
-	Web browsers implement objects that represent both the browser window and the document loaded into the browser window.
-	JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts.
-	Arrays and objects can be used to create complex data sets (and both can contain the other).

### LOOPS
there are two components to a decision:
-	an expression is evaluated, which returns a value.
-	a conditional statement says what to do in a given situation
1. **if condition:** if the condition returns true executethe statments between the first set of curly brackets, otherwise execute the statment between the secod set of curly brackets.
 example:
 if (average > 50) 
{  document.write('you passed');  }
 else {  document.write('you fail')  }

2.	**if else statment:** if ... else statement allows you to provide two sets of code:

-	 one set if the condition evaluates to true
-	another set if the condition is false

3. **Switch:**
A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value. 

