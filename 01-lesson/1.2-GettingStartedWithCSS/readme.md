# Lesson 01 CSS First Steps

## 1.2 Getting Started with Css

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
* [Extra](#extra) 

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

So far, we have styled elements based on their HTML element names. This works as long as you want all of the elements of that type in your document to look the same.
>To select a subset of the elements without changing the others, you can add a class to your HTML element and target that class in your CSS.
1. In your HTML document, add a class attribute to the second list item. Your list will now look like this:

        <ul>
          <li>Item one</li>
          <li class="special">Item two</li>
          <li>Item <em>three</em></li>
        </ul>
2. In your CSS, you can target the class of special by creating a selector that starts with a full stop character. Add the following to your CSS file:

        .special {
          color: orange;
          font-weight: bold;
        }
> What is `class`?  
>* The `class` global attribute is a space-separated list of the case-sensitive classes of the element.
>* Classes allow CSS and JavaScript to select and access specific elements via the class selectors or functions like the DOM method `document.getElementsByClassName`.

Sometimes you will see rules with a selector that lists the HTML element selector along with the class:     

    li.special {
      color: orange;
      font-weight: bold;
    }
>This syntax means "target any li element that has a class of special". If you were to do this, then you would no longer be able to apply the class to a `<span>` or another element by adding the class to it;     
you would have to add that element to the list of selectors:  

    li.special,
    span.special {
      color: orange;
      font-weight: bold;
    }
As you can imagine, some classes might be applied to many elements and you don't want to have to keep editing your CSS every time something new needs to take on that style.        
Therefore, it is sometimes best to bypass the element and refer to the class, unless you know that you want to create some special rules for one element alone, and perhaps want to make sure they are not applied to other things.

|[Back to Top](#overview)|
|-|

---

## Styling thing Based on their location in document

1. There are times when you will want something to look different based on where it is in the document. 
>*  there are two `<em>` elements — one inside a paragraph and the other inside a list item.
>* To select only an `<em>` that is nested inside an `<li>` element, you can use a selector called the descendant combinator, which takes the form of a space between two other selectors

    li em {
      color: rebeccapurple;
    }
>* This selector will select any `<em>` element that is inside (a descendant of) an `<li>`. So in your example document, you should find that the `<em>` in the third list item is now purple, but the one inside the paragraph is unchanged.  
2. Something else you might like to try is styling a paragraph when it comes directly after a heading at the same hierarchy level in the HTML. To do so, place a + (an adjacent sibling combinator) between the selectors

        h1 + p {
          font-size: 200%;
        }

|[Back to Top](#overview)|
|-|

---

## styling Things based on state

> The final type of styling we shall take a look at in this tutorial is the ability to style things based on their state. A straightforward example of this is when styling links. 
>* When we style a link, we need to target the `<a>` (anchor) element.
>* This has different states depending on whether it is unvisited, visited, being hovered over, focused via the keyboard, or in the process of being clicked (activated).
>* You can use CSS to target these different states — the CSS below styles unvisited links pink and visited links green.

    a:link {
      color: pink;
    }

    a:visited {
      color: green;
    }
>* You can change the way the link looks when the user hovers over it, for example by removing the underline, which is achieved by the next rule:

    a:hover {
      text-decoration: none;
    }

> Note:     
>* you will often see mention of accessibility in these lessons and across MDN. When we talk about accessibility we are referring to the requirement for our webpages to be understandable and usable by everyone.     
>*  Your visitor may well be on a computer with a mouse or trackpad, or a phone with a touchscreen. Or they might be using a screen reader, which reads out the content of the document, or they may need to use much larger text, or be navigating the site using the keyboard only.     
>*  A plain HTML document is generally accessible to everyone — as you start to style that document it is important that you don't make it less accessible



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

## Extra

* [1. List Item Style type](./Extra/1-list-style-type/readme.md)
* []()
* []()
* []()
* []()
* []()

|[Back to Top](#overview)|
|-|

---