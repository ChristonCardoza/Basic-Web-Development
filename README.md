# Here You Find Basic Concepts of Web Development
Hi all,

Its Christon Cardoza, Now I'm gona teach you Basics of HTML and CSS Development

* * *

<p align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSnseJsow1HPz5SQI36lRNU0gqiY1sLlgkMSVsJB6Kv_5O0DNV5Iw&s"> 
</p>

# Chapter - 0 (Introduction to CSS)

HTML is just a skeletal layout of a website. We need CSS to design a website, add styles to it and make it look beautiful.

## What is CSS
 CSS stands for cascading styles sheets. CSS is optional but it converts an off  looking HTML page into a beautiful & responsive website.

 1. CSS stands for Cascading Style Sheet
 2. It is a  language used to give styling and design to websites
 3. It is the standard for styling websites, used by most/all websites across the globe.
 4. It usually goes hand-in-hand with HTML, while CSS3 brings lots of new features to the table.
 
## Why Learn CSS
 CSS is a very demanded skill in the world of web development. If you are successfully able to master CSS you can customize your website as per your liking. 

 1. Styling
 2. Layout & Design
 3. Animations
 4. Font Changes
 5. Organization
 6. Grid Systems

## Your first line of CSS
 Create a .css file inside your directory and add it to your HTML. Add the following line to your CSS
 ` body {
    background-color:red;
 }`

# Chapter - 1 (Creating our first CSS Website)

## What is DOM?
DOM stands for document object model. When a page is loaded, the browser created a DOM of the page which is constructed as a tree of objects.

## How is CSS used?
 1. Typically, a file is saved in the .css format, and linked to using an HtML tag.
 2. CSS selectors can be used to address parts of te page to style and use.
 3. HTML Elements are given Class and ID attributes, which are then used to manipulated in CSS.
 4. It typically follows this method: Select, then Edit.

## What is a selector?
 1. Selectors are ways of grabbing and manipulating HTML.
 2. There are many different way to select, however they all turn out the same way.
 3. Different selectors have different applications.
 4. Types: 
      1. The Element Selector
           * You can select entire elements without any special characters.
           * This applies to all of the elements with that tag on the page.
           * It ranks on the bottom of the specificity scale.
           ```
            H2 {
                  color: blue;
            }
           ``` 
      2. The Class Selector
           * This is used to select elements with a certain class name.
           * Can be used on any and all elements with that class.
           * Can be used multiple times, and is select with the '.' symbol. 
           ```
            .red {
                     background: red;
            }
           ```
      3. The ID Selector
           * This is used to select elements with a certain ID. 
           * Can be used on any and all elements with that ID.
           * unlike classes, it can only be used on one element at a time, and is selected with the  '#' symbol. However, it is possible to use more than once.
           ```
            #first {
                     color: white;
                     background: black;
            }
           ``` 

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
 1. Should written in {}
 2. These are key value pair separate by colon ie :

## Chapter - 1 (Practice Set)
 1. Create a website with a class red div which has a background color of the red and color white.
 2. Create an element with id head and verify that background color works on its as inline, external as well a using style tag CSS.
 3. Create a CSS class one and verify that it works on multiple elements.
 4. Create multiple CSS classes and verify that all of these work on the same element.
 5. Have a look at MDN CSS reference and try to play around with few key-value CSS rules.
   

# Chapter -2 (Colors & Backgrounds)

 1. color: 
   The CSS color property can be used to set the text color inside an element
    * RGB/RGB(R,G,B,0 or1): Specify color using Red, Green, Blue and Alpha  E.g. rgb(200,98,70)
    * HSL/HSLA: Specify Hue, Saturation, Lightness and Alpha  E.g. hsl(8,90%,63%)
    * css named color
    * hash code E.g. #ff7180
   
 2. background:
    * background-color: Specify the background color of a container.

      ```
         .brown {
                  background-color: brown;
         }
         ```
    * background-image: Used to set an image as the background. The image is by default repeated in X & Y directions.
  
      ```
         body {
            background-image: url(“harry.jpg”)
         }
         ```
    * background-repeat :

            repeat-x : repeat in the horizontal direction
            repeat-y : repeat in the vertical direction
            no-repeat : image not repeat

    * background-size:

            cover : fits & no empty space remains
            contain : fits & image is fully visible
            auto : display in original size
            {{width}} : set width & height will be set automatically
            {{width}} {{height}} : set width & height

    * background-position : Sets the starting position of a background image.

      ```
         .div1{
            background-position: left top;
         }
      ```
    * background-attachment : Defines a scrollable/non-scrollable character of a background image.

      ```
         .div2{
            background-attachment: fixed
         }
      ```
    * background : A single property to set multiple background properties.

      ```
         .div3{
            background: red url(‘img.png’) no-repeat fixed right top;
         }
      ```
