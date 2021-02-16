# html (ch 4,15) and JS (ch 3)

The < a> tag indicates where the hyperlink starts and the < /a> tag indicates where it ends. Whatever text gets added inside these tags, will work as a hyperlink. Add the URL for the link in the < a href=” ”>. Just keep in mind that you should use the < a>…< /a> tags inside < body>…< /body> tags.

Ex: < a href="/about/about\*team.htm">team< /a>
\*\*\_On larger websites**\* it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories.
Structure The diagram on the right shows the directory structure for a fictional entertainment listings website called ExampleArts. The top-level folder is known as the root folder. (In this example, the root folder is called examplearts.) The root folder contains all of the other files and folders for a website.
Home pages
The main homepage of a site written in HTML (and the home pages of each section in a child folder) is called index.html.
**Absolute Hyperlinks**
Absolute hyperlinks are complete addresses that contain all the elements of a URL. They always start with some version of http:// followed by the domain name (for example, www.designisphilosophy.com) and optionally a page/folder. Absolute hyperlinks are used when linking to pages outside of the current site that have a different domain name.
**Relative Hyperlinks**
Relative hyperlinks are addresses that are relative to the current domain or location. They only contain the name of the target page prefixed with any necessary folder moves (for example, default.html).
**_Same Folder_**
To link to a file in the same folder, just use the file name. (Nothing else is needed.)
**_Child Folder_**
For a child folder, use the name of the child folder, followed by a forward slash, then the file name.
To link to music listings from the homepage:
< a href="music/listings.html">Listings< /a>
**_Grandchild Folder_**
Use the name of the child folder, followed by a forward slash, then the name of the grandchild folder, followed by another forward slash, then the file name.
To link to DVD reviews from the homepage:
< a href="movies/dvd/reviews.html">
Reviews< /a>
**_Parent Folder_**
Use ../ to indicate the folder above the current one, then follow it with the file name.
Ex:
To link to the homepage from the music reviews:
< a href="../index.html">Home< /a>
**_Grand Parent Folder_**
Repeat the ../ to indicate that you want to go up two folders (rather than one), then follow it with the file name.
To link to the homepage from the DVD reviews:
< a href="../../index.html">Home< /a>
**Root-relative Hyperlinks\*\*
Root-relative hyperlinks are a subset of relative hyperlinks in which all the links are assumed to start from the root folder (domain name) of the site. They differ from the relative hyperlinks in that the address is prefixed by a forward slash (for example, /default.html).

### How to create mailto link in HTML

The mailto link is written like regular link with extra parameters inside the href attribute:
< a href="mailto:name@email.com">Link text</ a>
| Parameter            |  Description                     |
|----------------------|----------------------------------|
|mailto:name@email.com | e-mail recipient address         |
|cc=name@email.com     | carbon copy e-mail address       |
|bcc=name@email.com    | blind carbon copy e-mail address |
|subject=subject text  | subject of e-mail                |
|body=body text        | body of e-mail                   |
|?                     | first parameter delimiter        |
|&                     | other parameters delimiter       |

**Inside the < a> tag there is an attribute for target**
Values of the target Attribute: 
* _blank: Opens the linked document in a new tab or window.
* _parent: 	Opens the link in the parent frame. Frames are deprecated in HTML5.
* _self: Open the link in the current frame.
* _top:	Opens the link in the top-most frame. Frames are deprecated in HTML5.


- inking to a Specific Part of the Same Page
Using the id selector
In CSS, "id" is a selector that is used to designate an area that a link should point to, similar to anchor in HTML. The nice thing about using id is you can create a link to any element on the page, rather than only the top or bottom. In the following sections, you'll see how to apply id to an HTML tag, and then how to link to it. This example will link to the opening paragraph at the top of this page.

**create links to sections on the same page**
1. Using #top or #bottom
The following examples use #top and #bottom with the <a> tag and href attribute to link to that section of the page. This method is similar to using "id," but you don't have to pick a specific element. Click "Top" or "Bottom" in the Results section to see what happens.

2. Using the id selector
In CSS, "id" is a selector that is used to designate an area that a link should point to, similar to anchor in HTML. The nice thing about using id is you can create a link to any element on the page, rather than only the top or bottom. In the following sections, you'll see how to apply id to an HTML tag, and then how to link to it. This example will link to the opening paragraph at the top of this page.

