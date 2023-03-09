# `list-style-type`

|[Back To Home](/README.md)|[Back To Lesson 1](/01-lesson/1.2-GettingStartedWithCSS/readme.md)|
|-|-|

The `list-style-type` CSS property sets the marker (such as a disc, character, or custom counter style) of a list item element.     
The `color` of the marker will be the same as the computed color of the element it applies to.      
Only a few elements (`<li>` and `<summary>`) have a default value of `display: list-item`.
> However, the `list-style-type` property may be applied to any element whose `display` value is set to `list-item`.    
>Moreover, because this property is inherited, it can be set on a parent element (commonly `<ol>` or` <ul>`) to make it apply to all list items.

---

## Syntax

    /* Partial list of types */
    list-style-type: disc;
    list-style-type: circle;
    list-style-type: square;
    list-style-type: decimal;
    list-style-type: georgian;
    list-style-type: trad-chinese-informal;
    list-style-type: kannada;

    /* <string> value */
    list-style-type: "-";

    /* Identifier matching an @counter-style rule */
    list-style-type: custom-counter-style;

    /* Keyword value */
    list-style-type: none;

    /* Global values */
    list-style-type: inherit;
    list-style-type: initial;
    list-style-type: revert;
    list-style-type: revert-layer;
    list-style-type: unset;

>The list-style-type property may be defined as any one of:
>* a  `<custom-ident>` value,
>* a `symbols()` value,
>* a `<string>` value, or
>* the keyword `none`.

> Note that: 
>* Some types require a suitable font installed to display as expected.
>* The cjk-ideographic is identical to trad-chinese-informal; it exists for legacy reasons.

### Values

>* `<custom-ident>`
>> An identifier matching the value of a @counter-style or one of the predefined styles:
 
>* symbols()
>> Defines an anonymous style of the list.
 
>* `<string>`
>> The specified string will be used as the item's marker.
 
>* none
>> No item marker is shown.
 
>* disc
>> A filled circle (default value).
 
>* circle
>> A hollow circle.
 
>* square
>> A filled square.
 
>* decimal
>> Decimal numbers, beginning with 1.
 
>* cjk-decimal
>> Han decimal numbers.
 
>* decimal-leading-zero
>> Decimal numbers, padded by initial zeros.
 
>* lower-roman
>> Lowercase roman numerals.
 
>* upper-roman
>> Uppercase roman numerals.
 
>* lower-greek
>> Lowercase classical Greek.
 
>* lower-alpha, lower-latin
>> Lowercase ASCII letters.
 
>* upper-alpha, upper-latin
>> Uppercase ASCII letters.
 
>* arabic-indic, -moz-arabic-indic
>> Arabic-Indic numbers.
 
>* armenian
>> Traditional Armenian numbering.
 
>* bengali, -moz-bengali
>> Bengali numbering.
 
>* cambodian/khmer
>> Cambodian/Khmer numbering.
 
>* cjk-earthly-branch, -moz-cjk-earthly-branch
>> Han "Earthly Branch" ordinals.
 
>* cjk-heavenly-stem, -moz-cjk-heavenly-stem
>> Han "Heavenly Stem" ordinals.
 
>* cjk-ideographic
>> Identical to trad-chinese-informal.
 
>* devanagari, -moz-devanagari
>> Devanagari numbering.
 
>* ethiopic-numeric
>> Ethiopic numbering.
 
>* georgian
>> Traditional Georgian numbering.
 
>* gujarati, -moz-gujarati
>> Gujarati numbering.
 
>* gurmukhi, -moz-gurmukhi
>> Gurmukhi numbering.
 
>* hebrew
>> Traditional Hebrew numbering.
 
>* hiragana
>> Dictionary-order hiragana lettering.
 
>* hiragana-iroha
>> Iroha-order hiragana lettering.
 
>* japanese-formal
>> Japanese formal numbering to be used in legal or financial documents. The kanjis are designed so that they can't be modified to look like another correct one.
 
>* japanese-informal
>* Japanese informal numbering.
 
>* kannada, -moz-kannada
>> Kannada numbering.
 
>* katakana
>> Dictionary-order katakana lettering.
 
>* katakana-iroha
>> Iroha-order katakana lettering.
 
>* korean-hangul-formal
>> Korean hangul numbering.
 
>* korean-hanja-formal
>> Formal Korean Han numbering.
 
>* korean-hanja-informal
>> Korean hanja numbering.
 
>* lao, -moz-lao
>> Laotian numbering.
 
>* lower-armenian
>> Lowercase Armenian numbering.
 
>* malayalam, -moz-malayalam
>> Malayalam numbering.
 
>* mongolian
>> Mongolian numbering.
 
>* myanmar, -moz-myanmar
>> Myanmar (Burmese) numbering.
 
>* oriya, -moz-oriya
>> Oriya numbering.
 
>* persian, -moz-persian
>> Persian numbering.
 
>* simp-chinese-formal
>> Simplified Chinese formal numbering.
 
>* simp-chinese-informal
>> Simplified Chinese informal numbering.
 
>* tamil, -moz-tamil
>> Tamil numbering.
 
>* telugu, -moz-telugu
>> Telugu numbering.
 
>* thai, -moz-thai
>> Thai numbering.
 
>* tibetan
>> Tibetan numbering.
 
>* trad-chinese-formal
>> Traditional Chinese formal numbering.
 
>* trad-chinese-informal
>> Traditional Chinese informal numbering.
 
>* upper-armenian
>> Traditional uppercase Armenian numbering.
 
>* disclosure-open
>> Symbol indicating that a disclosure widget such as `<details>` is opened.
 
>* `disclosure-closed`    
>>Symbol indicating that a disclosure widget, like `<details>` is closed.

### Non-Standard Extension

A few more predefined types are provided by Mozilla (Firefox), Blink (Chrome and Opera) and WebKit (Safari) to support list types in other languages. See the compatibility table to check which browsers support which extension.

* -moz-ethiopic-halehame
* -moz-ethiopic-halehame-am
* ethiopic-halehame-ti-er, -moz-ethiopic-halehame-ti-er
* ethiopic-halehame-ti-et, -moz-ethiopic-halehame-ti-et
* hangul, -moz-hangul
* hangul-consonant, -moz-hangul-consonant
* urdu, -moz-urdu

---

## Accessibility concerns

Safari will not recognize an ordered or unordered list as a list in the accessibility tree if it has a `list-style-type` value of `none`. To learn more about this and potential workarounds, see list-style.

---

## Formal Defination

|||
|-|-|
|Initial value	|disc|
|Applies to	    |list items|
|Inherited      |yes|
|Computed value	|as specified|
|Animation type	|discrete|

---

## Formal Syntax

    list-style-type = 
      <counter-style>  |
      <string>         |
      none             

    <counter-style> = 
      <counter-style-name>  |
      <symbols()>           

    <symbols()> = 
      symbols( <symbols-type>? [ <string> | <image> ]+ )  

    <symbols-type> = 
      cyclic      |
      numeric     |
      alphabetic  |
      symbolic    |
      fixed       

    <image> = 
      <url>       |
      <gradient>  

    <url> = 
      url( <string> <url-modifier>* )  |
      src( <string> <url-modifier>* ) 

---

## Example

All List Style Types: 

HTML
