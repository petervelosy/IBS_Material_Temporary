
# First website workshop

Get a feel of basic HTML and CSS while creating a simple personal landing page.

Focus on text styling (fonts, size, line height), basic layout and images.

## Objectives

- Using an editor
- Understanding how the browser opens a page
- Writing first HTML and CSS file
- Practicing basic HTML structure
- Using CSS
- Indentation and formatting

## Material review

### HTML

- html
  <!--  
  - creates the structure of the webpage
  - HyperText Markup Language
    - HyperText is text displayed on a computer or device that provides access
      to other text through links (aka hyperlinks)
    - markup language: a computer language that defines the structure and
      presentation of raw text
  -->
- html elements, tags
  <!-- 
  - HTML tags: wrapping the content
  - parts of an HTML element
    - opening tag (<p>)
    - the content (the information between the opening and closing tags)
    - a closing tag (</p>) (not always, self closing tags, br, img)
  - <html> tag is the root element of every page, or the parent element
  -->
- Doctype
  <!-- 
  - document type declaration
  - it must be in the very first row
  - for HTML5: <!DOCTYPE html>
  - it tells the browser that it is an html document and it should handle it
    like that
  -->
- head
  <!-- 
  - first child of the <html> tag
  - required for a valid HTML5 document
  - the <title> tag is also required inside the <head> tag for a valid HTML5
    document
  - the head's content is not displayed on the page
  - contains metadata about the document: title, scripts, style sheets, the 
    document's character encoding (utf-8), author, etc.
  -->
- body
  <!-- 
  - required element for a valid HTML5 document
  - child of the html tag
  - only content inside the opening and closing body tags can be displayed to
    the screen
  - <script> element: at the bottom of the document body (should be just before
    the closing </body> tag), in this tag we can connect our html document to a
    JS file, so we can add functionality to our webpage
    (Webpage:
    - HMTL: structure
    - JS: functionality
    - CSS: styling of our webpage)
  -->
- header
  <!-- 
  - Can contain company logo, hamburger menu bottom, navigation bar, links...
  - On the top of the page
  -->
- headings
  <!-- 
  - six different headings, or heading elements
  - purpose: titling sections, articles, or other forms of content
  - h1 tag is reserved for the headline of the page, the main topic, not to be
    confused with the page title
  - from a Web accessibility point of view, there should be only one h1 tag per
    page because this is the topic of the page, and there should be only one
    topic per page, like a Wikipedia article. There are usually multiple h2 tags
    per page
  - if you want your website to be accessible for assistive technology devices
    (such as screen readers), you cannot skip any heading, they must go in
    chronological order
  - if you want to adjust the sizes of the headings, that can be done without
    sacrificing the chronological order of the headings (with CSS)
  -->
- anchors
  <!-- 
  - is used to create hyperlinks in an HTML document
  - the hyperlinks can point to other webpages, files on the same server, a
    location on the same page, or any other URL via the hyperlink reference
    attribute, href which determines the location the anchor element points to
  - <target> attribute specifies where a hyperlink should be opened
    - "_blank":  opens the hyperlink in a new tab in modern browsers, or in a
      new window in older browsers
    - no target: default, url will open in the same tab, redirects
  - <a> can create hyperlinks to different parts of the same HTML document using
    the href attribute to point to the desired location with # followed by the
    id of the element to link to.
  -->
- p
  <!-- 
  - paragraph, contain a block of plain text
  -->
- strong
  <!-- 
  - The <strong> will generally render as bold emphasis.
  - opening and closing tags
  - The <em> tag will generally render as italic emphasis.
  -->
- div
  <!-- 
  - short for “division” 
  - container that divides the page into sections, grouping elements together
  - non-semantic, try to use semantic tags where you can instead of div-s
  - <div>-s can contain any text or other HTML elements, such as links, images,
    or videos
  -->
- img
  <!--  
  - self-closing: 
    - the end of the <img> tag has a forward slash /
    - it can not contain any content at all (only attributes)
    - self-closing tags may include or omit the final slash — both will render
      properly
  - required attribute called src and alt
  - alt attribute means alternative text, a description of the image
    - adding it is important because of web accessibility 
    - if an image fails to load on a web page, a user can mouse over the area
      originally intended for the image and read a brief description of it 
    - visually impaired users often browse the web with the aid of screen
      reading software. When you include the alt attribute, the screen reading
      software can read the image’s description out loud to the visually
      impaired user
    - the alt attribute also plays a role in Search Engine Optimization (SEO),
      because search engines cannot “see” the images on websites as they crawl
      the internet. Having descriptive alt attributes can improve the ranking of
      your site. 
  -->
  - image formats
    <!-- 
    - The <img> tag may support (depending on the browser) the following image
      formats: jpeg, gif, png, apng, svg, bmp, bmp ico, png ico.
    -->
