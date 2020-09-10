## Html
**HTML-** defining the content
**CSS-** styling the content

### Attributes
* **id**- identifies an element
* **class**- classify element
* **src** - specifies source for embeddable content
* **href** - hyperlink reference to a linked resource
```html
<!DOCTYPE html>
``` 
tells web browser which version of HTML is being used.

![Imgur](https://i.imgur.com/zXYDN7R.jpg)

## Understanding CSS terms
### Selectors
Selectors generally target an attribute value such as id or class vlalue or target type
```{
}
```
  Selector targets and applies style

### Properties
A property determines the styles that will be applied to that element

### Values
values  eg `color:orange;`

## Working with selectors
### Type selectors
Type selectors target by their element type.
```css
div{
}
```
### Class selectors
Class selectorsallows to select element according to element's class attribute

**SELF CLOSING TAGS**
`<br>` `<embed>` `<hr>` `<img>` `<input>` `<link>` `<meta>` `<param>` `<source>` `<wbr>`
### Id selectors
id selecctors are even more precise than class selectors , as they target only one element at a time.

## Referencing CSS
* **INCLUDING IN HTML**
```html
<head>
  <style>...</style>
</head>
```
* **.css file**

```html
<head>
  <link rel="stylesheet" href="address">
</head>
```
## Using CSS Resets

Every web browser has its own default styles for different elements. How Google Chrome renders headings, paragraphs, lists, and so forth may be different from how Internet Explorer does. To ensure cross-browser compatibility, CSS resets have become widely used.

CSS resets take every common HTML element with a predefined style and provide one unified style for all browsers. These resets generally involve removing any sizing, margins, paddings, or additional styles and toning these values down. Because CSS cascades from top to bottom—more on that soon—our reset needs to be at the very top of our style sheet. Doing so ensures that those styles are read first and that all of the different web browsers are working from a common baseline.

There are a bunch of different resets available to use, all of which have their own fortes. One of the most popular resets is Eric Meyer’s reset, which has been adapted to include styles for the new HTML5 elements.

If you are feeling a bit more adventurous, there is also Normalize.css, created by Nicolas Gallagher. Normalize.css focuses not on using a hard reset for all common elements, but instead on setting common styles for these elements. It requires a stronger understanding of CSS, as well as awareness of what you’d like your styles to be.


### Cross-Browser Compatibility & Testing

`As previously mentioned, different browsers render elements in different ways. It’s important to recognize the value in cross-browser compatibility and testing. Websites don’t need to look exactly the same in every browser, but they should be close. Which browsers you wish to support, and to what degree, is a decision you will need to make based on what is best for your website.`

## Semantics
Semantic code describes the value of content on a page regerdless of style or apperance.
`<div>` and `<span>` don't  hold semantic value .THey are used for styling purpose.
### Block vs inline elements
* block
```css
display: block;
```
It has width, height, margin. its like block
eg: <p>

* inline
```css
display: inline;
```
It has no width, height,margin.
e.g
<span>
