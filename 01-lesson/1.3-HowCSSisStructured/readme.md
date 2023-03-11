# Lesson 01 CSS First Steps

## 1.3 How CSS Is Structured

|[MDN-CSS](/README.md)|[Lesson 01](../readme.md)|
|-|-|
---

## Overview

* [Applyin CSS To Html](#applyin-css-to-html)
* [Playing with CSS in this article](#playing-with-css-in-this-article)
* [Selectors](#selectors)
* [Properties And Values](#properties-and-values)
* [@rules](#rules)
* [Shorthands](#shorthands)
* [Comments](#comments)
* [White Space](#white-space)
* [Summary](#summary)

---

## Applyin CSS To Html

>three methods of applying CSS to a document:
>1. with an external stylesheet,
>2. with an internal stylesheet,
>3. and with inline styles.

### External Stylesheet

>An external stylesheet contains CSS in a separate file with a `.css` extension. This is the most common and useful method of bringing CSS to a document.   
> You can link a single CSS file to multiple web pages, styling all of them with the same CSS stylesheet. In the `Getting started with CSS`, we linked an external stylesheet to our web page.      

You reference an external CSS stylesheet from an HTML `<link>` element:     
``` 
<!DOCTYPE html>
<html lang="en-GB">
  <head>
    <meta charset="utf-8" />
    <title>My CSS experiment</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>This is my first CSS example</p>
  </body>
</html>
```
The CSS stylesheet file might look like this:   
```
h1 {
  color: blue;
  background-color: yellow;
  border: 1px solid black;
}

p {
  color: red;
}
```
>The href attribute of the `<link>` element needs to reference a file on your file system.      
> In the example above, the CSS file is in the same folder as the HTML document, but you could place it somewhere else and adjust the path.     
> Here are three examples:
```
<!-- Inside a subdirectory called styles inside the current directory -->
<link rel="stylesheet" href="styles/style.css" />

<!-- Inside a subdirectory called general, which is in a subdirectory called styles, inside the current directory -->
<link rel="stylesheet" href="styles/general/style.css" />

<!-- Go up one directory level, then inside a subdirectory called styles -->
<link rel="stylesheet" href="../styles/style.css" />
```

### Internal Stylesheet

>An internal stylesheet resides within an HTML document. To create an internal stylesheet, you place CSS inside a `<style>` element contained inside the HTML `<head>`.

The HTML for an internal stylesheet might look like this:
```
<!DOCTYPE html>
<html lang="en-GB">
  <head>
    <meta charset="utf-8" />
    <title>My CSS experiment</title>
    <style>
      h1 {
        color: blue;
        background-color: yellow;
        border: 1px solid black;
      }

      p {
        color: red;
      }
    </style>
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>This is my first CSS example</p>
  </body>
</html>
```
>In some circumstances, internal stylesheets can be useful. For example, perhaps you're working with a content management system where you are blocked from modifying external CSS files.

But for sites with more than one page, an internal stylesheet becomes a less efficient way of working. To apply uniform CSS styling to multiple pages using internal stylesheets, you must have an internal stylesheet in every web page that will use the styling. The efficiency penalty carries over to site maintenance too. With CSS in internal stylesheets, there is the risk that even one simple styling change may require edits to multiple web pages.

### Inline Styles

>Inline styles are CSS declarations that affect a single HTML element, contained within a style attribute.      
> The implementation of an inline style in an HTML document might look like this:
```
<!DOCTYPE html>
<html lang="en-GB">
  <head>
    <meta charset="utf-8" />
    <title>My CSS experiment</title>
  </head>
  <body>
    <h1 style="color: blue;background-color: yellow;border: 1px solid black;">
      Hello World!
    </h1>
    <p style="color:red;">This is my first CSS example</p>
  </body>
</html>
```
><b>Avoid using CSS in this way, when possible</b>. It is the opposite of a best practice.      
>* First, it is the least efficient implementation of CSS for maintenance. One styling change might require multiple edits within a single web page.
>* Second, inline CSS also mixes (CSS) presentational code with HTML and content, making everything more difficult to read and understand. Separating code and content makes maintenance easier for all who work on the website.

There are a few circumstances where inline styles are more common. You might have to resort to using inline styles if your working environment is very restrictive. For example, perhaps your CMS only allows you to edit the HTML body. You may also see a lot of inline styles in HTML email to achieve compatibility with as many email clients as possible.

|[Back to Top](#overview)|
|-|

---

## Playing with CSS in this article

1. For the exercise that follows, create a folder on your computer. You can name the folder whatever you want. Inside the folder, copy the text below to create two files:

index.html:
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width" />
    <title>My CSS experiments</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <p>Create your test HTML here</p>
  </body>
</html>
```

styles.css:     
```
/* Create your test CSS here */

p {
  color: red;
}
```

When you find CSS that you want to experiment with, replace the HTML `<body>` contents with some HTML to style, and then add your test CSS code to your CSS file.



|[Back to Top](#overview)|
|-|

---

## Selectors






|[Back to Top](#overview)|
|-|

---

## Properties And Values

|[Back to Top](#overview)|
|-|

---

## @rules


|[Back to Top](#overview)|
|-|

---

## Shorthands

|[Back to Top](#overview)|
|-|

---

## Comments

|[Back to Top](#overview)|
|-|

---

## White Space

|[Back to Top](#overview)|
|-|

---

## Summary

|[Back to Top](#overview)|
|-|

---