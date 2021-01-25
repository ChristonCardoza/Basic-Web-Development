# Here You Find Basic Concepts of Web Development
Hi all,

Its Christon Cardoza, Now I'm gona teach you Basics of HTML and CSS Development

* * *

<p align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSnseJsow1HPz5SQI36lRNU0gqiY1sLlgkMSVsJB6Kv_5O0DNV5Iw&s"> 
</p>

# CSS (Cascading Style Sheet)

## What is Css?
 1. CSS stands for Cascading Style Sheet
 2. It is a  language used to give styling and design to websites
 3. It is the standard for styling websites, used by most/all websites across the globe.
 4. It usually goes hand-in-hand with HTML, while CSS3 brings lots of new features to the table.

## Why use CSS
 1. Styling
 2. Layout & Design
 3. Animations
 4. Font Changes
 5. Organization
 6. Grid Systems

## How is CSS used?
 1. Typically, a file is saved in the .css format, and linked to using an HtML tag.
 2. CSS selectors can be used to address parts of te page to style and use.
 3. HTML Elements are fiven Class and ID attributes, which are then used to manipulated in CSS.
 4. It typically folloes this method: Select, then Edit.

## What is a selector?
 1. Selectors are ways of grabbing and manipulating HTML.
 2. There are many different way to select, however they all turn out the same way.
 3. Different selectors have different applications.
 4. Types: 
      1. The Element Selector
           * You can select entire elements without any special charecters.
           * This applies to all of the elements with that tag on the page.
           * It ranks on the botttom of the specificity scale.
      2. The Class Selector
           * This is used to select elements with a certain class name.
           * Can be used on any and all elements with that class.
           * Can be used multiple times, and is select with the '.' symbol. 
      3. The ID Selector
           * This is used to select elements with a certain ID. 
           * Can be used on any and all elements with that ID.
           * unlike classes, it can only be used on one element at a time, and is selected with the  '#' symbol. However, it is possible to use more than once.

### What is psuedo selector?
 1. syntax :
    `<selector>:<psudoselctor>`
 2. Example :
    * `h2:hover {}`  
    * `li:first-child {}`
    * `li:last-child {}`
    * `li:nth-child(n) {}`
    * `li:only-child {}`
    * `a:link {}`
    * `a:visited {}`

### Advance Selector
 1. Adjcent sibling: If one selctor directly follows another
   syntax: `<beforeselctor> + <afterselctor>`   
   Ex : `h2 + a {}`
 2. General sibling: similar to above one but they should share same  parent
   syntax: `<beforeselctor> ~ <afterselctor>`   
   Ex : `textarea + button {}`
 3. Child: Every single child of selector ie direct child
   syntax: `<parent> > <child>`   
   Ex : `ul > li {}`
 4. Decendent : Same as above but also indirect child
   syntax: `<parent>  <child>`   
   Ex : `textarea  button {}`

### Attribute Selector
  syntax :
    `<selector>[<attribute>=<value>] {}` start with `^=`, end with `$=`, antwhere `*=`, separeted by whitespace `~ =` contains - `|=`

## Property
 1. Should writte in {}
 2. These are key vaue pait separate by colon ie :

### Color 
 1. color: 
   * rgb(R,G,B | 0 - 255)
   * rgba(R,G,B,0 or1)
   * css named color
   * hash code
 2. background:
   * css named color
   * hash code 
   * rgb(R,G,B | 0 - 255)
   * rgba(R,G,B,0 or1): Opacity or transparency
   * url()
   * linear-gradient(to bottom right |`<anglee>`, red,blue)
   * radial-gradenient(circle, red 20%, blue 40%, green 60%)
 3. background-repeat: 
   * no-repeat 
   * repeat
 4. background-size:
   * `<height>px <width>px`
   * cover
   * contain