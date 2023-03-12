# Lesson 01 CSS First Steps

## 1.5 Styling a Biography Page - Assessment

|[MDN-CSS](/README.md)|[Lesson 01](../readme.md)|[index.html](./index.html)|
|-|-|-|
---

## Overview

1. [Starting Point](#1-starting-point)
1. [Project Brief](#2-project-brief)
1. [Hints And tips](#3-hints-and-tips)
1. [Example](#4-example)
1. [Assessment or Further help](#5-assessment-or-further-help)

|[Back to Top](#overview)|
|-|

---

## 1. Starting Point

You can work in the live editor below, or you can [download the starting point file](https://github.com/mdn/css-examples/blob/main/learn/getting-started/biog-download.html) to work with in your own editor. This is a single page containing both the HTML and the starting point CSS (in the head of the document). If you prefer you could move this CSS to a separate file and link to it when you create the example on your local computer.

Alternatively use an online tool such as [CodePen](https://codepen.io), [jsFiddle](https://jsfiddle.net), or [Glitch](https://glitch.com) to work on the tasks.



|[Back to Top](#overview)|
|-|

---

## 2. Project Brief

The following live example shows a biography, which has been styled using CSS. The CSS properties that are used are as follows — each one links to its property page on MDN, which will give you more examples of its use.

* [font-family](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family)
* [color](https://developer.mozilla.org/en-US/docs/Web/CSS/color)
* [border-bottom](https://developer.mozilla.org/en-US/docs/Web/CSS/border-bottom)
* [font-weight](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight)
* [font-size](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size)
* [font-style](https://developer.mozilla.org/en-US/docs/Web/CSS/font-style)
* [text-decoration](https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration)

In the interactive editor you will find some CSS already in place. This selects parts of the document using element selectors, classes, and pseudo-classes. Make the following changes to this CSS:

1. Make the level one heading pink, using the CSS color keyword hotpink.
2. Give the heading a 10px dotted [border-bottom](https://developer.mozilla.org/en-US/docs/Web/CSS/border-bottom) which uses the CSS color keyword purple.
```
h1 {
    /* color: #375e97; */
    color: hotpink;
    
    font-size: 2em;
    font-family: Georgia, 'Times New Roman', Times, serif;
    
    /* border-bottom: 1px solid #375e97; */
    border-bottom: 10px dotted purple;
  }
```
3. Make the level 2 heading italic.
4. Give the ul used for the contact details a [background-color](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color) of #eeeeee, and a 5px solid purple [border](https://developer.mozilla.org/en-US/docs/Web/CSS/border). Use some [padding](https://developer.mozilla.org/en-US/docs/Web/CSS/padding) to push the content away from the border.
```
h2 {
    font-size: 1.5em;
    font-style: italic;
  }
  ul{
    background-color: #eee;
    border: 5px solid purple;
    padding: 20px;
  }
```
5. Make the links green on hover.
```
a:hover {
    text-decoration: none;
    color: green;
  }
```



|[Back to Top](#overview)|
|-|

---

## 3. Hints And tips

|[Back to Top](#overview)|
|-|

---

## 4. Example

|[Back to Top](#overview)|
|-|

---

## 5. Assessment or Further help

|[Back to Top](#overview)|
|-|

---