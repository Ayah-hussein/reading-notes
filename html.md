## Summary for html (3 , 13 ch) and JS (2 , 4 ch) 

**HTML** offers authors several mechanisms for specifying lists of information. All lists must contain one or more list elements. Lists may contain:
1.	**Unordered list**
Ex:
 < UL>
< LI> Unordered information. 
< LI> Ordered information. 
< LI> Definitions. 
< /UL>

2.	**Ordered list**

Ex:
 < oL>
< LI>ordered information.< /li> 
< LI>Ordered information. < /li>
< LI>Definitions. < /li>
 < /oL>

3.	**Definitions** : used to define terminology ,and  consist of a series of term/definition pairs
< dl> : list is created with the < dl> element
< dt> :This is used to contain the term being defined (the definition term).
< dd>: This is used to contain the definition.

Ex:
< DL>
< DT> < STRONG>Lower cost </ STRONG>
< DD>The new version of this product costs significantly less than the
previous one!
< DT> < STRONG>Easier to use < /STRONG>
< DD>We've changed the product so that it's much easier to use!
< DT> < STRONG>Safe for kids </ STRONG>
< DD>You can leave your kids alone in a room with this product and
they won't get hurt (not a guarantee).
< /DL>

***Nested lists:***
Ex:
< ul>
< li> Mousses < /li>
< li> Pastries
< ul>
< li> Croissant< /li>
< li> Mille-feuille< /li>
< li> Palmier< /li>
< li> Profiterole < /li>
< /ul>
< /li>
< li>Tarts< /li>
< /ul>


#### Overflowing Content:

The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:
- *Hidden:* 
This property simply hides any extra content that does not fit in the box.
- *Scroll:*
This property adds a scrollbar to the box so that users can scroll to see the missing content.

### Border, Margin & Padding

**Border**
Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.
**Margin**
Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.
**Padding**
Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.

 

***Border Width***
The border-width property is used to control the width of a border.
using one of the following values:   thin  , medium  , thick

**Border Style**

You can control the style of a border using the border-style property. This property can take the following values:
p.one {border-style: solid;}
p.two {border-style: dotted;}


 **Border Color**
It is possible to individually control the colors of the borders on different sides of a box using:
-	border-top-color
-	border-right-color
-	border-bottom-color
-	border-left-color
also possible to use a shorthand to control all four border colors in the one property: 
 *border-color*

**Shorthand border:**

The border property allows you to specify the width, style and color of a border in one property (and the values should be coded in that specific order).

**Centering Content**
Once you have specified the width of the box, setting the left and right margins to auto will make the browser put an equal gap on each side of the box.
 **Change Inline/Block display:**

- inline
This causes a block-level element to act like an inline element.
- block
This causes an inline element to act like a block-level element.
- inline-block
This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.
- none
This hides an element from the page.

**Hiding Boxes (visibility):**
The visibility property allows you to hide boxes from users but It leaves a space where the element would have been.
- hidden
This hides the element.
- visible
This shows the element.

## SS3: Border Images

The border-image property applies an image to the border of any box. It takes a background image and slices it into nine pieces.

This property requires three pieces of information:
1. The URL of the image
2. Where to slice the image
3. What to do with the straight edges; the possible values are:

-	stretch stretches the image
-	repeat repeats the image
-	round like repeat but if the tiles do not fit exactly, scales the tile image so the will.

### CSS 3: Box Shadows

*The box-shadow property* allows you to add a drop shadow around a box (text-shadow property)

- Horizontal offset
Negative values position the shadow to the left of the box.

- Vertical offset
Negative values position the shadow to the top of the box.

- Blur distance If omitted, the shadow is a solid line like a border.

- Spread of shadow : If used, a positive value will cause the shadow to expand in all directions, and a negative value will make it contract.

### CSS 3: Rounded Corners
CSS3 introduces the ability to create rounded corners on any box, using a property called border-radius.

You can specify individual values for each corner of a box using:
-	border-top-right-radius
-	border-bottom-right-radius
-	border-bottom-left-radius
-	border-top-left-radius

### CSS 3: Elliptical Shapes: 

To create more complex shapes, you can specify different distances for the horizontal and the vertical parts of the rounded corners.

 **Book summary:**
- CSS treats each HTML element as if it has its own box.
- You can use CSS to control the dimensions of a box.
- You can also control the borders, margin and padding for each box with CSS.
- It is possible to hide elements using the display and visibility properties.
-  Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.
-  Legibility can be improved by controlling the width of boxes containing text and the leading.
-  CSS3 has introduced the ability to create image borders and rounded borders.


# JAVASCRIT section:

**USING QUOTES INSIDE A STRING**
Sometimes you will want to use a double or single quote mark within a string.
Because strings can live in single or double quotes, if you just want to use double quotes in the string, you could surround the entire string in single quotes.
escaping the quotation characters. 
This is done by using a backwards slash (or "backslash" ) before any type of quote mark that appears within a string
A Boolean variable can only have a value of true or false

**SHORTHAND FOR CREATING VARIABLES**

1. Variables are declared and values assigned in the same statement.
2. Three variables are declared on the same line, then values assigned to each.
3. Two variables are declared and assigned values on the same line. Then one is declared and assigned a value on the next line.
4. Here, a variable is used to hold a reference to an element in the HTML page.

**To change a variable value :**
You just use the variable name, the equals sign, and the new value for that attribute.
if condition: if the condition returns true execute the statements between the first set of curly brackets, otherwise execute the statement between the second set of curly brackets.
 example: 
     if (average > 50) {
     document.write('you passed'); }
      else 
      {document.write('you fail')} 


**if else statement** : Here you can see that an if ... else statement allows you to provide two sets of code:
1. one set if the condition evaluates to true
2.	another set if the condition is false

**switch:**
A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

**USING FOR LOOPS**
A for loop is often used to loop through the items in an array.

**The While Loop**
Loops can execute a block of code as long as a specified condition is true.

**The Do/While Loop**
The do/while loop is a variant of the while loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.

**TYPE COERCION & WEAK TYPING**
JavaScript can convert data types behind the scenes to complete an operation.
 This is known as ***type coercion***.
**JavaScript** is said to use weak typing because the data type for a value can change. Some other languages require that you specify what data type each variable will be. They are said to use ***strong typing***.

**TRUTHY & FALSY VALUES**

*Falsy values* are treated as if they are false. The table to the left shows a high Score variable with a series of values, all of which are falsy.
*Truthy values* are treated as if they are true. Almost everything that is not in the falsy table can be treated as if it were true.

