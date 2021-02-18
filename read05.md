# Choosing Images for Your Site

**Images should:**

1. Be relevant
2. Convey information
3. Convey the right mood
4. Be instantly recognisable
5. Fit the color palette

**Adding Images**
To add an image into the page you need to use an `<img>` element.
ex: `<img src="images/quokka.jpg">`

**Image attributes:**

- src
  This tells the browser where it can find the image file.
- alt
  This provides a text description of the image which describes the image if you cannot see it.
- title
  You can also use the title attribute with the <img> element to provide additional information about the image.
- height
  This specifies the height of the image in pixels.
- width
  This specifies the width of the image in pixels.

**Where to Place Images in Your Code**

1. before a paragraph
2. inside the start of a paragraph
3. in the middle of a paragraph

**Where you place the image in**
the code is important because browsers show HTML elements in one of two ways:

1. Block elements always appear on a new line.
2. Inline elements sit within a block level element and do not start on a new line.

#### Three Rules for Creating Images:

1. Save images in the right format : Websites mainly use images in **jpeg, gif, or png format**,

- Whenever you have many different colors in a picture you should use a **JPEG**.
- Use **GIF** or **PNG** format when saving images with few colors or large areas of the same color.

2. Save images at the right size.
3. Use the correct resolution.

#### Tools to Edit & Save Images

- Adobe Photoshop.
- Adobe Fireworks
- Pixelmator
- PaintShop Pro
- Paint.net

- **Image Dimensions**
  The images you use on your website should be saved at the same width and height that you want them to appear on the page.

- **Image Resolution**
  Images created for the web should be saved at a resolution of 72 ppi. The higher the resolution of the image, the larger the size of the file.

- **Vector images** differ from bitmap images and are resolution-independent. Vector images are commonly created in programs such as AdobeIllustrator.

- **Animated GIFs** show several frames of an image in sequence and therefore can be used to create simple animations.

**Transparency**
Creating an image that is partially transparent( or "see-through") for the web involves selecting one of two formats:

- Transparent GIF
- png

#### Examining Images on the Web

- This can be achieved by right-clicking on the image and making a selection from the pop-up menu that appears

### HTML 5: Figure and Figure Caption

- `<figure>`: Images often come with captions. HTML5 has introduced a new `<figure>` element to contain images and their caption so that the two are associated.

- `<figcaption>`
  The `<figcaption>` element has been added to HTML5 in order to allow web page authors to add a caption to an image.

**book summary**

- The `<img>` element is used to add images to a web page.
- You must always specify a src attribute to indicate the source of an image and an alt attribute to describe the content of an image.
- You should save images at the size you will be using them on the web page and in the appropriate format.
- Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.



# Colors in CSS:
There are several different ways to specify colors in CSS.

### Color Keywords
- RGB
- RGBA
- HSL
- HSLA
- Hexadecimal

### Color Keywords
The first and easiest way to specify a color is using one of the 140 predefined color keywords specified in CSS.

### RGB Color Values
* RGB colors have three values that represent: red, green, and blue
* Each value can be a number between 0 and 255 or a percentage from 0 to 100%
* A value of 0 means none of that color is being used
* A value of 255 or 100% means all of that color is being used
* A 0 for all three color values will be black
* A 255 or 100% for all three color values will be white.

**The CSS syntax for using RGB: color: rgb(0, 0, 0)**

## RGBA Color Values:
**RGBA is all the rage**
Seriously though, it's just like RGB, except with the addition of a fourth value: the alpha channel.
### rgba (250,250,250,a)
The alpha value represents the level of transparency that the rgb color should have. It can be a value from 0 to 1 or a percentage from 0 to 100%. Note that you must specify RGBA instead of RGB.

### HSL
The HSL color model is one of the least used, but gaining traction because can be more intuitive to use when working with shades and color adjustments.

**HSL stands** for: hue, saturation, and lightness.
EX: hsl(240, 100%, 90%)