- semantic tags
  <!-- 
  - semantic HTML refers to syntax that makes the HTML more comprehensible by
    better defining the different sections and layout of web pages
  - it makes web pages more informative and adaptable, allowing browsers and
    search engines to better interpret content
  - semantic elements are specifically designed to communicate meaning to the
    browser, developer, reader, and any other technologies interpreting the
    document (e.g. voice assistants)
  -->
- article
  <!-- 
  - defines a piece of self-contained content
  - it does not refer to the main content alone and can be used for comments and
    widgets 
  -->
- nav
  <!-- 
  - Navigational  Element (<nav>) defines a section that contains navigation
    links that appear often on a site
  - you can have primary and secondary menus, but you never nest, or put a <nav>
    element inside a <nav> element.
  -->
- main
  <!-- 
  - represents the dominant content of the <body> of a document
  - consists of content that is directly related to or expands upon the central
    topic of a document, or the central functionality of an application
  -->

### CSS

- what is CSS?
  <!--
  - Cascading Style Sheets
  - it is a style sheet language used for describing the presentation of a
    document written in a markup language like HTML: how they are styled, laid
    out, etc.
  - the cascade and the closely-related concept of specificity are mechanisms
    that control which rule applies when there is a conflict (two different
    rules applied to the same element)
  - the order of CSS rules matter: when two rules apply that have equal
    specificity, the one that comes last in the CSS is the one that will be used
  -->
