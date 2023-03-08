# Lesson 01 CSS First Steps

## 1.1 What Is CSS?

|[MDN-CSS](/README.md)|[Lesson 01](../readme.md)|
|-|-|
---

## Overview

* [Starting with some HTML](#starting-with-some-html)
* [Adding CSS to Our Document](#adding-css-to-our-document)
* [Styling HTML Elements](#styling-html-elements)
* [Changing the default behavior of elements](#changing-the-default-behavior-of-elements)
* [Adding a class](#adding-a-class)
* [Styling thing Based on their location in document](#styling-thing-based-on-their-location-in-document)
* [styling Things based on state](#styling-things-based-on-state)
* [Combining selectors and combinators](#combining-selectors-and-combinators)
* [Summary](#summary)

---

## Starting with some HTML

Our starting point is an HTML document. You can copy the code from below if you want to work on your own computer. Save the code below as index.html in a folder on your machine.

    <!DOCTYPE html>
    <html lang="en">
      <head>
        <meta charset="utf-8" />
        <title>Getting started with CSS</title>
      </head>
    
      <body>
        <h1>I am a level one heading</h1>
    
        <p>
          This is a paragraph of text. In the text is a
          <span>span element</span> and also a
          <a href="https://example.com">link</a>.
        </p>
    
        <p>
          This is the second paragraph. It contains an <em>emphasized</em> element.
        </p>
    
        <ul>
          <li>Item <span>one</span></li>
          <li>Item two</li>
          <li>Item <em>three</em></li>
        </ul>
      </body>
    </html>
    

|[Back to Top](#overview)|
|-|

---

## Adding CSS to Our Document

>The very first thing we need to do is to tell the HTML document that we have some CSS rules we want it to use. There are three different ways to apply CSS to an HTML document that you'll commonly come across,   
> — linking CSS from the head of your document.
>* Create a file in the same folder as your HTML document and save it as `styles.css`. The `.css` extension shows that this is a CSS file.

> To link styles.css to index.html, add the following line somewhere inside the <head> of the HTML document:
>* `<link rel="stylesheet" href="styles.css" />`    

> This `<link>` element tells the browser that we have a stylesheet, using the `rel` attribute, and the location of that stylesheet as the value of the `href` attribute. 

You can test that the CSS works by adding a rule to styles.css. Using your code editor, add the following to your CSS file:

    `h1 {
      color: red;
    }`

|[Back to Top](#overview)|
|-|

---

## Styling HTML Elements

>By making our heading red, we have already demonstrated that we can target and style an HTML element. We do this by targeting an element selector      
>* — this is a selector that directly matches an HTML element name. 
>* To target all paragraphs in the document, you would use the `selector p`.    

To turn all paragraphs green, you would use:

    p {
      color: green;
    }
> You can target multiple selectors at the same time by separating the selectors with a comma. 

If you want all paragraphs and all list items to be green, your rule would look like this:

    p,
    li {
      color: green;
    }

|[Back to Top](#overview)|
|-|

---

## Changing the default behavior of elements

When we look at a well-marked up HTML document, even something as simple as our example, we can see how the browser is making the HTML readable by adding some `default styling`.   
> Headings are large and bold and our list has bullets.     

This happens because browsers have `internal stylesheets` containing `default styles`, which they apply to all pages by default; without them all of the text would run together in a clump and we would have to style everything from scratch.     
>All modern browsers display HTML content by default in pretty much the same way.

However, you will often want something other than the choice the browser has made. This can be done by choosing the HTML element that you want to change and using a CSS rule to change the way it looks.   
>A good example is `<ul>`, an unordered list. It has list bullets.  
If you don't want those bullets, you can remove them like so:

    li {
      list-style-type: none;
    }
> [list-style-type](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-type) property is a good property to look at on MDN to see which values are supported.


|[Back to Top](#overview)|
|-|

---

## Adding a class

|[Back to Top](#overview)|
|-|

---

## Styling thing Based on their location in document

|[Back to Top](#overview)|
|-|

---

## styling Things based on state

|[Back to Top](#overview)|
|-|

---

## Combining selectors and combinators

|[Back to Top](#overview)|
|-|

---

## Summary

|[Back to Top](#overview)|
|-|

---
