# Lesson 01 CSS First Steps

## 1.1 What Is CSS?

|[MDN-CSS](/README.md)|[Lesson 01](../readme.md)|
|-|-|
---

## Overview

* [What is CSS for?](#what-is-css-for)
* [CSS Syntax](#css-syntax)
* [CSS Modules](#css-modules)
* [CSS Specifications](#css-specifications)
* [Browser Support Information](#browser-support-information)
* [Summary](#summary)





---

## What is CSS for?

* CSS is a language for specifying how documents are presented to users — how they are styled, laid out, etc.     
* Presenting a document to a user means converting it into a form usable by your audience. Browsers, like Firefox, Chrome, or Edge, are designed to present documents visually, for example, on a computer screen, projector, or printer.
>* Note: A browser is sometimes called a user agent, which basically means a computer program that represents a person inside a computer system.
>* Browsers are the main type of user agents we think of when talking about CSS, however, they are not the only ones.
>* There are other user agents available, such as those that convert HTML and CSS documents into PDFs to be printed.
* CSS can be used for very basic document text styling — for example, for changing the color and size of headings and links. It can be used to create a layout — for example, turning a single column of text into a layout with a main content area and a sidebar for related information. It can even be used for effects such as animation. Have a look at the links in this paragraph for specific examples.


---

## CSS Syntax

CSS is a rule-based language — you define the rules by specifying groups of styles that should be applied to particular elements or groups of elements on your web page.    

For example, you can decide to have the main heading on your page to be shown as large red text.

    h1 {
      color: red;
      font-size: 5em;
    }
>* In the above example, the CSS rule opens with a selector. This selects the HTML element that we are going to style. In this case, we are styling level one headings (`h1`).
>* We then have a set of curly braces `{ }`.
>* Inside the braces will be one or more declarations, which take the form of property and value pairs. We specify the property (`color` in the above example) before the colon, and we specify the value of the property after the colon (`red` in this example).
>* This example contains two declarations, one for `color` and the other for `font-size`. Each pair specifies a property of the element(s) we are selecting (`h1` in this case), then a value that we'd like to give the property.

CSS properties have different allowable values, depending on which property is being specified. In our example, we have the `color` property, which can take various color values. We also have the `font-size` property. This property can take various size units as a value.

A CSS stylesheet will contain many such rules, written one after the other.

    h1 {
      color: red;
      font-size: 5em;
    }
    
    p {
      color: black;
    }
    

---

## CSS Modules


---

## CSS Specifications


---

## Browser Support Information


---

## Summary

---

## Resources

* [Video](https://youtu.be/spK_S0HfzFw)
* [Mozila Developer Network](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS)