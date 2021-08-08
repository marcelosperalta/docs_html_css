# [freeCodeCamp](https://www.freecodecamp.org/learn)

## [Responsive Web Design](https://www.freecodecamp.org/learn/responsive-web-design/)  

### Table of contents

[Basic HTML and HTML5](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#basic-html-and-html5)  
[Basic CSS](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#basic-css)  
[Applied Visual Design](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#applied-visual-design)  
[Applied Accessibility](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#applied-accessibility)  
[Responsive Web Design Principles](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#responsive-web-design-principles)  
[CSS Flexbox](https://github.com/marcelosperalta/study_html_css/tree/master/course_freecodecamp#css-flexbox)  

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