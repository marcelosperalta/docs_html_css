<div align="end">
    <img height="100" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/html/html.png" alt="HTML"/>
    &nbsp;&nbsp;
    <img height="100" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/css/css.png" alt="CSS"/>
</div>

# **[HTML](https://html.spec.whatwg.org/multipage/) and [CSS](https://www.w3.org/TR/CSS/#css) Docs**

## :arrow_heading_down: Table of Contents

* [Glossary](https://github.com/marcelosperalta/docs_html_css#glossary)
* [HTML](https://github.com/marcelosperalta/docs_html_css#html)
  * [Documentation](https://github.com/marcelosperalta/docs_html_css#documentation)
  * [HTML elements reference](https://github.com/marcelosperalta/docs_html_css#html-elements-reference)
  * [Global attributes](https://github.com/marcelosperalta/docs_html_css#global-attributes)
  * [Debug](https://github.com/marcelosperalta/docs_html_css#debug-debugging)
  * [Tools](https://github.com/marcelosperalta/docs_html_css#tools)
  * [Courses](https://github.com/marcelosperalta/docs_html_css#courses)
* [CSS](https://github.com/marcelosperalta/docs_html_css#css)
  * [Documentation](https://github.com/marcelosperalta/docs_html_css#documentation-1)
  * [style](https://github.com/marcelosperalta/docs_html_css#style)
  * [Design System Tools](https://github.com/marcelosperalta/docs_html_css#design-system-tools)
  * [Preprocessor](https://github.com/marcelosperalta/docs_html_css#preprocessor)
  * [CSS-in-JS](https://github.com/marcelosperalta/docs_html_css#css-in-js)
  * [Design methodologies](https://github.com/marcelosperalta/docs_html_css#design-methodologies)
  * [Framework](https://github.com/marcelosperalta/docs_html_css#framework)
  * [Software development tool](https://github.com/marcelosperalta/docs_html_css#software-development-tool)
  * [Articles](https://github.com/marcelosperalta/docs_html_css#articles)
* [Responsive web design (RWD)](https://github.com/marcelosperalta/docs_html_css#responsive-web-design-rwd)
* [Prototyping / Wireframe](https://github.com/marcelosperalta/docs_html_css#prototyping--wireframe)
* [Design system / Design language](https://github.com/marcelosperalta/docs_html_css#design-system--design-language)
* [Fonts](https://github.com/marcelosperalta/docs_html_css#fonts)
* [Stock Photos](https://github.com/marcelosperalta/docs_html_css#stock-photos)
* [Content management system (CMS)](https://github.com/marcelosperalta/docs_html_css#content-management-system)

<hr>

## Glossary

* [Content management system](https://en.wikipedia.org/wiki/Content_management_system)
  * A content management system (CMS) is a computer software used to manage the creation and modification of digital content (content management). A CMS is typically used for enterprise content management (ECM) and web content management (WCM).
* [Modal window / Modal dialog](https://en.wikipedia.org/wiki/Modal_window)
  * In user interface design for computer applications, a modal window is a graphical control element subordinate to an application's main window. A modal window creates a mode that disables the main window but keeps it visible, with the modal window as a child window in front of it. Users must interact with the modal window before they can return to the parent application. This avoids interrupting the workflow on the main window. Modal windows are sometimes called heavy windows or modal dialogs because they often display a dialog box.
* [Responsive web design (RWD)](https://en.wikipedia.org/wiki/Responsive_web_design)
  * Responsive web design (RWD) or responsive design is an approach to web design that aims to make web pages render well on a variety of devices and window or screen sizes from minimum to maximum display size to ensure usability and satisfaction.
* [Website wireframe](https://en.wikipedia.org/wiki/Website_wireframe)
  * A website wireframe, also known as a page schematic or screen blueprint, is a visual guide that represents the skeletal framework of a website.The term wireframe is taken from other fields that use a skeletal framework to represent 3 dimensional shape and volume. Wireframes are created for the purpose of arranging elements to best accomplish a particular purpose. The purpose is usually driven by a business objective and a creative idea. The wireframe depicts the page layout or arrangement of the website's content, including interface elements and navigational systems, and how they work together.

<hr>

## HTML

### Documentation

* [WHATWG - current HTML standard](https://html.spec.whatwg.org/multipage/)
* [MDN web docs (Mozilla Developer Network) - HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)

### [HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

* \<html>
* \<base>
* \<head>
* \<link>
* \<meta>
* \<style>
* \<title>
* \<body>
* \<address>
* \<article>
* [...](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

### [Global attributes](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes)

Global attributes are attributes common to all HTML elements; they can be used on all elements, though they may have no effect on some elements[...](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes)

* class
* hidden
* id
* style 
* title
* [...](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes)

### Debug (_Debugging_)

* [Chrome DevTools](https://developer.chrome.com/docs/devtools/javascript/)
* [Firefox Developer Tools](https://firefox-dev.tools/)

### Tools

* Automated tool for improving the quality of web pages
  * [Lighthouse](https://developers.google.com/web/tools/lighthouse)

### Courses

* [freeCodeCamp - Responsive Web Design](./course_freecodecamp)  

<hr>

## CSS

### Documentation

* [W3C - current state of Cascading Style Sheets (CSS)](https://www.w3.org/TR/CSS/#css)
* [MDN web docs (Mozilla Developer Network) - CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)

### style

* [global attribute](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/style)

  ```
  <html>
  <head>
  </head>
  <body>
    <p style="color: red;">Global attribute</p>
  </body>
  </html>
  ```

* [HTML element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/style)

  ```
  <html>
  <head>
    <style>
      p {
        color: red;
      }
    </style>
  </head>
  <body>
    <p>HTML element</p>
  </body>
  </html>
  ```

* [file](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics)

  _index.html_  
  ```
  <html>
  <head>
      <link href="style.css" rel="stylesheet">
  </head>
  <body>
    <p>HTML element</p>
  </body>
  </html>
  ```

  _style.css_  
  ```
  p {
    color: red;
  }
  ```

### Design System Tools

* [Figma](https://www.figma.com/)
* [Zepelin](https://zeplin.io/)

### Preprocessor

* [Sass](https://sass-lang.com/)
* [Less](https://lesscss.org/)

### CSS-in-JS

* [Emotion](https://emotion.sh/docs/introduction)
* [styled-components](https://styled-components.com/)
    * [VSC Syntax highlighting and IntelliSense](https://marketplace.visualstudio.com/items?itemName=jpoissonnier.vscode-styled-components)
* [JSS](https://cssinjs.org/)
* [glamorous](https://glamorous.rocks/)
* [polished](https://polished.js.org/)

### Design methodologies

* [BEM](http://getbem.com/)

### Framework

* [Bootstrap](https://getbootstrap.com/)
* [Foundation](https://get.foundation/)
* [tailwindcss](https://tailwindcss.com/)

### Software development tool

* [PostCSS](https://postcss.org/)

### Articles

* :link: [Flexbox vs Grid - How to Build the Most Common HTML Layouts](https://www.freecodecamp.org/news/flexbox-vs-grid-how-to-build-the-most-common-html-layouts/)  
    * :file_folder: [article_ondrej_polesny](https://github.com/marcelosperalta/docs_html_css/tree/master/article_ondrej_polesny)

* :link: [HTML Center Text – How to CSS Vertical Align a Div](https://www.freecodecamp.org/news/html-center-text-how-to-css-vertical-align-a-div/)  
    * :file_folder: [article_said_hayani](https://github.com/marcelosperalta/docs_html_css/tree/master/article_said_hayani)

<hr>

## Responsive web design (RWD)

### Concepts

* [Mobile first](https://en.wikipedia.org/wiki/Responsive_web_design#Related_concepts)
* [Desktop first](https://designmodo.com/desktop-first-design-responsive/)

<hr>

## Prototyping / Wireframe

* [Figma](https://www.figma.com/)
* [InVisionApp](https://www.invisionapp.com/)
* [Whimsical](https://whimsical.com/)

<hr>

### Design system / Design language

* [Material Design](https://material.io/)
  * [Materialize](https://materializecss.com/)
  * [MUI](https://www.muicss.com/)
* [Ant Design](https://ant.design/)

<hr>

## Fonts

* [Google Fonts](https://fonts.google.com/)

<hr>

## Stock Photos

* [Unsplash](https://unsplash.com/)

<hr>

## Content management system (CMS)

* [contentful](https://www.contentful.com/)
* [WordPress](https://wordpress.com/)