# Key Concepts in Positioning Elements
Building Blocks
CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.
**Block-level elements**
start on a new line Examples include: < h1> < p> < ul> < li>
**Inline elements**
 flow in between surrounding text Examples include: < img> < b> < i>

**To use positioning** on an element, you must first declare its position property, which specifies the type of positioning method used for an element. Using the position property values, the elements are positioned using the top, bottom, left, and right properties. They also work differently depending on their position value.

- There are five types of positioning values:

1. static
2. relative
3. fixed
4. absolute
5. sticky

**Page Sizes**
Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide
(since most users will be able to see designs this wide on their screens).

**Fixed Width Layouts**
fixed width layout designs do not change size as the user increases or decreases the size of their browser window.
Measurements tend to be given in pixels.

**Advantages**
-  Pixel values are accurate at controlling size and positioning of elements.
- The designer has far greater control over the appearance and position of items on the page than with liquid layouts.
- You can control the lengths of lines of text regardless of the size of the user's window.
- The size of an image will always remain the same relative to the rest of the page.

**Disadvantages**
- You can end up with big gaps around the edge of a page.
- If the user's screen is a much higher resolution than the designer's screen, the page can look smaller and text can be harder to read.
- If a user increases font sizes, text might not fit into the allotted spaces.
- The design works best on devices that have a site or resolution similar to that of desktop or laptop computers.
- The page will often take up more vertical space than a liquid layout with the same content.

**Liquid Layouts**
Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.
**Advantages**
1. Pages expand to fill the entire browser window so there are no spaces around the page on a large screen.
2. If the user has a small window, the page can contract to fit it without the user having to scroll to the side.
3. The design is tolerant of users setting font sizes larger than the designer intended (because the page can stretch).

**Disadvantages**
1. If you do not control the width of sections of the page then the design can look very different than you intended, with unexpected gaps around certain elements or items squashed together.
2. If the user has a wide window, lines of text can become very long, which makes them harder to read.
3. If the user has a very narrow window, words may be squashed and you can end up with few words on each line.
4. If a fixed width item (such as an image) is in a box that is too small to hold it (because the user has made the
window smaller) the image can overflow over the text.

**A Fixed Width Layout**
To create a fixed width layout, the width of the main boxes on a page will usually be specified in pixels (and sometimes their height, too).
**Layout Grids**
Many designers use a grid structure to help them position items on a page, and the same is true for web designers.

**CSS Frameworks**
CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.

# JAVASCRIPT

 a **function** is a "subprogram" that can be called by code external (or internal in the case of recursion) to the function. Like the program itself, a function is composed of a sequence of statements called the function body. Values can be passed to a function, and the function will return a value.

In JavaScript, functions are first-class objects, because they can have properties and methods just like any other object. What distinguishes them from other objects is that functions can be called. In brief, they are Function objects.

Every function in JavaScript is a Function object. See Function for information on properties and methods of Function objects.

To return a value other than the default, a function must have a return statement that specifies the value to return. A function without a return statement will return a default value. In the case of a constructor called with the new keyword, the default value is the value of its this parameter. For all other functions, the default return value is undefined.

The parameters of a function call are the function's arguments. Arguments are passed to functions by value. If the function changes the value of an argument, this change is not reflected globally or in the calling function. However, object references are values, too, and they are special: if the function changes the referred object's properties, that change is visible outside the function, as shown in the following example:

ex:

/* Declare the function 'myFunc' */
function myFunc(theObject) {
  theObject.brand = "Toyota";
}

/*
 *Declare variable 'mycar';
 *create and initialize a new Object;
 *assign reference to it to 'mycar'
 */
var mycar = {
  brand: "Honda",
  model: "Accord",
  year: 1998
};

/* Logs 'Honda' */
console.log(mycar.brand);

/* Pass object reference to the function */
myFunc(mycar);

/*
 *Logs 'Toyota' as the value of the 'brand' property
 *of the object, as changed to by the function.
 */
console.log(mycar.brand);
The this keyword does not refer to the currently executing function, so you must refer to Function objects by name, even within the function body.

There is a special syntax for declaring functions (see function statement for details):

function name([param], [param], ... [param]) {
   statements
}

