# [freeCodeCamp](https://www.freecodecamp.org/learn)

## [Responsive Web Design](https://www.freecodecamp.org/learn/responsive-web-design/)  

### [Basic HTML and HTML5](https://www.freecodecamp.org/learn/responsive-web-design/#basic-html-and-html5)  

HTML5 introduces more descriptive HTML tags. These include main, header, footer, nav, video, article, section and others.  

hese tags give a descriptive structure to your HTML, make your HTML easier to read, and help with Search Engine Optimization (SEO) and accessibility.  

```<a>``` element = anchor element  

### [Basic CSS](https://www.freecodecamp.org/learn/responsive-web-design/#basic-css)  

CSS, or Cascading Style Sheets, tell the browser how to display the text and other content that you write in HTML. With CSS, you can control the color, font, size, spacing, and many other aspects of HTML elements.  

[Google Fonts](https://fonts.google.com/)  

### Vocabulary

Property = ``transform``  
Function = ``scale()``  

```
p {
  transform: scale(2);
}
```

Pseudo-classes = ``:hover``, etc...  

```
p:hover {
  transform: scale(2.1);
}
```

#### CSS Selectors

- id
- class
- [attr=value] (e.g. [type='radio'])

#### Absolute versus Relative Units

_Absolute_  
- in
- mm

_Relative_  
- em
- rem

#### Represent colors in CSS

[RGB color model](https://en.wikipedia.org/wiki/RGB_color_model)  

**Hed Code**  

In CSS, we can use 6 hexadecimal digits to represent colors, two each for the red (R), green (G), and blue (B) components  

_black:_  
```
color: #000000;
```

white:_  
```
color: #FFFFFF;
```

_red:_ 
```
color: #FF0000;
```

_green:_ 
```
color: #00FF00;
```

_blue:_ 
```
color: #0000FF;
```

**_Abbreviated Hex Code_**  

For example, red's hex code #FF0000 can be shortened to #F00. This shortened form gives one digit for red, one digit for green, and one digit for blue.  
This reduces the total number of possible colors to around 4,000. But browsers will interpret #FF0000 and #F00 as exactly the same color.  

Short Hex Code  

_red:_ 
```
color: #F00;
```

_green:_ 
```
color: #0F0;
```

_blue:_ 
```
color: #00F;
```

_cyan:_ 
```
color: #0FF;
```

**RGB values**  

_black:_  
```
color: rgb(0, 0, 0);
```

white:_  
```
color: rgb(255, 255, 255);
```

_red:_ 
```
color: rgb(255, 0, 0);
```

_green:_ 
```
color: rgb(0, 255, 0);
```

_blue:_ 
```
color: rgb(0, 0, 255);
```

#### CSS Variables

```
<style>
    :root {
        --p-color: purple;
    }
</style>
```

### Applied Visual Design

- Use the ```<u>``` Tag to Underline Text

- Use the ```<em>``` Tag to Italicize Text

- Use the ```<s>``` Tag to Strikethrough Text

- Use the ```<hr>``` Tag to Create a Horizontal Line

**rgba()**

The RGB values can range from 0 to 255. The alpha value can range from 1, which is fully opaque or a solid color, to 0, which is fully transparent or clear.  

**_rgba stands for:_**  
r = red  
g = green  
b = blue  
a = alpha/level of opacity  

_example:_  
```
background-color: rgba(45, 45, 45, 0.1)
```
**opacity:**  

A value of 1 is opaque, which isn't transparent at all.  
A value of 0.5 is half see-through.  
A value of 0 is completely transparent.  

**text-transform:**  
Value | Result
--- | ---
lowercase | "transform me"
uppercase | "TRANSFORM ME"
capitalize | "Transform Me"
initial | Use the default value
inherit | Use the text-transform value from the parent element
none | Default: Use the original text

**pseudo-class selector**  

:hover  

**CSS Box Model**  

**_Block-level_** items automatically start on a new line (think headings, paragraphs, and divs) while **_inline_** items sit within surrounding content (like images or spans).  

The default layout of elements in this way is called the **_normal flow_** of a document, but CSS offers the position property to override it.  

**relative**  
allows you to specify how CSS should move it relative to its current position in the normal flow of the page.  

**absolute**  
locks the element in place relative to its parent container. Unlike the relative position, this removes the element from the normal flow of the document, so surrounding items ignore it. 
One nuance with absolute positioning is that it will be locked relative to its closest positioned ancestor.  

**fixed**  
One key difference between the fixed and absolute positions is that an element with a fixed position won't move when the user scrolls.  

**float**  
Floating elements are removed from the normal flow of a document and pushed to either the left or right of their containing parent element.  

**z-index**  
When elements are positioned to overlap (i.e. using position: absolute | relative | fixed | sticky), the element coming later in the HTML markup will, by default, appear on the top of the other elements. However, the z-index property can specify the order of how elements are stacked on top of one another.  

**Center an Element Horizontally Using the margin Property**
Another positioning technique is to center a block element horizontally. One way to do this is to set its margin to a value of auto.  
This method works for images, too. Images are inline elements by default, but can be changed to block elements when you set the display property to block.  

[Color wheel](https://en.wikipedia.org/wiki/Color_wheel)  
A color wheel or color circle is an abstract illustrative organization of color hues around a circle, which shows the relationships between primary colors, secondary colors, tertiary colors etc.  

[Color model](https://en.wikipedia.org/wiki/Color_model)  
A color model is an abstract mathematical model describing the way colors can be represented as tuples of numbers, typically as three or four values or color components. When this model is associated with a precise description of how the components are to be interpreted (viewing conditions, etc.), the resulting set of colors is called "color space." This section describes ways in which human color vision can be modeled.  

**Adjust the Hue of a Color**  

```hsl()```  

_'h', 's', and 'l' of ```hsl()``` stand for hue, saturation, and lightness_  

Colors have several characteristics including hue, saturation, and lightness. CSS3 introduced the hsl() property as an alternative way to pick a color by directly stating these characteristics.  

**Hue** is what people generally think of as 'color'. If you picture a spectrum of colors starting with red on the left, moving through green in the middle, and blue on right, the hue is where a color fits along this line. In hsl(), hue uses a color wheel concept instead of the spectrum, where the angle of the color on the circle is given as a value between 0 and 360.  

**Saturation** is the amount of gray in a color. A fully saturated color has no gray in it, and a minimally saturated color is almost completely gray. This is given as a percentage with 100% being fully saturated.  

**Lightness** is the amount of white or black in a color. A percentage is given ranging from 0% (black) to 100% (white), where 50% is the normal color.  

Here are a few examples of using ```hsl()``` with fully-saturated, normal lightness colors:

Color | HSL
--- | ---
red | hsl(0, 100%, 50%)
yellow | hsl(60, 100%, 50%)
green | hsl(120, 100%, 50%)
cyan | hsl(180, 100%, 50%)
blue | hsl(240, 100%, 50%)
magenta | hsl(300, 100%, 50%)

**Adjust the Tone of a Color**  
The ```hsl()``` option in CSS also makes it easy to adjust the tone of a color. Mixing white with a pure hue creates a tint of that color, and adding black will make a shade. Alternatively, a tone is produced by adding gray or by both tinting and shading. Recall that the 's' and 'l' of hsl() stand for saturation and lightness, respectively. The saturation percent changes the amount of gray and the lightness percent determines how much white or black is in the color. This is useful when you have a base hue you like, but need different variations of it.  

**Gradual CSS Linear Gradient**  

```linear-gradient()```  

This is accessed through the background property's linear-gradient() function. Here is the general syntax:  

```
background: linear-gradient(gradient_direction, color 1, color 2, color 3, ...);
```

```repeating-linear-gradient()```  

The repeating-linear-gradient() function is very similar to linear-gradient() with the major difference that it repeats the specified gradient pattern.  

```
background: repeating-linear-gradient(
      90deg,
      yellow 0px,
      blue 40px,
      green 40px,
      red 80px
    );
```

```url()```  

```
background: url(https://cdn-media-1.freecodecamp.org/imgr/MJAkxbh.png);
```

**Transform property**  

To change the scale of an element, CSS has the transform property, along with its ```scale()``` function.  

```scale()```  

```
div {
    transform: scale(2);
}
```

```:hover```  

```
div:hover {
    transform: scale(2);
}
```

```skewX()```  

```
div {
    transform: skewX(-24deg)
}
```

```skewY()```  

```
div {
    transform: skewY(24deg)
}
```

**crescent moon shape**  

```
<style>
  .center {
    position: absolute;
    margin: auto;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    width: 100px;
    height: 100px;
    background-color: transparent;
    border-radius: 50%;
    box-shadow: 25px 10px 0 0 blue;
                offset-x offset-y,
  }

</style>
<div class="center"></div>
```