- CSS rules and its parts:
  - selector
  - declaration (property, value)
    <!-- 
    - CSS rule is made up of two distinct parts:
    - the selector: selects the HTML element that we are going to style
    - the declaration: between {}-s
      - tells exactly what do we want to format, and how
      - also 2 parts:
        2.1. property: which aspect of the selector will be changed visually
        2.2. value: what the chosen CSS property will be changed to
      p {
        font-size: 12px;
      }
      p: selector
      font-size: property
      12px: value

      selectors:
      1. type selectors (e.g., h1) and pseudo-elements (e.g., ::before).
      2. class selectors (e.g., .example), 
        - attributes selectors (e.g., [type="radio"]) 
        - pseudo-classes (e.g., :hover).
        CSS classes are meant to be reused over many elements
      3. ID selectors (e.g., #example).
      4. Universal selectors –  * symbol which applies the CSS code to each and
      every element in body. (font-size, font-family)
    -->
- shorthand properties
  <!--
  - they are CSS properties that let you set the values of multiple other CSS
    properties simultaneously
  - example:
    background-color: #000;
    background-image: url(images/bg.gif);
    background-repeat: no-repeat;
    background-position: left top;

    it is the same:
    background: #000 url(images/bg.gif) no-repeat left top;
  -->
- color
  <!--
  - color is responsible for the color of the text
  - for background, use background-color
  -->
- box model
  <!--
  - all HTML elements can be considered as boxes
  - in CSS, the term "box model" is used when talking about design and layout
  - the CSS box model is essentially a box that wraps around every HTML element
  - it consists of: margins, borders, padding, and the actual content
  - the calculation of the dimensions (width or height) depends on the
    box-sizing property
  -->
- block vs. inline
  <!--
  - there are two types of boxes — block boxes and inline boxes (refering to 
    behaviour: page flow, relation to other boxes)
  - define in the display property ( display: block;)
  1. block:
    - fill the space available in its container. In most cases this means that
      the box will become as wide as its container
    - the box will break onto a new line
    - we can give it a width and height values
    - padding, margin and border will cause other elements to be pushed away
      from the box
    - unless we decide to change the display type to inline, elements such as
      headings (e.g. <h1>) and <p> all use block as their outer display type by
      default

  2. inline
    - the box will not break onto a new line
    - the width and height properties will not apply (takes as much space as the
      content needs, no more)
    - padding, margin and borders will apply but will not cause other inline
      boxes to move away from the box
    - default inline elements: <a>, <span>, <em>, <strong>, <img>

  3. inline-block
    - similar to inline elements, except they can have padding and margins added
      on all four sides
    - will not break onto new line 
  -->
- webfonts
  <!--
  - @font-face tag
  - there are several repositories offering a huge range of open source fonts
    which are served from a Content Delivery Network (CDN). Popular options:

    Google Fonts: https://fonts.google.com/
    Font Library: https://fontlibrary.org/
    Adobe Edge: https://edgewebfonts.adobe.com/

    Google Fonts is the most-used and provides searchable list, weight and style
    customization options, and load time estimation.

    To embed a font in a page, use the standard <link> tag in the HTML head, eg:

    <link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="stylesheet">
    The font will be downloaded and processed in parallel with your own
    stylesheet

    The web font can then be set in any CSS declaration, e.g:

    body {
      font-family: "Open Sans", sans-serif;
    }
  -->
- units (px, %, em, rem)
  <!-- 
  - a dimension is a number with a unit attached to it, for example 45deg, 5s,
    or 10px
  - font-size, padding, margin, height, width, line-height, etc.

  1. Absolute length units:
    - px: pixel, (1px = 1/96th of 1in (inch))

  2. Relative length units: relative to something else, perhaps the size of the 
    parent element's font, or the size of the viewport
    - em: font size of the parent element
    - rem: font size of the root element (<html>)
    - %: percentage of the font-size of the element's parent
  -->
- font-size
  <!--
  - can be given in length valus (12px), in absolute-size values (small),
    percentage (20%), in global (inherit) 
  - https://developer.mozilla.org/en-US/docs/Web/CSS/font-size
  -->
- line-height
  <!-- 
  - sets the height of a line box
  - commonly used to set the distance between lines of text
  1. normal
  - Depends on the user agent. Desktop browsers use a default value of roughly
    1.2
  2. <number> (unitless): USUALLY THIS IS THE PREFERRED WAY
  - The used value is this unitless <number> multiplied by the element's own
    font size. The computed value is the same as the specified <number>. In most
    cases, this is the preferred way to set line-height and avoid unexpected
    results due to inheritance.
  3. <length>
  - The specified <length> is used in the calculation of the line box height.
    Values given in em units may produce unexpected results
  4. <percentage>
  - Relative to the font size of the element itself. The computed value is this
    <percentage> multiplied by the element's computed font size. Percentage
    values may produce unexpected results as well.
  -->
- background
  <!--
  - shorthand CSS property sets all background style properties at once, such as
    color, image, origin and size, or repeat method
  - pro: short
  - con: harder to read
  -->
- background-image
  <!--
  - can be set with URL
  - background-repeat CSS property sets how background images are repeated.
    A background image can be repeated along the horizontal and vertical axes,
    or not repeated at all
  -->

### Environment

- Download and install [Visual Studio Code](https://code.visualstudio.com/)
  - If you use Hungarian keyboard layout, you might want to keep your sanity and
    change the default code running shortcut from `CTRL-ALT-B` to `CTRL-R`
    because the `}` symbol happens to be on the `B` key on hungarian layouts. To
    do this, go to `File -> Preferences -> Keyboard shortcuts` and search for
    `run code`.
- Download and install [Google Chrome](https://www.google.com/chrome)

### Tools

- Stack Overflow: <http://stackoverflow.com/>
- MDN: <https://developer.mozilla.org/en-US/>
- W3schools: <https://www.w3schools.com>

## Workshop

### Follow these steps

#### Keep things tidy

- Create a folder for today's exercise and and work in that folder (create
subfolder(s) if necessary)

#### Create your first page

- Create an HTML file using your editor called `index.html` and open it in your
browser

#### Start with the content

- Recreate the contents seen on the design, but use your own name
- Write two sentences about yourself and place it under your name

#### Make sure you have all these prepared

- Navigation bar with links
- Name
- Title
- Two short sentences
- A separator (just three dashes)
- The wiki definitions

#### Give it some structure

- What semantic role do these paragraphs fill? Divide it into a few separate
  HTML tags
- Try to figure out what HTML tags describe the content the best

#### Design

- Check out [the design](first-website-design.png) that you'll recreate

#### Add in style

- Create a `style.css` file and link it to your HTML
- Keep an eye on paddings, margins, line-heights, font-sizes
- The page should have a `10%` padding on the sides
- How do you center content on the page?
- Add a custom font for headings via
  [Google Fonts](https://www.google.com/fonts#UsePlace:use/Collection:Merriweather)
- Base text font should be `consolas, courier`
- Header background color is `#333333`
- Link and subtitle color is `#ff0099`
- Download the
  [page background pattern](https://www.toptal.com/designers/subtlepatterns/topography/)
- Use [this image](aperture.svg) for the header logo

#### Use these definitions in the wiki section *(ding dong)*

- Your task is to figure out what the title should be
- [Open the wiki](wiki.md) and try to guess the titles
- Copy these to your page

In case you have finished,
[you can continue with your own blog](https://github.com/green-fox-academy/teaching-materials/tree/master/project/blog)
&
[your own CV](https://github.com/green-fox-academy/teaching-materials/tree/master/project/cv-I)
