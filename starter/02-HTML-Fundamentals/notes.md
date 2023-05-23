# Intro to HTML

**HTML** -> Hyper Text Markup Language  
It is used to describe the content of a webpage (not a _programming language_)

An element is made up of three parts

- opening tag
- content of the element
- closing tag

# HTML Document structure

All HTML files require a html, body and head element

Elements in the head element will not necessarily be shown to the user

# Text elements

There are six "h" elements -> h1 to h6

![](https://github.com/j-koziel/html-css-course/blob/master/starter/02-HTML-Fundamentals/20230523104552.png)

Headings are used to break up text into logical sections

"p" elements are used to write more generic smaller text

A good practice is to only ever have **one** h1 element in each html page

You can use "b" elements to create bold text however it is deprecated and the "strong" element should be used instead as it has no **semantic** meaning

The same goes for the "i" element (italics). Use "em" (emphasise) instead

# More text elements: Lists

Ordered lists can be constructed with the "ol" element and "li" elements inside of it

Unordered lists are the same as an ordered list but with a "ul" element -> creates a bullet pointed list

# Images and attributes

The "img" element is one of those elements with no **content**  
Instead it uses attributes which provide it with information about the content

## Attributes

- The "src" attribute provides information as to the location of the image
- The "alt" attribute means alt text. This helps with accessibility and the browser knows what the image is.
- "width" and "height" attributes obviously change the size of the image
- The html element uses the "lang" attribute to specify the language of the page
- The head element requires meta elements (metadata) to describe the caracter set being used in the page

# Hyperlinks

Links can be put into two categories

- Links which lead to other pages on our website
- Links to other places on the internet which are **not** on our website

Use the "a" (anchor) element with the "href" attribute where you put your link

A usefull tool is to use the "target" attribute with the "\_blank" value. This will open the link in a new tab

# Structuring our page

It's good to put everything in containers as it makes it neat and organised

- "nav" element -> group links together
- "header" element -> the top part of a page
- "article" element -> good for blog posts or large pieces of text
- "footer" element -> the bottom part of the page

This is all part of _semantic_ html

# Semantic HTML

Certain elements have a meaning or purpose attached to them -> Not what it looks like but what it means and what it stands for

Not all elements are semantic

For example, the "em" element. It makes the text italics but it means to **em**phasise the text

The "div" element is just a box with no meaning -> Only use for containers where they have no meaning.

Semantic elements should be used for meaningful parts of the page
