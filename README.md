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
 2. These are key value pair separate by colon ie :

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
    * linear-gradient(to bottom right |`<angle>`, red,blue)
    * radial-gradenient(circle, red 20%, blue 40%, green 60%)
 3. background-repeat: 
    * no-repeat 
    * repeat
 4. background-size:
    * `<height>px <width>px`
    * cover
    * contain 

### Text
 1. text-decoration: 
    * underline
 2. text-align:
    * justify
 3. font-size:
    * em
    * cm
    * px
 4. font-weight:
 5. font-family:
    * `<font_name>,<if first font not found then default font name>`
  
## Box Modal
 1. The css Box model is a series of positioning properties designed to help with layout.
 2. Each peoperty work in a different way, and positioning the item with different spacing.
 3. The Box Modek is the most commonly used way to position items.
 4. Each layer represent a different part of the model, and it can be strtched and sized either symmetrically or asymetrically
  <p align="center">
    <img src="CSS\img\Modal.PNG"> 
  </p>

## Flex Box
 1. Flexbox stands for 'flexible box'
 2.  It is a display type that comes with a range of properties allowing you to arrange items easily.
 3. It is an alternative to using displays, floats and oter layout properties 
 4. A flexbox element is split into two main parts: the container, and the items.
 5. The container is the parent element in which the display type is active. This is usually in the form of a div.
 6. Flex items are child elemnts of the conatiner, and make up the contents of the box.
  <p align="center">
    <img src="CSS\img\Flexbox.PNG"> 
  </p>

## Grid Box
 1. Similarto Flexbox, Gid is a display type that can be used to activate certain layout features on a container element.
 2. They are both alternatives to other layout feature avialable in Css
  <p align="center">
    <img src="CSS\img\Grid.PNG"> 
  </p>

### Box
 1. border:
    * `<size> <style> <color>`
    * Style :- 
        * solid
        * dotted
        * double
 2. padding:
    * padding-right
    * padding-top
    * padding -left
    * padding-bottom
    * `<top> <right> <bottom> <left>`
 3. margin:
    * `<top-bottom> <left-right>`
 4. float:
    * right
    * left
 5. display:
    * none
    * inline
    * inline-block
    * flex
    * grid

### Flex
 1. display:flex
 2. flex-direction:
     * column
     * row
     * column-reverse
     * row-reverse
  3. flex-wrap:
     * wrap
     * nowrap
     * wrap-reverse 
  4. justify-content:
     * space-around
     * space-between
     * flex-end
     * center
  5. align-items:
     * center
     * flex-start
     * flex-end
     * stretch
     * baseline 
  6. flex-grow
  7. flex-strink
  8. flex-basis  

### Grid
 1. display:grid
 2. grid-template-columns: 
     * `<Column 1 size> <Column 2 size> .... <Column n size>`
 3. grid-template-rows: 
     * `<Row 1 size> <Row 2 size> .... <Row n size>`
 4. justify-content:
     * end
     * start
     * space-around
     * space-evenly
 5. align-content:
     * space-between
     * space-evenly
     * center
     * start
     * end
 6. grid-column-gap: `<size>`
 7. grid-row-gap: `<size>`
 8. grid-gap: 
     * `<column gap size> <row gap size>`
 9. grid-column:
     * `<column-start-at>/<column-end-at >` 
     * 1/3
     * 1/span 2
 10. grid-row:
     * `<row-start-at>/<row-end-at >` 
     * 1/3
     * 1/span 2
 11. grid-area:
     * `<row-start>/<column-start>/<row-end>/<column-end>`

### Transition
  1. transition:
     * all
     * `<where to apply> <property change time> <style of transition> <delay time>`
         * background
         * `<seconds or milisecond>`: duration from one property to another
         * `<ease or linear or ease-in-out>` : tansition style
         * `<seconds or milisecond>`: delay the peoperty
   2. transform:
      * translate(`<x-shilft> <y-shift>`)
      * scale(`<size-up>`)
      * rotate(`<angle in deg>`)
      * skewX(`<angle in deg>`)
      * skewY(`<angle in deg>`)
      * matrix(`<x-scale>, <x-skew>, <y-skew>, <y-scale>, <x-translate>, <y-translate>`)

### Animation
 1. Creating annimation
   * ```
      @Keyframes <name_of_anim> {

         from {.....}
         to {.....}

            OR

         0% {....}
         50% {....}
         100% {....}
      }
     ``` 
 2. Calling animation
   * animation-name: 
      * `<name_of_anim>`
   * animation-duration: 
      *  `<duration in seconds>`
   * animation-timing-function: 
      *  `<ease or linear or ease-in-out>`
   * animation-delay: `<duration in seconds>` 
      * 
   * animation-iteration-count:  
      * `<count in number or infinite >`
   * animation-direction: 
      *  `<normal or reverse or alternate or alternate-reverse>`
   * animation:  
      * `<animation-name> <animation-duration> <animation-timing-function > <animation-delay> <animation-iteration-count> <animation-direction>` 