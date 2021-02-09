
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