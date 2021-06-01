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
 1. Adjacent sibling: If one selctor directly follows another
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

            1. repeat-x : repeat in the horizontal direction
            2. repeat-y : repeat in the vertical direction
            3. no-repeat : image not repeat

    * background-size:

            1. cover : fits & no empty space remains
            2. contain : fits & image is fully visible
            3. auto : display in original size
            4. {{width}} : set width & height will be set automatically
            5. {{width}} {{height}} : set width & height

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

         1. font-size: Sets the size of the font
         2. font-style: Sets the font style
         3. font-variant: Sets whether the text is displayed in small-caps
         4. font-weight: sets the weight of the font

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

# Chapter – 5 (Size, Position & Lists)
There are more units for describing size other than ‘px’. There are rem, em, vw, vh, percentages, etc.

* What’s wrong with pixels?

      Pixels (px) are relative to the viewing device. For a device with the size 1920x1080, 1px is 1unit out of 1080/1920.

* Relative lengths

      These units are relative to the other length property. Following are some of the most commonly used relative lengths,

      1. em – unit relative to the parent font size, em means “my parent element’s font-size”
      2. rem – unit relative to the root font size (<html> tag)
      3. vw – unit relative to 1% viewport width
      4. vh – unit relative to 1% viewport height
      5. % - unit relative to the parent element
 
* Min/max- height/width property

      CSS has a min-height, max-height, and min-width, max-width property.

      If the content is smaller than the minimum height, minimum height will be applied.

      Similar is the case with other related properties.

* The position property

      Used to manipulate the location of an element. Following are the possible values:

      1. static: The default position. top/bottom/left/right/z-index has no effect
      2. relative : The top/bottom/left/right/z-index will now work. Otherwise, the element is in the flow of the document like static.
      3. absolute: The element is removed from the flow and is relatively positioned to its first non-static ancestor. top/bottom etc. works
      4. fixed: Just like absolute except the element is positioned relative to the browser window
      5. sticky: The element is positioned based on the user’s scroll position
 

* list-style property

      The list-style property is a shorthand for type, position, and image

   ```
      ul{
               list-style: square inside url(‘harry.jpg’)
      }

      /* ‘square’ in the above code is the list-style-type, ‘inside’ is the list-style-position and ‘harry.jpg’ is the list-style-image.  */
   ```

* z-index property

      The z-index property specifies the stack order of an element. It defines which layer will be above which in case of overlapping elements. 

## Chapter – 5 (Practice Set)
   1. Create a responsive navbar using relative lengths.
   2. Create a sticky navbar using the position property.
   3. Demonstrate the use of list-style property using a ul as an example.
   4. Demonstrate the use of z-index using an example.

# Chapter – 6 (Flexbox)
 ```
   .container{
          display: flex;  /*Initialize a flexbox*/
   }
 ```
 1. Flexbox stands for 'flexible box'
 2.  It is a display type that comes with a range of properties allowing you to arrange items easily.
 3. It is an alternative to using displays, floats and oter layout properties 
 4. A flexbox element is split into two main parts: the container, and the items.
 5. The container is the parent element in which the display type is active. This is usually in the form of a div.
 6. Flex items are child elemnts of the conatiner, and make up the contents of the box.
  <p align="center">
    <img src="CSS\img\Flexbox.PNG"> 
  </p>

  * The float property

         float property is simple. It just flows the element towards left/right 

  * The clear property
     
         Used to clear the float. It specifies what elements can float beside a given element 

  * flex-direction property
         
        Defines the direction towards which items are laid. Can be row (default), row-reverse, column and column-reverse

   * Flex properties for parent (flex container)

         1. flex-wrap: Can be wrap, nowrap, wrap-reverse. Wrap items as needed with this property
         2. justify-content: Defines alignment along the main axis
         3. align-items: Defines alignment along the cross axis
         4. align-content: Aligns a flex container’s lines when there is extra space in the cross axis
   
   * Flex properties for the children (flex items)

         1. order: Controls the order in which the items appear in the flex container
         2. align-self: Allows default alignment to be overridden for the individual flex items
         3. flex-grow: Defines the ability for a flex item to grow
         4. flex-shrink: Specifies how much a flex item will shrink relative to the rest of the flex items

## Chapter – 6 (Practice Set)

   1. Create a layout of your choice using float.
   2. Create the same layout in question 1 using flexbox.
   3. Create the following navigation bar using flexbox
   4. Create the following layout using flexbox,


