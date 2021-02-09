
# CSS
## block and inline elements:
Block level elements look like they start on a new line.
Inline elements flow within the text and do not start on a new line.

- CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.
- CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a selector and a declaration.

- CSS declarations sit inside curly brackets and each is made up of two parts: a property and value, separated by a colon.

**ex:**

h1, h2, h3 {
font-family: Arial;
color: yellow;}

## Using External CSS:
we prepare a separated css page then we put this element inside the head tag to link it with html:<link href="css/styles.css" type="text/css"
rel="stylesheet" /> 

### WHY USE EXTERNAL CSS?
When building a website there are several advantages to placing your CSS rules in a separate style sheet.

* All of your web pages can share the same style sheet.
* Therefore, once the user has downloaded the CSS stylesheet,the rest of the site will load faster.
* the one CSS style sheet, rather than changing the CSS rules on every page.

## Using Internal CSS:
EXAMPLE:
<!DOCTYPE html>
<html>
<head>
<title>Using Internal CSS</title>
<style type="text/css">
body {
font-family: arial;
background-color: rgb(185,179,175);}
h1 {
color: rgb(255,255,255);}
</style>
</head>
<body>
<h1>Potatoes</h1>
<p>There are dozens of different potato
varieties. They are usually described as
early, second early and maincrop.</p>
</body>
</html>

## Inheritance:
If you specify the font-family or color properties on the <body> element, they will apply
to most child elements. This is because the value of the font-family property is inherited by child elements. It saves you from having to apply these properties to as many elements (and results in simpler style sheets).

## CSS SUMMARY:
- CSS treats each HTML e XX lement as if it appears inside its own box and uses rules to indicate how that element should look.
-  Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like).
- Different types of selectors allow you to target your rules at different elements.
- Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.
- CSS rules usually appear in a separate document, although they may appear within an HTML page.