**HSLA**
HSLA is simply the HSL color model with the addition of an alpha channel. This works exactly the same way as the alpha channel in RGBA.
EX:
h1 {
   background-color: hsla(240, 25%, 50%, .5);
}


## Hexadecimal Color Values:
Instead of using three numbers between 0 and 255, you use six hexadecimal numbers. Hex numbers can be 0-9 and A-F. Hex values are always prefixed with a # symbol

EXAMPLE:
p { color: #000000; }     /* black */
h1 { color: #ffffff; }    /* white */
h1 { color: #aaaaaa; }    /* medium gray */
ul { color: #8050c8; }    /* purple */

**Shorthand Notation for Hex Values:**
p { color: #000; }     /* black same as #000000 */
p { color: #fff; }    /* white same as #ffffff */
p { color: #f00; }     /* red: same as #ff0000 */
h1 { color: #0f0; }    /* lime: same as #00ff00 */
ul { color: #ff0; }    /* yellow: same as #ffff00 */

## CSS3: Opacity

*CSS3* introduces the opacity property which allows you to specify the opacity of an element and any of its child elements.The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).
EX:
p.one {
background-color: rgb(0,0,0);
opacity: 0.5;}
p.two {
background-color: rgb(0,0,0);
background-color: rgba(0,0,0,0.5);}

## COLOR SUMMARY:
* Color not only brings your s XX ite to life, but also helps convey the mood and evokes reactions.
* There are three ways to specify colors in CSS:RGB values, hex codes, and color names.
* Color pickers can help you find the color you want.
* It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).
* CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
* CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.


# HTML HTML 

**Text Formatting**

HTML provides us with the ability for formatting text just like we do it in MS Word or any text editing software. In this article, we would go through few such options.

Making text Bold or Strong: We can make the text bold using the < b> tag. The tag uses both opening and closing tag. The text that needs to be made bold must be within < b> and < /b> tag.

We can also use the `<strong>` tag to make the text strong, with added semantic importance. It also opens with `<strong>` and ends with `</strong>` tag.

**Example:**

< !DOCTYPE html> 
< html> 
< head> 
    < title> Bold </ title> 
< /head> 
< body> 

    <!--Normal text-->
    < p>Hello GeeksforGeeks< /p> 
    <!--Text in Bold-->
    < p>< b>Hello GeeksforGeeks</ b></ p> 
    <!--Text in Strong-->    
    < p>< strong>Hello GeeksforGeeks< /strong>< /p> 

< /body> 
< /html> 

- Making text Italic or emphasize: The **< i>** tag is used to italicise the text. It opens with **< i>** and ends with **< /i>** tag.
The **< em>** tag is used to emphasize the text, with added semantic importance. It opens with **< em>** and ends with **</ em>** tag.

- **Highlighting a text:** It is also possible to highlight a text in HTML using the < mark> tag. It has a opening tag < mark> and a closing tag < /mark>.

- **Making text smaller:** The < small> element is used to make the text smaller. The text that needs to be displayed smaller should be written inside < small> and < /small> tag.

- **Striking through the text:** The < del> element is used to strike through the text marking the part as deleted. It also has an opening and a closing tag.

- **Adding a text:** The < ins> element is used to underline a text marking the part as inserted or added. It also has an opening and a closing tag.

# JPEG vs PNG vs GIF — which image format to use and when?

***Compression***
Almost all forms of data that we see on the internet — text, image, video etc. — are compressed to reduce the size of data and ensure faster transmission. Choosing the correct format and compression is a major factor that determines image size.
Compression can be of two types — lossless and lossy. In lossless compression, it is possible to reconstruct the original image from the compressed image because there is no information loss during compression.

- **JPEG** is a lossy compression specification that takes advantage of human perception.

- **PNG**
 is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are introduced in the image.
 
 - **GIF**
  is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing.

  - **Transparency**
In a simple form, transparency indicates something that is completely invisible.