## Chapter – 2 (Practice Set)
   1. Create a dark blue navigation bar with light color items.
   2. Change the color of the main container on your page to dark red.
   3. Create a div and add a background image with a given width and height.
   4. Create a vertical box and add a fixed non-scrolling background to it.
   5. Verify that the background shorthand property works with some of the values skipped.


  
# Chapter – 3 (CSS Box Model)
 1. The css Box model is a series of positioning properties designed to help with layout.
 2. Each property work in a different way, and positioning the item with different spacing.
 3. The Box Model is the most commonly used way to position items.
 4. Each layer represent a different part of the model, and it can be stretched and sized either symmetrically or asymmetrically
  <p align="center">
    <img src="CSS\img\Modal.PNG"> 
  </p>

  * Setting Width & Height: We can set width and height in CSS as follows
  
      ```
         #box {
          height: 70px;
          width: 70px;
         }
          /* Total height = height + top/bottom padding + top/bottom border + top/bottom margin*/
      ``` 
  * Setting Margin & Padding: We can set margin and padding as follows
  
      ```
         .box{
            margin: 3px;        /* Sets top, bottom, left & right values*/
            padding: 4px;       /* Sets top, bottom, left & right values*/
         }

         .boxMain{
            margin: 7px 0px 2px 11px;      /*top, right, bottom, left*/
         }

         .boxLast{
            margin: 7px 3px;           /*(top & bottom) (left & right)*/
         }        
      ```
  * Setting Borders:We can set the border as follows
  
      ```
         .bx{
            border-width: 2px;
            border-style: solid;
            border-color: red;
         }
         set border: 2px solid red;
      ``` 
  * Border Radius:We can set border-radius to create rounded borders
  
      ```
         .div2{
          border-radius: 7px;
         }
       
      ``` 
 * Margin Collapse:When two margins from different elements overlap, the equivalent margin is the greater of the two. This is called margin collapse
  * Box Sizing:Determines what out of padding and border is included in elements width and height, Can be content-box or border-box
  
      ```
         .div1{
          box-sizing: border-box;
         }
         /* The content width and height includes, content + padding + border */
      ```  
## Chapter – 3 (Practice Set)

   1. Create a website layout. Add a header box, one content box, and one footer.
   2. Add borders and margins to question 1 (website layout)
   3. Did the margin collapse between the content box and footer?
   4. Add the box-sizing property to the content box. What changes did you notice?

# Chapter – 4 (Fonts & Display)

 * The display property:
  
      The CSS display property is used to determine whether an element is treated as a block/inline element & the layout used for its children (flexbox/grid/etc.)

 * display: inline

      Takes only the space required by the element. No line breaks before and after. Setting width/height (or margin/padding) not allowed.

 * display: block

      Takes full space available in width and leaves a newline before and after the element

 * display: inline-block

      Similar to inline but setting height, width, margin, and padding is allowed. Elements can sit next to each other

 * display: none vs visibility: hidden

      With display: none, the element is removed from the document flow. Its space is not blocked.

      With visibility: hidden, the element is hidden but its space is reserved.

 * text-align 

      Used to set the horizontal alignment of a text
      ```
         .div1{
                  text-align: center;
         }
      ```
 * text-decoration 

      Used to decorate the text.Can be overline, line-through, underline, none

  * text-transform

      Used to specify uppercase and lowercase letters in a text
      ```
         p.uppercase{
                  text-transform: uppercase;
         }
      ```

  * line-height

      Used to specify the space between lines
      ```
      .Small{
               line-height: 0.7;
      }
      ``` 

  * Font Property

      Font plays a very important role in the look and feel of a website

  * Font-family

      Font family specifies the font of a text. It can hold multiple values as a “fallback” system
      ```
         p{
                  font-family: “Times new Roman”, monospace;
         }
      ```
  * Web Safe Fonts

      These fonts are universally installed across browsers

  * How to add Google Fonts

      In order to use custom google fonts, go to google fonts then select a style, and finally paste it to the style.css of your page.

  * Other Font Properties

         Some of the other font properties are listed below:

         font-size: Sets the size of the font

         font-style: Sets the font style

         font-variant: Sets whether the text is displayed in small-caps

         font-weight: sets the weight of the font

  * Generic Families

         A broad class of similar fonts e.g. Serif, Sans-Serif

         Just like when we say fruit, it can be any fruit

         When we say Serif it can be any Serif font

         font-family – Specific

         Generic family - Generic

## Chapter – 4 (Practice Set)
1. Create the following website layout,
2. Add a footer with Google Font “Ballu Bhai” to question 1.
3. Remove the underlines from links in question 1.
4. Demonstrate the difference between display: none and visibility: hidden using a div.
5. Change the footer to all uppercase in question 1.

https://www.codewithharry.com/videos/css-in-one-video
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


