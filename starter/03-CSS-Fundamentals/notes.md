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

# Combining selectors

Makes the CSS file less repetetive and improves maintainability of styling

Descendant selectors select child elements

Not the most recommended way to do this as it is not maintainable
