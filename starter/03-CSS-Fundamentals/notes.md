# Intro to CSS

CSS means **C**ascading **S**tyle **S**heets  
It describes the visual style and presentation of the content within HTML

There are a lot of properties which let you change the way elements look and are layed out

**YOU DO NOT NEED TO LEARN THEM ALL**

# Inline, Internal and External CSS

### **Inline CSS**

CSS code written inside the HTML element  
**SHOUlD NEVER BE USED**

### **Internal CSS**

This comes in the form of a "style" element inside the head  
Everything inside this element is CSS syntax

Better than inline styling but still not recommended for large style sheets -> seperation of concerns

### **External CSS**

Usually the best path to take as everything is nicely organised

Use the "link" element with the "href" and "rel" attributes to define the location of the css file (href) and the type of link this is (rel)

# Styling text

6 properties which let you style text:

- font-size: changes the size of the font. By default the font-size is 16px
- font-family: Different fonts for text
- text-transform: Change text to a different case (upper case, lower case etc)
- font-style: The style of the text (bold, italics etc)
- text-align: How the text is aligned relative to its parent element
- line-height: Space between each line of text

Other properties:

- font-weight: lets you make text bold

# Combining selectors

Makes the CSS file less repetetive and improves maintainability of styling

Descendant selectors select child elements

Not the most recommended way to do this as it is not maintainable

# Class and ID selectors

IDs are special attributes on HTML elements which can be selected inside CSS using the hash (#) selector

The big difference between classes and IDs is that each ID name is only allowed to be used once. However multiple elements can have the same class names

If the class name has a space it should seperated with a dash

Select classes using the dot (.) selector

Classes are most of the time better than IDs and should be used more as it makes your code more prepared for the future and will prevent unnecessary bugs

**Extra styling property**

- list-style: none; -> Removes bullet points from unordered lists

# Working with colors

Different ways to represent colours in CSS

## **RGB MODEL**

- Every color is represented with a combination of red, green, blue
- Each of the 3 base colours take a value between 0 and 255

![](20230524120047.png)

### RGB notation

- rgb(0, 255, 255) - regular
- rgba(0, 255, 255, 0.3) - with transparency ("alpha")

### Hexadecimal notation

- scale from 0 to ff - (255 in hexadecimal)
- #00**ff**_ff_
- shorthand - #0**f**_f_ -> When the colors have identical pairs

In practice hexadecimal is mostly used and rgba used for transparency

## CSS color properties

- color - Lets you change the color of an element in hexadecimal or rgb form
- background-color - Changes the background color of an element
- border - Takes in 3 values (size, style, color)
- border-top/bottom/left/right - Border at specific sides of the element

# Pseudo-classes

To select the first element of any list you can do this:

`li:first-child`

This will select all the first list elements in any lists

This selects the first child of the element and not the first occurence of that element

Works the same for `last-child`

# Styling hyperlinks

You shouldn't directly style the anchors

Instead use pseudo classes to style the links at different states

`a:link` pseudo-class only styles anchors which are real links

# CSS Theory #1: Conflicts between selectors

There could be multiple declarations for the same elements.

Different selectors have different priority in CSS:

1. IDs have the highest priority -> when there are multiple the last one will be applied
   1. Apparently it is more complex than this
2. Class or pseudo-class selectors
3. Element selector
4. Universal selector -> lowest priority

Misc:

1. Inline styles have higher priority than IDs
2. Declarations marked as `!important` have even more priority than inline styles -> Best to avoid this

# CSS Theory #2: Inheritance and the Universal selector

Some elements inherit their parent's styles.

This is a cool mechanic as it means that properties which are going to be shared among elements can be put into the body

The universal (`*`) selector selects all the elements inside the page

# CSS Theory #3: The CSS Box Model

The box model defines how elements are displayed on a webpage and how they are sized.

Content can range from anything like text to images.  
Define the width and height of the content

A border is a line around the element but still inside

Padding is invisible whitespace between the border and the content

Margin is the space outside of an element between other elements

The fill area is the area which gets filled with background color or a background image

Final element width = left border + left padding + width + right padding + right border

final element height = top border + top padding +height + bottom padding + bottom border

This is all just _default_ behaviour

# Using margins and paddings

An element with background colour can always use some padding to seperate it from the content of the element

Its good not to mix margin-top and margin-bottom because you can easily get confused

The space between elements (margin) is not added but rather the larger value is used.

# Adding dimensions

As mentioned in the box model, changing the height is not the final height. You have to add up the padding on both sides to get the final height

Setting the height to auto will automatically fit an image to the aspect ratio of the width. And vice versa

Percentages apply to the percentage of the _parent_ element. This is useful because it means as the size of the window changes the image will always stay at the same percentage -> ✨*auto resizing*✨.

# Centering a page

This is the hardest thing to achieve in life

Steps:

1. Put all of our content inside a container element (otherwise there is no content to center). Divs will work great
2. Add a width to that element. The elements inside the container can not be wider than the container
3. Add margins to the left and right of the container and set them to auto.
