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
>* In the above example, the CSS rule opens with a  [selector](https://developer.mozilla.org/en-US/docs/Glossary/CSS_Selector). This selects the HTML element that we are going to style. In this case, we are styling level one headings ([h1](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements)).
>* We then have a set of curly braces `{ }`.
>* Inside the braces will be one or more declarations, which take the form of property and value pairs. We specify the property (`color` in the above example) before the colon, and we specify the value of the property after the colon (`red` in this example).
>* This example contains two declarations, one for `color` and the other for `font-size`. Each pair specifies a property of the element(s) we are selecting (`h1` in this case), then a value that we'd like to give the property.

CSS properties have different allowable values, depending on which property is being specified. In our example, we have the `color` property, which can take various [color values](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units#color). We also have the `font-size` property. This property can take various [size units](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units#numbers_lengths_and_percentages) as a value.

A CSS stylesheet will contain many such rules, written one after the other.

    h1 {
      color: red;
      font-size: 5em;
    }

    p {
      color: black;
    }
>Note: You can find links to all the CSS property pages (along with other CSS features) listed on the MDN CSS reference. Alternatively, you should get used to searching for "mdn css-feature-name" in your favorite search engine whenever you need to find out more information about a CSS feature. For example, try searching for "mdn color" and "mdn font-size"!




---

## CSS Modules



As there are so many things that you could style using CSS, the language is broken down into modules. You'll see reference to these modules as you explore MDN. Many of the documentation pages are organized around a particular module. For example, you could take a look at the MDN reference to the [Background and Borders Module](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Backgrounds_and_Borders) to find out what its purpose is and the properties and features it contains. In that module, you will also find a link to Specifications that defines the technology (also see the section below).

---

## CSS Specifications


All web standards technologies (HTML, CSS, JavaScript, etc.) are defined in giant documents called specifications (or "specs"), which are published by standards organizations (such as the [W3C](https://developer.mozilla.org/en-US/docs/Glossary/W3C), [WHATWG](https://developer.mozilla.org/en-US/docs/Glossary/WHATWG), [ECMA](https://developer.mozilla.org/en-US/docs/Glossary/ECMA), or [Khronos](https://developer.mozilla.org/en-US/docs/Glossary/Khronos)) and define precisely how those technologies are supposed to behave.      

CSS is no different — it is developed by a group within the W3C called the [CSS Working Group](https://www.w3.org/Style/CSS/). This group is made of representatives of browser vendors and other companies who have an interest in CSS. There are also other people, known as invited experts, who act as independent voices; they are not linked to a member organization.     

New CSS features are developed or specified by the CSS Working Group — sometimes because a particular browser is interested in having some capability, other times because web designers and developers are asking for a feature, and sometimes because the Working Group itself has identified a requirement. CSS is constantly developing, with new features becoming available. However, a key thing about CSS is that everyone works very hard to never change things in a way that would break old websites. A website built in 2000, using the limited CSS available then, should still be usable in a browser today!     

As a newcomer to CSS, it is likely that you will find the CSS specs overwhelming — they are intended for engineers to use to implement support for the features in user agents, not for web developers to read to understand CSS. Many experienced developers would much rather refer to MDN documentation or other tutorials. Nevertheless, it is worth knowing that these specs exist and understanding the relationship between the CSS you are using, the browser support (see below), and the specs.



---

## Browser Support Information

>* After a CSS feature has been specified, then it is only useful for us in developing web pages if one or more browsers have implemented the feature.
>* This means that the code has been written to turn the instruction in our CSS file into something that can be output to the screen. We'll look at this process more in the lesson How CSS works.     
>* It is unusual for all browsers to implement a feature at the same time, and so there is usually a gap where you can use some part of CSS in some browsers and not in others. For this reason, being able to check implementation status is useful.

>* The browser support status is shown on every MDN CSS property page in a table named "Browser compatibility". Consult the information in that table to check if the property can be used on your website. For an example, see the [browser compatibility table for the CSS font-family property](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family#browser_compatibility).    

Based on your requirements, you can use the browser compatibility table to check how this property is supported across various browsers, or check if your specific browser and the version you have support the property, or if there are any caveats you should be aware of for the browser and version you are using.

---

## Summary






---

## Resources

* [Video](https://youtu.be/spK_S0HfzFw)
* [Mozila Developer Network](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS)
* [size units](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units#numbers_lengths_and_percentages)
* [color values](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units#color)
* [selector](https://developer.mozilla.org/en-US/docs/Glossary/CSS_Selector)
* [h1](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements)
* [Background and Borders Module](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Backgrounds_and_Borders)
* [W3C](https://developer.mozilla.org/en-US/docs/Glossary/W3C)
* [WHATWG](https://developer.mozilla.org/en-US/docs/Glossary/WHATWG)
* [ECMA](https://developer.mozilla.org/en-US/docs/Glossary/ECMA)
* [Khronos](https://developer.mozilla.org/en-US/docs/Glossary/Khronos)
* [CSS Working Group](https://www.w3.org/Style/CSS/)
* [browser compatibility table for the CSS font-family property](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family#browser_compatibility).
