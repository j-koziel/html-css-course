# Intro to HTML

**HTML** -> Hyper Text Markup Language  
It is used to describe the content of a webpage (not a _programming language_)

An element is made up of three parts

- opening tag
- content of the element
- closing tag

# HTML Document structure

All HTML files require a html, body and head tag
Elements in the head tag will not necessarily be shown to the user

# Text elements

There are six "h" tags -> h1 to h6

![](https://github.com/j-koziel/html-css-course/blob/master/starter/02-HTML-Fundamentals/20230523104552.png)

Headings are used to break up text into logical sections

"p" tags are used to write more generic smaller text

A good practice is to only ever have **one** h1 tag in each html page

You can use "b" tags to create bold text however it is deprecated and the "strong" tag should be used instead as it has no **semantic** meaning

The same goes for the "i" tag (italics). Use "em" (emphasise) instead

# More text elements: Lists

Ordered lists can be constructed with the "ol" tag and "li" tags inside of it

Unordered lists are the same as an ordered list but with a "ul" tag -> creates a bullet pointed list

# Images and attributes

The "img" tag is one of those elements with no **content**

Instead it uses attributes which provide it with information about the content

The src attribute provides information as to the location of the image

The alt attribute means alt text. This helps with accessibility and the browser knows what the image is.

width and height attributes obviously change the size of the image

The html tag uses the lang attribute to specify the language of the page

The head tag requires meta tags (metadata) to describe the caracter set being used in the page