# Chapter – 7 (CSS Grid & Media Queries)
 1. Similar to Flexbox, Gid is a display type that can be used to activate certain layout features on a container element.
 2. They are both alternatives to other layout feature available in CSS
 3. All direct children automatically become grid items
  <p align="center">
    <img src="CSS\img\Grid.PNG"> 
  </p>

  * The grid-column-gap property
   
         Used to adjust the space between the columns of a CSS grid 

  * The grid-row-gap property

         Used to adjust the space between the rows of a CSS grid

  * The grid-gap property
   
         .container {
                  display: grid;
                  grid-gap: 40px 100px;            /*40px for row and 100px for column*/
                  /* For a single value of grid-gap, both row and column gaps can be set in one value. */
               }
  
  *  properties for grid container:

         1. The grid-template-columns property can be used to specify the width of columns

         .container {
                  display: grid;
                  grid-template-columns: 80px 120px auto;
         }

         2. The grid-template-rows property can be used to specify the height of each row

         .container {
                  display: grid;
                  grid-template-rows: 70px 150px;
         }

         3. The justify-content property is used to align the whole grid inside the container.
         4. The align-content property is used to vertically align the whole grid inside the container.  

   * Following are the properties for grid item:

         1. The grid-column property defines how many columns an items will span. 
          
         .grid-item{
                  grid-column: 1/5;
         }

         2. The grid-row property defines how many rows an item will span.
         3. We can make an item to start on column 1 and space 3 columns like this:
        
         .item{
                  grid-column: 1/span 3;
         }
         

   * CSS Media Queries

         Used to apply CSS only when a certain condition is true.
         Syntax:

         @media only screen and (max-width: 800px) {
                           body{
                                    background: red;
                                    }
                  }
 
## Chapter – 7 (Practice Set)

1. Create a header with content using CSS grid.
2. Create the layouts created in chapter-6 practice set using CSS grid.
3. Create a webpage that is green on large devices, red on medium, and yellow on small devices.

# Chapter – 8 (Transforms, Transitions & Animations)

 1. CSS Transforms
  
         Transforms are used to rotate, move, skew or scale elements. They are used to create a 3-D effect.

         * The transform property
               Used to apply a 2-D or 3-D transformation to an element

         * The transform-origin property
               Allows to change the position of transformed elements.
               2D transforms – can change x & y-axis.3D transforms – can change Z-axis as well 

               CSS 2D transform methods
               
               1. scaleX()
               2. scaleY()
               3. scale()
               4. translate(`<x-shilft> <y-shift>`)
               5. scale(`<size-up>`)
               6. rotate(`<angle in deg>`)
               7. skewX(`<angle in deg>`)
               8. skewY(`<angle in deg>`)
               9. matrix(`<x-scale>, <x-skew>, <y-skew>, <y-scale>, <x-translate>, <y-translate>`)
               

               CSS 3D transform methods

               1. rotateX()
               2. rotateY()
               3. rotateZ()
         

 2. CSS Transitions

         Used to change property values smoothly, over a given duration.

         * The transition property
               The transition property is used to add a transition in CSS.

         * Following are the properties used for CSS transition:
               1. transition-property: The property you want to transition
               2. transition-duration: Time for which you want the transition to apply
               3. transition-timing-function: How you want the property to transition
               4. transition-delay: Specifies the delay for the transition
               5. All these properties can be set using a single shorthand property
                     transition: property duration timing-function delay;
                     transition: width 35 ease-in 25;
               6. Transitioning multiple properties
                     We can transition multiple properties as follows:
                     transition: opacity 15 ease-out 15, transform 25 ease-in;
 

1. CSS Animations

         Used to animate CSS properties with more control. We can use the @keyframes rule to change the animation from a given style to a new style.

            @keyframes harry {
                     from { width: 20px; }              /*Can change multiple properties*/
                     to { width: 31px; }
            }

         Properties to add Animations
            1. animation-name: name of the animation
            2. animation-duration: how long does the animation run?
            3. animation-timing-function: determines speed curve of the animation
            4. animation-delay: delay for the start of an animation
            5. animation-iteration-count: number of times an animation should run
            6. animation-direction: specifies the direction of the animation
 
            * animation-name: 
                 `<name_of_anim>`
            * animation-duration: 
                 `<duration in seconds>`
            * animation-timing-function: 
                 `<ease or linear or ease-in-out>`
            * animation-delay: 
                 `<duration in seconds>`  
            * animation-iteration-count:  
                 `<count in number or infinite >`
            * animation-direction: 
                 `<normal or reverse or alternate or alternate-reverse>`
            * animation:  
                 `<animation-name> <animation-duration> <animation-timing-function > <animation-delay> <animation-iteration-count> <animation-direction>` 

         Animation Shorthand
            All the animation properties from 1-6 can be applied like this:
               animation: harry 65 linear 15 infinite reverse;
 
            Using percentage value states with animation.We can use % values to indicate what should happen when a certain percent of animation is completed

               @keyframes harry {
                        0% {
                                 width: 20px;
                                 }
                        50% {
                                 width: 80px;
                                 }
                        100% {
                                 width: 200px;
                                 }
                        }
               Can add as many intermediate properties as possible
 

## Chapter – 8 (Practice Set)
1. Create a thin progress bar animation for a website.
2. Create the same progress bar using transition.
3. Create a rotating image animation using CSS.
4. Create a slider with 3 images using CSS.
 

# Project-1 E-Commerce Website
Create a homepage for an E-commerce website. Use media queries to make it responsive.
