# [freeCodeCamp](https://www.freecodecamp.org/learn)

## [Responsive Web Design](https://www.freecodecamp.org/learn/responsive-web-design/)  

### Table of contents

[Basic HTML and HTML5](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#basic-html-and-html5)  
[Basic CSS](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#basic-css)  
[Applied Visual Design](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#applied-visual-design)  
[Applied Accessibility](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#applied-accessibility)  
[Responsive Web Design Principles](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#responsive-web-design-principles)  
[CSS Flexbox](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#css-flexbox)  
[CSS Grid](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#css-grid)  

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

**_code snippet:_**  
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

Elements = ``.heart``, ``#heart``, etc...  

```
.heart {
  background-color: blue;
}
```

Pseudo-elements = ``::before``, ``::after``, etc...  

```
.heart::before {
  content: "";
  background-color: yellow;
}
```

``.heart::before`` = selector  

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

### [Applied Visual Design](https://www.freecodecamp.org/learn/responsive-web-design#applied-visual-design)

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

````::before```` and ````::after````  

For the ``::before`` and ``::after`` pseudo-elements to function properly, they must have a defined ``content`` property. This property is usually used to add things like a photo or text to the selected element.  

When the ``::before`` and ``::after`` pseudo-elements are used to make shapes, the ``content`` property is still required, but it's set to an empty string.  

**heart shape**  

```
<style>
  .heart {
    position: absolute;
    margin: auto;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    background-color: pink;
    height: 50px;
    width: 50px;
    transform: rotate(-45deg);
  }
  .heart::after {
    background-color: pink;
    content: "";
    border-radius: 50%;
    position: absolute;
    width: 50px;
    height: 50px;
    top: 0px;
    left: 25px;
  }
  .heart::before {
    content: "";
    background-color: pink;
    border-radius: 50%;
    position: absolute;
    width: 50px;
    height: 50px;
    top: -25px;
    left: 0px;
  }
</style>
<div class="heart"></div>
```

``@keyframes`` and **animation** properties  

To animate an element, you need to know about the **animation** properties and the ``@keyframes`` rule.  

The **animation** properties control how the animation should behave and the ``@keyframes`` rule controls what happens during that animation.  

``animation-name``  

``animation-name`` sets the name of the animation, which is later used by @keyframes to tell CSS which rules go with which animations.  

``animation-duration``  

``animation-duration`` sets the length of time for the animation.  

```
<style>
  div {
    height: 40px;
    width: 70%;
    background: black;
    margin: 50px auto;
    border-radius: 5px;
  }

  #rect {
    animation-name: rainbow;
    animation-duration: 4s;
  }
  @keyframes rainbow {
    0% {
      background-color: blue;
    }
    50% {
      background-color: green;
    }
    100% {
      background-color: yellow;
    }
  }
</style>
<div id="rect"></div>
```

**CSS Animation to Change the Hover State**  

```
<style>
  button {
    border-radius: 5px;
    color: white;
    background-color: #0F5897;
    padding: 5px 10px 8px 10px;
  }

  button:hover {
    animation-name: background-color;
    animation-duration: 500ms;
  }
  @keyframes background-color {
    100% {
      background-color: #4791d0;
    }
  }
</style>
<button>Register</button>
```

``animation-fill-mode``  

```
<style>
  button {
    border-radius: 5px;
    color: white;
    background-color: #0F5897;
    padding: 5px 10px 8px 10px;
  }
  button:hover {
    animation-name: background-color;
    animation-duration: 500ms;
    animation-fill-mode: forwards;
  }
  @keyframes background-color {
    100% {
      background-color: #4791d0;
    }
  }
</style>
<button>Register</button>
```

**Movement Using CSS Animation**  

```
@keyframes rainbow {
  0% {
    background-color: blue;
    top: 0px;
  }
  50% {
    background-color: green;
    top: 50px;
  }
  100% {
    background-color: yellow;
    top: 0px;
  }
}
```

**Fading an Element from Left to Right**  

```
<style>
  #ball {
    width: 70px;
    height: 70px;
    margin: 50px auto;
    position: fixed;
    left: 20%;
    border-radius: 50%;
    background: linear-gradient(
      35deg,
      #ccffff,
      #ffcccc
    );
    animation-name: fade;
    animation-duration: 3s;
  }
  @keyframes fade {
    50% {
      left: 60%;
      opacity: 0.1;
    }
  }
</style>
<div id="ball"></div>
```

**Using an Infinite Animation Count**  

```
animation-iteration-count: 3;
```

```
animation-iteration-count: infinite;
```

```
<style>
  #ball {
    width: 100px;
    height: 100px;
    margin: 50px auto;
    position: relative;
    border-radius: 50%;
    background: linear-gradient(
      35deg,
      #ccffff,
      #ffcccc
    );
    animation-name: bounce;
    animation-duration: 1s;
    animation-iteration-count: infinite;
  }

  @keyframes bounce{
    0% {
      top: 0px;
    }
    50% {
      top: 249px;
      width: 130px;
      height: 70px;
    }
    100% {
      top: 0px;
    }
  }
</style>
<div id="ball"></div>
```

**Make a CSS Heartbeat using an Infinite Animation Count**  

```
<style>
  .back {
    position: fixed;
    padding: 0;
    margin: 0;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: white;
    animation-name: backdiv;
    animation-duration: 1s;
    animation-iteration-count: infinite;
  }

  .heart {
    position: absolute;
    margin: auto;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    background-color: pink;
    height: 50px;
    width: 50px;
    transform: rotate(-45deg);
    animation-name: beat;
    animation-duration: 1s;
    animation-iteration-count: infinite;
  }
  .heart:after {
    background-color: pink;
    content: "";
    border-radius: 50%;
    position: absolute;
    width: 50px;
    height: 50px;
    top: 0px;
    left: 25px;
  }
  .heart:before {
    background-color: pink;
    content: "";
    border-radius: 50%;
    position: absolute;
    width: 50px;
    height: 50px;
    top: -25px;
    left: 0px;
  }

  @keyframes backdiv {
    50% {
      background: #ffe6f2;
    }
  }

  @keyframes beat {
    0% {
      transform: scale(1) rotate(-45deg);
    }
    50% {
      transform: scale(0.6) rotate(-45deg);
    }
  }

</style>
<div class="back"></div>
<div class="heart"></div>
```

``animation-duration``  

```
<style>
  .stars {
    background-color: white;
    height: 30px;
    width: 30px;
    border-radius: 50%;
    animation-iteration-count: infinite;
  }

  .star-1 {
    margin-top: 15%;
    margin-left: 60%;
    animation-duration: 1s;
    animation-name: twinkle;
  }

  .star-2 {
    margin-top: 25%;
    margin-left: 25%;
    animation-duration: 0.9s;
    animation-name: twinkle;
  }

  .star-3 {
    margin-top: 10%;
    margin-left: 50%;
    animation-duration: 1.1s;
    animation-name: twinkle;
  }

  @keyframes twinkle {
    20% {
      transform: scale(0.5);
      opacity: 0.5;
    }
  }

  #back {
    position: fixed;
    padding: 0;
    margin: 0;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(black, #000099, #66c2ff, #ffcccc, #ffeee6);
  }
</style>

<div id="back"></div>
<div class="star-1 stars"></div>
<div class="star-2 stars"></div>
<div class="star-3 stars"></div>
```

``animation-timing-function``  

```
<style>

  .balls {
    border-radius: 50%;
    background: linear-gradient(
      35deg,
      #ccffff,
      #ffcccc
    );
    position: fixed;
    width: 50px;
    height: 50px;
    margin-top: 50px;
    animation-name: bounce;
    animation-duration: 2s;
    animation-iteration-count: infinite;
  }
  #ball1 {
    left:27%;
animation-timing-function: linear;
  }
  #ball2 {
    left:56%;
animation-timing-function: ease-out;
  }

  @keyframes bounce {
    0% {
      top: 0px;
    }
    100% {
      top: 249px;
    }
  }

</style>

<div class="balls" id="ball1"></div>
<div class="balls" id="ball2"></div>
```

**Bezier curves**  

``cubic-bezier``  

example 1:  

```
<style>
  .balls{
    border-radius: 50%;
    position: fixed;
    width: 50px;
    height: 50px;
    margin-top: 50px;
    animation-name: bounce;
    animation-duration: 2s;
    animation-iteration-count: infinite;
  }
  #red {
    background: red;
    left: 27%;
    animation-timing-function: cubic-bezier(0, 0, 0.58, 1);
  }
  #blue {
    background: blue;
    left: 56%;
    animation-timing-function: ease-out;
  }
  @keyframes bounce {
    0% {
      top: 0px;
    }
    100% {
      top: 249px;
    }
  }
</style>
<div class="balls" id= "red"></div>
<div class="balls" id= "blue"></div>
```

example 2:  

```
<style>
  .balls {
    border-radius: 50%;
    position: fixed;
    width: 50px;
    height: 50px;
    top: 60%;
    animation-name: jump;
    animation-duration: 2s;
    animation-iteration-count: infinite;
  }
  #red {
    background: red;
    left: 25%;
    animation-timing-function: linear;
  }
  #blue {
    background: blue;
    left: 50%;
    animation-timing-function: ease-out;
  }
  #green {
    background: green;
    left: 75%;
    animation-timing-function: cubic-bezier(0.311, 0.441, 0.444, 1.649);
  }

  @keyframes jump {
    50% {
      top: 10%;
    }
  }
</style>
<div class="balls" id="red"></div>
<div class="balls" id="blue"></div>
<div class="balls" id="green"></div>
```

### [Applied Accessibility](https://www.freecodecamp.org/learn/responsive-web-design#applied-accessibility)

**Text Alternative to Images for Visually Impaired Accessibility**  

```
<img src="importantLogo.jpeg" alt="Company logo">
```

**Know When Alt Text Should be Left Blank**  

Sometimes images are grouped with a caption already describing them, or are used for decoration only. In these cases, alt text may seem redundant or unnecessary.  

```
<img src="visualDecoration.jpeg" alt="">
```

**Background images** usually fall under the 'decorative' label as well.  
However, they are typically applied with CSS rules, and therefore not part of the markup screen readers process.  

**Use Headings to Show Hierarchical Relationships of Content**  

Headings (h1 through h6 elements) are workhorse tags that help provide structure and labeling to your content.  

**Jump Straight to the Content Using the main Element**  

HTML5 introduced several new elements that give developers more options while also incorporating accessibility features. These tags include ``main``, ``header``, ``footer``, ``nav``, ``article``, and ``section``, among others.  

``article`` is another one of the new HTML5 elements that add semantic meaning to your markup. article is a sectioning element and is used to wrap independent, self-contained content. The tag works well with blog entries, forum posts, or news articles.  

The ``section`` element is also new with HTML5, and has a slightly different semantic meaning than ``article``. An ``article`` is for standalone content, and a ``section`` is for grouping thematically related content. They can be used within each other, as needed. For example, if a book is the ``article``, then each chapter is a ``section``. When there's no relationship between groups of content, then use a ``div``.  

``<div>`` - groups content  
``<section>`` - groups related content  
``<article>`` - groups independent, self-contained content  

```
<h1>Deep Thoughts with Master Camper Cat</h1>
<main>
  <article>
    <h2>The Garfield Files: Lasagna as Training Fuel?</h2>
    <p>The internet is littered with varying opinions on nutritional paradigms, from catnip paleo to hairball cleanses. But let's turn our attention to an often overlooked fitness fuel, and examine the protein-carb-NOM trifecta that is lasagna...</p>
  </article>

  <img src="samuraiSwords.jpeg" alt="">

  <article>
    <h2>Defeating your Foe: the Red Dot is Ours!</h2>
    <p>Felines the world over have been waging war on the most persistent of foes. This red nemesis combines both cunning stealth and lightning speed. But chin up, fellow fighters, our time for victory may soon be near...</p>
  </article>

  <img src="samuraiSwords.jpeg" alt="">

  <article>
    <h2>Is Chuck Norris a Cat Person?</h2>
    <p>Chuck Norris is widely regarded as the premier martial artist on the planet, and it's a complete coincidence anyone who disagrees with this fact mysteriously disappears soon after. But the real question is, is he a cat person?...</p>
  </article>
</main>
```

**Make Screen Reader Navigation Easier with the header Landmark**  

``header`` shares the embedded landmark feature you saw with ``main``, allowing assistive technologies to quickly navigate to that content.  

The ``header`` is meant for use in the ``body`` tag of your HTML document. It is different than the ``head`` element, which contains the page's title, meta information, etc.  

**Make Screen Reader Navigation Easier with the nav Landmark**  

The ``nav`` element is another HTML5 item with the embedded landmark feature for easy screen reader navigation.  

**Make Screen Reader Navigation Easier with the footer Landmark**

Similar to header and nav, the footer element has a built-in landmark feature that allows assistive devices to quickly navigate to it.  

```
<body>
  <header>
    <h1>Training</h1>
    <nav>
      <ul>
        <li><a href="#stealth">Stealth &amp; Agility</a></li>
        <li><a href="#combat">Combat</a></li>
        <li><a href="#weapons">Weapons</a></li>
      </ul>
    </nav>
  </header>
  <main>
    <section id="stealth">
      <h2>Stealth &amp; Agility Training</h2>
      <article><h3>Climb foliage quickly using a minimum spanning tree approach</h3></article>
      <article><h3>No training is NP-complete without parkour</h3></article>
    </section>
    <section id="combat">
      <h2>Combat Training</h2>
      <article><h3>Dispatch multiple enemies with multithreaded tactics</h3></article>
      <article><h3>Goodbye world: 5 proven ways to knock out an opponent</h3></article>
    </section>
    <section id="weapons">
      <h2>Weapons Training</h2>
      <article><h3>Swords: the best tool to literally divide and conquer</h3></article>
      <article><h3>Breadth-first or depth-first in multi-weapon training?</h3></article>
    </section>
  </main>

  <footer>&copy; 2018 Camper Cat</footer>
</body>
```

**Improve Accessibility of Audio Content with the audio Element**  

HTML5's ``audio`` element gives semantic meaning when it wraps sound or audio stream content in your markup.  
The ``audio`` tag supports the ``controls`` attribute. This shows the browser default play, pause, and other controls, and supports keyboard functionality. This is a boolean attribute, meaning it doesn't need a value, its presence on the tag turns the setting on.  

**Improve Chart Accessibility with the figure Element**  

HTML5 introduced the ``figure`` element and the related ``figcaption``. Used together, these items wrap a visual representation (like an image, diagram, or chart) along with its caption.  

**Improve Form Field Accessibility with the label Element**  

The ``label`` tag wraps the text for a specific form control item, usually the name or label for a choice.  

The value of the for attribute must be the same as the value of the id attribute of the form control. Here's an example:  

```
<form>
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
</form>
```

**Wrap Radio Buttons in a fieldset Element for Better Accessibility**  

```
<form>
  <fieldset>
    <legend>Choose one of these three items:</legend>
    <input id="one" type="radio" name="items" value="one">
    <label for="one">Choice One</label><br>
    <input id="two" type="radio" name="items" value="two">
    <label for="two">Choice Two</label><br>
    <input id="three" type="radio" name="items" value="three">
    <label for="three">Choice Three</label>
  </fieldset>
</form>
```

**Add an Accessible Date Picker**  

```
<label for="input1">Enter a date:</label>
<input type="date" id="input1" name="input1">
```

**Standardize Times with the HTML5 datetime Attribute**  

```
<p>Thank you to everyone for responding to Master Camper Cat's survey. The best day to host the vaunted Mortal Kombat tournament is <time datetime="2016-09-15">Thursday, September 15<sup>th</sup></time>. May the best ninja win!</p>
```

**Make Elements Only Visible to a Screen Reader by Using Custom CSS**  

CSS's magic can also improve accessibility on your page when you want to visually hide content meant only for screen readers. This happens when information is in a visual format (like a chart), but screen reader users need an alternative presentation (like a table) to access the data. CSS is used to position the screen reader-only elements off the visual area of the browser window.  

Here's an example of the CSS rules that accomplish this:  

```
.sr-only {
  position: absolute;
  left: -10000px;
  width: 1px;
  height: 1px;
  top: auto;
  overflow: hidden;
}
```

display: none; or visibility: hidden; hides content for everyone, including screen reader users  

Zero values for pixel sizes, such as width: 0px; height: 0px; removes that element from the flow of your document, meaning screen readers will ignore it  

**Improve Readability with High Contrast Text**  

Low contrast between the foreground and background colors can make text difficult to read. Sufficient contrast improves your content's readability, but what exactly does "sufficient" mean?  

The Web Content Accessibility Guidelines (WCAG) recommend at least a 4.5 to 1 contrast ratio for normal text. The ratio is calculated by comparing the relative luminance values of two colors. This ranges from 1:1 for the same color, or no contrast, to 21:1 for white against black, the most substantial contrast. There are many contrast checking tools available online that calculate this ratio for you.  

:link: [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)  

**Avoid Colorblindness Issues by Using Sufficient Contrast**  

Color is a large part of visual design, but its use introduces two accessibility issues. First, color alone should not be used as the only way to convey important information because screen reader users won't see it. Second, foreground and background colors need sufficient contrast so colorblind users can distinguish them.  

**Avoid Colorblindness Issues by Carefully Choosing Colors that Convey Information**  

There are various forms of colorblindness. These can range from a reduced sensitivity to a certain wavelength of light to the inability to see color at all. The most common form is a reduced sensitivity to detect greens.  

[Color Blindness Simulator](https://www.color-blindness.com/coblis-color-blindness-simulator/)  

**Give Links Meaning by Using Descriptive Link Text**  

Screen reader users have various options for what type of content their device reads. These options include skipping to (or over) landmark elements, jumping to the main content, or getting a page summary from the headings. Another option is to only hear the links available on a page.  

**Make Links Navigable with HTML Access Keys**  

HTML offers the ``accesskey`` attribute to specify a shortcut key to activate or bring focus to an element. Adding an ``accesskey`` attribute can make navigation more efficient for keyboard-only users.  

HTML5 allows this attribute to be used on any element, but it's particularly useful when it's used with interactive ones. This includes links, buttons, and form controls.  

Here's an example:  

```
<button accesskey="b">Important Button</button>
```

**Use tabindex to Add Keyboard Focus to an Element**  

The HTML ``tabindex`` attribute has three distinct functions relating to an element's keyboard focus. When it's on a tag, it indicates that the element can be focused on. The value (an integer that's positive, negative, or zero) determines the behavior.  `

Certain elements, such as links and form controls, automatically receive keyboard focus when a user tabs through a page. It's in the same order as the elements come in the HTML source markup. This same functionality can be given to other elements, such as ``div``, ``span``, and ``p``, by placing a ``tabindex="0"`` attribute on them. Here's an example:  

```
<div tabindex="0">I need keyboard focus!</div>
```

Note: A negative ``tabindex`` value (typically -1) indicates that an element is focusable, but is not reachable by the keyboard. This method is generally used to bring focus to content programmatically (like when a ``div`` used for a pop-up window is activated), and is beyond the scope of these challenges.  

Using ``tabindex`` also enables the CSS pseudo-class :focus to work on the tag.  

**Use tabindex to Specify the Order of Keyboard Focus for Several Elements**  

The tabindex attribute also specifies the exact tab order of elements. This is achieved when the attribute's value is set to a positive number of 1 or higher.  

Setting a tabindex="1" will bring keyboard focus to that element first. Then it cycles through the sequence of specified tabindex values (2, 3, etc.), before moving to default and tabindex="0" items.  

It's important to note that when the tab order is set this way, it overrides the default order (which uses the HTML source). This may confuse users who are expecting to start navigation from the top of the page. This technique may be necessary in some circumstances, but in terms of accessibility, take care before applying it.  

Here's an example:  

```
<div tabindex="1">I get keyboard focus, and I get it first!</div>
```

```
<div tabindex="2">I get keyboard focus, and I get it second!</div>
```

Another thing to note is that some browsers may place you in the middle of your tab order when an element is clicked. An element has been added to the page that ensures you will always start at the beginning of your tab order.  

### [Responsive Web Design Principles](https://www.freecodecamp.org/learn/responsive-web-design/#responsive-web-design-principles)

There are many devices that can access the web, and they come in all shapes and sizes. Responsive web design is the practice of designing flexible websites that can respond to different screen sizes, orientations, and resolutions.  

In this course, you'll learn how to use CSS to make your webpages look good, no matter what device they're viewed on.  

**Create a Media Query**  

Media Queries are a new technique introduced in CSS3 that change the presentation of content based on different viewport sizes. The viewport is a user's visible area of a web page, and is different depending on the device used to access the site.  

Media Queries consist of a media type, and if that media type matches the type of device the document is displayed on, the styles are applied. You can have as many selectors and styles inside your media query as you want.  

Here's an example of a media query that returns the content when the device's width is less than or equal to 100px:  

```
@media (max-width: 100px) { /* CSS Rules */ }
```

and the following media query returns the content when the device's height is more than or equal to 350px:  

```
@media (min-height: 350px) { /* CSS Rules */ }
```

Remember, the CSS inside the media query is applied only if the media type matches that of the device being used.  

**Make an Image Responsive**  

Making images responsive with CSS is actually very simple. You just need to add these properties to an image:  

```
img {
  max-width: 100%;
  height: auto;
}
```

The max-width of 100% will make sure the image is never wider than the container it is in, and the height of auto will make the image keep its original aspect ratio.  

**Use a Retina Image for Higher Resolution Displays**  

With the increase of internet connected devices, their sizes and specifications vary, and the displays they use could be different externally and internally. Pixel density is an aspect that could be different on one device from others and this density is known as **Pixel Per Inch(PPI)** or **Dots Per Inch(DPI)**. The most famous such display is the one known as a "Retina Display" on the latest Apple MacBook Pro notebooks, and recently iMac computers. Due to the difference in pixel density between a "Retina" and "Non-Retina" displays, some images that have not been made with a High-Resolution Display in mind could look "pixelated" when rendered on a High-Resolution display.  

The simplest way to make your images properly appear on High-Resolution Displays, such as the MacBook Pros "retina display" is to define their width and height values as only half of what the original file is. Here is an example of an image that is only using half of the original height and width:  

```
<style>
  img { height: 250px; width: 250px; }
</style>
<img src="coolPic500x500" alt="A most excellent picture">
```

**Make Typography Responsive**  

Instead of using em or px to size text, you can use viewport units for responsive typography. Viewport units, like percentages, are relative units, but they are based off different items. Viewport units are relative to the viewport dimensions (width or height) of a device, and percentages are relative to the size of the parent container element.  

The four different viewport units are:  

- vw (viewport width): 10vw would be 10% of the viewport's width.
- vh (viewport height): 3vh would be 3% of the viewport's height.
- vmin (viewport minimum): 70vmin would be 70% of the viewport's smaller dimension (height or width).
- vmax (viewport maximum): 100vmax would be 100% of the viewport's bigger dimension (height or width).

Here is an example that sets a body tag to 30% of the viewport's width.  

```
body { width: 30vw; }
```

### [CSS Flexbox](https://www.freecodecamp.org/learn/responsive-web-design/#css-flexbox)  

Flexbox is a powerful, well-supported layout method that was introduced with the latest version of CSS, CSS3. With flexbox, it's easy to center elements on the page and create dynamic user interfaces that shrink and expand automatically.  

In this course, you'll learn the fundamentals of flexbox and dynamic layouts by building a Twitter card.  

**Use display: flex to Position Two Boxes**  

Placing the CSS property display: flex; on an element allows you to use other flex properties to build a responsive page.  

**Add Flex Superpowers to the Tweet Embed**  

**Use the flex-direction Property to Make a Row**  

Adding ``display: flex`` to an element turns it into a flex container. This makes it possible to align any children of that element into rows or columns. You do this by adding the ``flex-direction`` property to the parent item and setting it to row or column. Creating a row will align the children horizontally, and creating a column will align the children vertically.  

Other options for ``flex-direction`` are row-reverse and column-reverse.  

Note: The default value for the ``flex-direction`` property is row.  

**Apply the flex-direction Property to Create Rows in the Tweet Embed**  

**Use the flex-direction Property to Make a Column**  

**Apply the flex-direction Property to Create a Column in the Tweet Embed**  

**Align Elements Using the justify-content Property**  

Sometimes the flex items within a flex container do not fill all the space in the container. It is common to want to tell CSS how to align and space out the flex items a certain way. Fortunately, the ``justify-content`` property has several options to do this. But first, there is some important terminology to understand before reviewing those options.  

[Here is a useful image showing a row to illustrate the concepts below.](https://www.w3.org/TR/css-flexbox-1/images/flex-direction-terms.svg)  

Recall that setting a flex container as a row places the flex items side-by-side from left-to-right. A flex container set as a column places the flex items in a vertical stack from top-to-bottom. For each, the direction the flex items are arranged is called the main axis. For a row, this is a horizontal line that cuts through each item. And for a column, the main axis is a vertical line through the items.  

There are several options for how to space the flex items along the line that is the main axis. One of the most commonly used is ``justify-content: center``;, which aligns all the flex items to the center inside the flex container. Other options include:  

- ``flex-start``: aligns items to the start of the flex container. For a row, this pushes the items to the left of the container. For a column, this pushes the items to the top of the container. This is the default alignment if no ``justify-content`` is specified.

- ``flex-end``: aligns items to the end of the flex container. For a row, this pushes the items to the right of the container. For a column, this pushes the items to the bottom of the container.

- ``space-between``: aligns items to the center of the main axis, with extra space placed between the items. The first and last items are pushed to the very edge of the flex container. For example, in a row the first item is against the left side of the container, the last item is against the right side of the container, then the remaining space is distributed evenly among the other items.

- ``space-around``: similar to space-between but the first and last items are not locked to the edges of the container, the space is distributed around all the items with a half space on either end of the flex container.

- ``space-evenly``: Distributes space evenly between the flex items with a full space at either end of the flex container

**Use the justify-content Property in the Tweet Embed**  

**Align Elements Using the align-items Property**  

The align-items property is similar to justify-content. Recall that the justify-content property aligned flex items along the main axis. For rows, the main axis is a horizontal line and for columns it is a vertical line.  

Flex containers also have a cross axis which is the opposite of the main axis. For rows, the cross axis is vertical and for columns, the cross axis is horizontal.  

CSS offers the align-items property to align flex items along the cross axis. For a row, it tells CSS how to push the items in the entire row up or down within the container. And for a column, how to push all the items left or right within the container.  

The different values available for align-items include:  

- ``flex-start``: aligns items to the start of the flex container. For rows, this aligns items to the top of the container. For columns, this aligns items to the left of the container.

- ``flex-end``: aligns items to the end of the flex container. For rows, this aligns items to the bottom of the container. For columns, this aligns items to the right of the container.

- ``center``: align items to the center. For rows, this vertically aligns items (equal space above and below the items). For columns, this horizontally aligns them (equal space to the left and right of the items).

- ``stretch``: stretch the items to fill the flex container. For example, rows items are stretched to fill the flex container top-to-bottom. This is the default value if no align-items value is specified.

- ``baseline``: align items to their baselines. Baseline is a text concept, think of it as the line that the letters sit on.

**Use the align-items Property in the Tweet Embed**  

**Use the flex-wrap Property to Wrap a Row or Column**  

CSS flexbox has a feature to split a flex item into multiple rows (or columns). By default, a flex container will fit all flex items together. For example, a row will all be on one line.  

However, using the flex-wrap property tells CSS to wrap items. This means extra items move into a new row or column. The break point of where the wrapping happens depends on the size of the items and the size of the container.  

CSS also has options for the direction of the wrap:  

- ``nowrap``: this is the default setting, and does not wrap items.

- ``wrap``: wraps items onto multiple lines from top-to-bottom if they are in rows and left-to-right if they are in columns.

- ``wrap-reverse``: wraps items onto multiple lines from bottom-to-top if they are in rows and right-to-left if they are in columns.

**Use the flex-shrink Property to Shrink Items**  

There are several useful properties for the flex items.  

When ``flex-shrink`` property is used, it allows an item to shrink if the flex container is too small. Items shrink when the width of the parent container is smaller than the combined widths of all the flex items within it.  

The ``flex-shrink`` property takes numbers as values. The higher the number, the more it will shrink compared to the other items in the container. For example, if one item has a ``flex-shrink`` value of 1 and the other has a ``flex-shrink`` value of 3, the one with the value of 3 will shrink three times as much as the other.  

**Use the flex-grow Property to Expand Items**  

The opposite of ``flex-shrink`` is the ``flex-grow`` property. Recall that ``flex-shrink`` controls the size of the items when the container shrinks. The ``flex-grow`` property controls the size of items when the parent container expands.  

Using a similar example from the last challenge, if one item has a ``flex-grow`` value of 1 and the other has a ``flex-grow`` value of 3, the one with the value of 3 will grow three times as much as the other.  

**Use the flex-basis Property to Set the Initial Size of an Item**  

The flex-basis property specifies the initial size of the item before CSS makes adjustments with ``flex-shrink`` or ``flex-grow``.  

The units used by the flex-basis property are the same as other size properties (px, em, %, etc.). The value auto sizes items based on the content.  

**Use the flex Shorthand Property**  

There is a shortcut available to set several flex properties at once. The ``flex-grow``, ``flex-shrink``, and ``flex-basis`` properties can all be set together by using the flex property.  

For example, ``flex: 1 0 10px``; will set the item to ``flex-grow: 1;``, ``flex-shrink: 0;``, and ``flex-basis: 10px;``.  

The default property settings are ``flex: 0 1 auto``;.  

**Use the order Property to Rearrange Items**  

The ``order`` property is used to tell CSS the order of how flex items appear in the flex container. By default, items will appear in the same order they come in the source HTML. The property takes numbers as values, and negative numbers can be used.  

**Use the align-self Property**  

The final property for flex items is ``align-self``. This property allows you to adjust each item's alignment individually, instead of setting them all at once. This is useful since other common adjustment techniques using the CSS properties float, clear, and vertical-align do not work on flex items.  

``align-self`` accepts the same values as align-items and will override any value set by the align-items property.  

### [CSS Grid](https://www.freecodecamp.org/learn/responsive-web-design/#css-grid)  

The CSS grid is a newer standard that makes it easy to build complex responsive layouts. It works by turning an HTML element into a grid, and lets you place child elements anywhere within.  

In this course, you'll learn the fundamentals of CSS grid by building different complex layouts, including a blog.  

**Create Your First CSS Grid**  

Turn any HTML element into a grid container by setting its display property to grid. This gives you the ability to use all the other properties associated with CSS Grid.  

Note: In CSS Grid, the parent element is referred to as the container and its children are called items.  

**Add Columns with grid-template-columns**  

Simply creating a grid element doesn't get you very far. You need to define the structure of the grid as well. To add some columns to the grid, use the grid-template-columns property on a grid container as demonstrated below:  

```
.container {
  display: grid;
  grid-template-columns: 50px 50px;
}
```

This will give your grid two columns that are each 50px wide. The number of parameters given to the ``grid-template-columns`` property indicates the number of columns in the grid, and the value of each parameter indicates the width of each column.  

**Add Rows with grid-template-rows**  

To adjust the rows manually, use the ``grid-template-rows`` property in the same way you used ``grid-template-columns`` in the previous challenge.  

**Use CSS Grid units to Change the Size of Columns and Rows**  

You can use absolute and relative units like px and em in CSS Grid to define the size of rows and columns. You can use these as well:  

``fr``: sets the column or row to a fraction of the available space,  

``auto``: sets the column or row to the width or height of its content automatically,  

``%``: adjusts the column or row to the percent width of its container.  

Here's the code that generates the output in the preview:  

```
grid-template-columns: auto 50px 10% 2fr 1fr;
```

This snippet creates five columns. The first column is as wide as its content, the second column is 50px, the third column is 10% of its container, and for the last two columns; the remaining space is divided into three sections, two are allocated for the fourth column, and one for the fifth.  

**Create a Column Gap Using grid-column-gap**  

So far in the grids you have created, the columns have all been tight up against each other. Sometimes you want a gap in between the columns. To add a gap between the columns, use the ``grid-column-gap`` property like this:  

```
grid-column-gap: 10px;
```

This creates 10px of empty space between all of our columns.  

**Create a Row Gap using grid-row-gap**  

You can add a gap in between the rows of a grid using ``grid-row-gap`` in the same way that you added a gap in between columns in the previous challenge.  

**Add Gaps Faster with grid-gap**  

``grid-gap`` is a shorthand property for ``grid-row-gap`` and ``grid-column-gap`` from the previous two challenges that's more convenient to use. If ``grid-gap`` has one value, it will create a gap between all rows and columns. However, if there are two values, it will use the first one to set the gap between the rows and the second value for the columns.  

**Use grid-column to Control Spacing**  

The ``grid-column`` property is ofr use on the grid items themselves.  

The hypothetical horizontal and vertical lines that create the grid are referred to as lines. These lines are numbered starting with 1 at the top left corner of the grid and move right for columns and down for rows, counting upward.  

To control the number of columns an item will consume, you can use the ``grid-column`` property in conjunction with the line numbers you want the item to start and stop at.  

Here's an example:  

```
grid-column: 1 / 3;
```

This will make the item start at the first vertical line of the grid on the left and span to the 3rd line of the grid, consuming two columns.  

**Use grid-row to Control Spacing**  

Of course, you can make items consume multiple rows just like you can with columns. You define the horizontal lines you want an item to start and stop at using the ``grid-row`` property on a grid item.  

**Align an Item Horizontally using justify-self**  

In CSS Grid, the content of each item is located in a box which is referred to as a **cell**. You can align the content's position within its cell horizontally using the ``justify-self`` property on a grid item. By default, this property has a value of ``stretch``, which will make the content fill the whole width of the cell. This CSS Grid property accepts other values as well:  

``start``: aligns the content at the left of the cell, 

``center``: aligns the content in the center of the cell, 

``end``: aligns the content at the right of the cell. 

**Align an Item Vertically using align-self**  

Just as you can align an item horizontally, there's a way to align an item vertically as well. To do this, you use the ``align-self`` property on an item. This property accepts all of the same values as ``justify-self`` from the last challenge.  

**Align All Items Horizontally using justify-items**  

Sometimes you want all the items in your CSS Grid to share the same alignment. You can use the previously learned properties and align them individually, or you can align them all at once horizontally by using **justify-items** on your grid container. This property can accept all the same values you learned about in the previous two challenges, the difference being that it will move all the items in our grid to the desired alignment.  

**Align All Items Vertically using align-items**  

Using the ``align-items`` property on a grid container will set the vertical alignment for all the items in our grid.  

**Divide the Grid Into an Area Template**  

You can group cells of your grid together into an area and give the area a custom name. Do this by using ``grid-template-areas`` on the container like this:  

```
grid-template-areas:
  "header header header"
  "advert content content"
  "advert footer footer";
```

The code above groups the cells of the grid into four areas; ``header``, ``advert``, ``content``, and ``footer``. Every word represents a cell and every pair of quotation marks represent a row.  

**Place Items in Grid Areas Using the grid-area Property**  

After creating an area template for your grid container, as shown in the previous challenge, you can place an item in your custom area by referencing the name you gave it. To do this, you use the ``grid-area`` property on an item like this:  

```
.item1 {
  grid-area: header;
}
```

This lets the grid know that you want the item1 class to go in the area named ``header``. In this case, the item will use the entire top row because that whole row is named as the header area.  

**Use grid-area Without Creating an Areas Template**  

The ``grid-area`` property you learned in the last challenge can be used in another way. If your grid doesn't have an areas template to reference, you can create an area on the fly for an item to be placed like this:  

```
item1 { grid-area: 1/1/2/4; }
```

This is using the line numbers you learned about earlier to define where the area for this item will be. The numbers in the example above represent these values:  

```
grid-area: horizontal line to start at / vertical line to start at / horizontal line to end at / vertical line to end at;
```

So the item in the example will consume the rows between lines 1 and 2, and the columns between lines 1 and 4.  

**Reduce Repetition Using the repeat Function**  

When you used ``grid-template-columns`` and ``grid-template-rows`` to define the structure of a grid, you entered a value for each row or column you created.  

Let's say you want a grid with 100 rows of the same height. It isn't very practical to insert 100 values individually. Fortunately, there's a better way - by using the ``repeat`` function to specify the number of times you want your column or row to be repeated, followed by a comma and the value you want to repeat.  

Here's an example that would create the 100 row grid, each row at 50px tall.  

```
grid-template-rows: repeat(100, 50px);
```

You can also repeat multiple values with the repeat function and insert the function amongst other values when defining a grid structure. Here's what that looks like:  

```
grid-template-columns: repeat(2, 1fr 50px) 20px;  
```

This translates to:

```
grid-template-columns: 1fr 50px 1fr 50px 20px;
```

Note: The 1fr 50px is repeated twice followed by 20px.  

**Limit Item Size Using the minmax Function**  

There's another built-in function to use with ``grid-template-columns`` and ``grid-template-rows`` called ``minmax``. It's used to limit the size of items when the grid container changes size. To do this you need to specify the acceptable size range for your item. Here is an example:  

```
grid-template-columns: 100px minmax(50px, 200px);
```

In the code above, ``grid-template-columns`` is set to create two columns; the first is 100px wide, and the second has the minimum width of 50px and the maximum width of 200px.  

**Create Flexible Layouts Using auto-fill**  

The repeat function comes with an option called auto-fill. This allows you to automatically insert as many rows or columns of your desired size as possible depending on the size of the container. You can create flexible layouts when combining ``auto-fill`` with ``minmax``, like this:  

```
repeat(auto-fill, minmax(60px, 1fr));
```

When the container changes size, this setup keeps inserting 60px columns and stretching them until it can insert another one. Note: If your container can't fit all your items on one row, it will move them down to a new one.  

**Create Flexible Layouts Using auto-fit**  

``auto-fit`` works almost identically to ``auto-fill``. The only difference is that when the container's size exceeds the size of all the items combined, ``auto-fill`` keeps inserting empty rows or columns and pushes your items to the side, while ``auto-fit`` collapses those empty rows or columns and stretches your items to fit the size of the container.  

Note: If your container can't fit all your items on one row, it will move them down to a new one.  

**Use Media Queries to Create Responsive Layouts**  

CSS Grid can be an easy way to make your site more responsive by using media queries to rearrange grid areas, change dimensions of a grid, and rearrange the placement of items.  

In the preview, when the viewport width is 300px or more, the number of columns changes from 1 to 2. The advertisement area then occupies the left column completely.  

**Create Grids within Grids**  

Turning an element into a grid only affects the behavior of its direct descendants. So by turning a direct descendant into a grid, you have a grid within a grid.  

# Build a Tribute Page

Objective: Build a CodePen.io app that is functionally similar to this: https://codepen.io/freeCodeCamp/full/zNqgVx.  

Fulfill the below [user stories](https://en.wikipedia.org/wiki/User_story) and get all of the tests to pass. Give it your own personal style.  

You can use HTML, JavaScript, and CSS to complete this project. Plain CSS is recommended because that is what the lessons have covered so far and you should get some practice with plain CSS. You can use Bootstrap or SASS if you choose. Additional technologies (just for example jQuery, React, Angular, or Vue) are not recommended for this project, and using them is at your own risk. Other projects will give you a chance to work with different technology stacks like React. We will accept and try to fix all issue reports that use the suggested technology stack for this project. Happy coding!  

User Story #1: My tribute page should have an element with a corresponding ``id="main"``, which contains all other elements.  

User Story #2: I should see an element with a corresponding ``id="title"``, which contains a string (i.e. text) that describes the subject of the tribute page (e.g. "Dr. Norman Borlaug").  

User Story #3: I should see a ``div`` element with a corresponding ``id="img-div"``.  

User Story #4: Within the ``img-div`` element, I should see an ``img`` element with a corresponding ``id="image"``.  

User Story #5: Within the ``img-div`` element, I should see an element with a corresponding ``id="img-caption"`` that contains textual content describing the image shown in ``img-div``.  

User Story #6: I should see an element with a corresponding ``id="tribute-info"``, which contains textual content describing the subject of the tribute page.  

User Story #7: I should see an ``a`` element with a corresponding ``id="tribute-link"``, which links to an outside site that contains additional information about the subject of the tribute page. HINT: You must give your element an attribute of ``target`` and set it to ``_blank`` in order for your link to open in a new tab (i.e. ``target="_blank"``).  

User Story #8: The ``img`` element should responsively resize, relative to the width of its parent element, without exceeding its original size.  

User Story #9: The ``img`` element should be centered within its parent element.  

You can build your project by using this [CodePen template](https://codepen.io/pen?template=MJjpwO) and clicking ``Save`` to create your own pen. Or you can use this CDN link to run the tests in any environment you like: https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js.  

Once you're done, submit the URL to your working project with all its tests passing.  

# Build a Survey Form

Objective: Build a CodePen.io app that is functionally similar to this: https://codepen.io/freeCodeCamp/full/VPaoNP.  

Fulfill the below user stories and get all of the tests to pass. Give it your own personal style.  

You can use HTML, JavaScript, and CSS to complete this project. Plain CSS is recommended because that is what the lessons have covered so far and you should get some practice with plain CSS. You can use Bootstrap or SASS if you choose. Additional technologies (just for example jQuery, React, Angular, or Vue) are not recommended for this project, and using them is at your own risk. Other projects will give you a chance to work with different technology stacks like React. We will accept and try to fix all issue reports that use the suggested technology stack for this project. Happy coding!  

User Story #1: I can see a title with id="title" in H1 sized text.  

User Story #2: I can see a short explanation with id="description" in P sized text.  

User Story #3: I can see a form with id="survey-form".  

User Story #4: Inside the form element, I am required to enter my name in a field with id="name".  

User Story #5: Inside the form element, I am required to enter an email in a field with id="email".  

User Story #6: If I enter an email that is not formatted correctly, I will see an HTML5 validation error.  

User Story #7: Inside the form, I can enter a number in a field with id="number".  

User Story #8: If I enter non-numbers in the number input, I will see an HTML5 validation error.  

User Story #9: If I enter numbers outside the range of the number input, which are defined by the min and max attributes, I will see an HTML5 validation error.  

User Story #10: For the name, email, and number input fields inside the form I can see corresponding labels that describe the purpose of each field with the following ids: id="name-label", id="email-label", and id="number-label".  

User Story #11: For the name, email, and number input fields, I can see placeholder text that gives me a description or instructions for each field.  

User Story #12: Inside the form element, I can select an option from a dropdown that has a corresponding id="dropdown".  

User Story #13: Inside the form element, I can select a field from one or more groups of radio buttons. Each group should be grouped using the name attribute.  

User Story #14: Inside the form element, I can select several fields from a series of checkboxes, each of which must have a value attribute.  

User Story #15: Inside the form element, I am presented with a textarea at the end for additional comments.  

User Story #16: Inside the form element, I am presented with a button with id="submit" to submit all my inputs.  

You can build your project by using this CodePen template and clicking Save to create your own pen. Or you can use this CDN link to run the tests in any environment you like: https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js  

Once you're done, submit the URL to your working project with all its tests passing.  

# Build a Product Landing Page

Objective: Build a CodePen.io app that is functionally similar to this: https://codepen.io/freeCodeCamp/full/RKRbwL.  

Fulfill the below user stories and get all of the tests to pass. Give it your own personal style.  

You can use HTML, JavaScript, and CSS to complete this project. Plain CSS is recommended because that is what the lessons have covered so far and you should get some practice with plain CSS. You can use Bootstrap or SASS if you choose. Additional technologies (just for example jQuery, React, Angular, or Vue) are not recommended for this project, and using them is at your own risk. Other projects will give you a chance to work with different technology stacks like React. We will accept and try to fix all issue reports that use the suggested technology stack for this project. Happy coding!  

User Story #1: My product landing page should have a header element with a corresponding id="header".  

User Story #2: I can see an image within the header element with a corresponding id="header-img". A company logo would make a good image here.  

User Story #3: Within the #header element I can see a nav element with a corresponding id="nav-bar".  

User Story #4: I can see at least three clickable elements inside the nav element, each with the class nav-link.  

User Story #5: When I click a .nav-link button in the nav element, I am taken to the corresponding section of the landing page.  

User Story #6: I can watch an embedded product video with id="video".  

User Story #7: My landing page has a form element with a corresponding id="form".  

User Story #8: Within the form, there is an input field with id="email" where I can enter an email address.  

User Story #9: The #email input field should have placeholder text to let the user know what the field is for.  

User Story #10: The #email input field uses HTML5 validation to confirm that the entered text is an email address.  

User Story #11: Within the form, there is a submit input with a corresponding id="submit".  

User Story #12: When I click the #submit element, the email is submitted to a static page (use this mock URL: https://www.freecodecamp.com/email-submit).  

User Story #13: The navbar should always be at the top of the viewport.  

User Story #14: My product landing page should have at least one media query.  

User Story #15: My product landing page should utilize CSS flexbox at least once.  

You can build your project by using this CodePen template and clicking Save to create your own pen. Or you can use this CDN link to run the tests in any environment you like: https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js  

Once you're done, submit the URL to your working project with all its tests passing.  

# Build a Technical Documentation Page

Objective: Build a CodePen.io app that is functionally similar to this: https://codepen.io/freeCodeCamp/full/NdrKKL.  

Fulfill the below user stories and get all of the tests to pass. Give it your own personal style.  

You can use HTML, JavaScript, and CSS to complete this project. Plain CSS is recommended because that is what the lessons have covered so far and you should get some practice with plain CSS. You can use Bootstrap or SASS if you choose. Additional technologies (just for example jQuery, React, Angular, or Vue) are not recommended for this project, and using them is at your own risk. Other projects will give you a chance to work with different technology stacks like React. We will accept and try to fix all issue reports that use the suggested technology stack for this project. Happy coding!  

User Story #1: I can see a main element with a corresponding id="main-doc", which contains the page's main content (technical documentation).  

User Story #2: Within the #main-doc element, I can see several section elements, each with a class of main-section. There should be a minimum of 5.  

User Story #3: The first element within each .main-section should be a header element which contains text that describes the topic of that section.  

User Story #4: Each section element with the class of main-section should also have an id that corresponds with the text of each header contained within it. Any spaces should be replaced with underscores (e.g. The section that contains the header "JavaScript and Java" should have a corresponding id="JavaScript_and_Java").  

User Story #5: The .main-section elements should contain at least 10 p elements total (not each).  

User Story #6: The .main-section elements should contain at least 5 code elements total (not each).  

User Story #7: The .main-section elements should contain at least 5 li items total (not each).  

User Story #8: I can see a nav element with a corresponding id="navbar".  

User Story #9: The navbar element should contain one header element which contains text that describes the topic of the technical documentation.  

User Story #10: Additionally, the navbar should contain link (a) elements with the class of nav-link. There should be one for every element with the class main-section.  

User Story #11: The header element in the navbar must come before any link (a) elements in the navbar.  

User Story #12: Each element with the class of nav-link should contain text that corresponds to the header text within each section (e.g. if you have a "Hello world" section/header, your navbar should have an element which contains the text "Hello world").  

User Story #13: When I click on a navbar element, the page should navigate to the corresponding section of the main-doc element (e.g. If I click on a nav-link element that contains the text "Hello world", the page navigates to a section element that has that id and contains the corresponding header.  

User Story #14: On regular sized devices (laptops, desktops), the element with id="navbar" should be shown on the left side of the screen and should always be visible to the user.  

User Story #15: My Technical Documentation page should use at least one media query.  

You can build your project by using this CodePen template and clicking Save to create your own pen. Or you can use this CDN link to run the tests in any environment you like: https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js  

Once you're done, submit the URL to your working project with all its tests passing.  

# Build a Personal Portfolio Webpage

Objective: Build a CodePen.io app that is functionally similar to this: https://codepen.io/freeCodeCamp/full/zNBOYG.  

Fulfill the below user stories and get all of the tests to pass. Give it your own personal style.  

You can use HTML, JavaScript, and CSS to complete this project. Plain CSS is recommended because that is what the lessons have covered so far and you should get some practice with plain CSS. You can use Bootstrap or SASS if you choose. Additional technologies (just for example jQuery, React, Angular, or Vue) are not recommended for this project, and using them is at your own risk. Other projects will give you a chance to work with different technology stacks like React. We will accept and try to fix all issue reports that use the suggested technology stack for this project. Happy coding!  

User Story #1: My portfolio should have a welcome section with an id of welcome-section.  

User Story #2: The welcome section should have an h1 element that contains text.  

User Story #3: My portfolio should have a projects section with an id of projects.  

User Story #4: The projects section should contain at least one element with a class of project-tile to hold a project.  

User Story #5: The projects section should contain at least one link to a project.  

User Story #6: My portfolio should have a navbar with an id of navbar.  

User Story #7: The navbar should contain at least one link that I can click on to navigate to different sections of the page.  

User Story #8: My portfolio should have a link with an id of profile-link, which opens my GitHub or FCC profile in a new tab.  

User Story #9: My portfolio should have at least one media query.  

User Story #10: The height of the welcome section should be equal to the height of the viewport.  

User Story #11: The navbar should always be at the top of the viewport.  

You can build your project by using this CodePen template and clicking Save to create your own pen. Or you can use this CDN link to run the tests in any environment you like: https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js  

Once you're done, submit the URL to your working project with all its tests passing.  