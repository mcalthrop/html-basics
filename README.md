# html-basics

_Practical explanation and examples of some HTML basics_

## Overview

### Objectives

- understand the basics of how HTML works
- construct a simple web page using HTML

### Prerequisites

- access to a text editor or IDE and a web browser


## HTML essentials

### Purpose

HTML is the standard markup language for creating web pages. 

It has two primary purposes:

1. Defines what **content** (words, images, etc) that are displayed on a web page.
1. Ascribes **meaning** to the content (headings, paragraphs, etc).

> The acronym stands for **H**yper**t**ext **M**arkup **L**anguage.

### Constructs

> Open your editor or IDE, create a new and empty file called `index.html`, and be ready to add some text to it.

#### Elements/Tags

The basic construct of HTML is an **element** (also referred to as a **tag**).

The HTML element ascribes _meaning_, and the value inside the tag is the _content_.

Let's take a very simple example of how to mark up two paragraphs:

```html
<p>Pack my box with five dozen liquor jugs.</p>
<p>Exploring the zoo, we saw every kangaroo jump and quite a few carried babies.</p>
```

In this example, we can see the following for each paragraph:

- the `<p>` tag: this means that a paragraph (in this instance) is about to begin &ndash; referred to as an _opening tag_
- the `</p>` tag: means that the paragraph that was started by the `<p>` tag now finishes here &ndash; referred to as a _closing tag_
- the words inside the `<p>` and `</p>` tags are the _content_ of each paragraph.

> Now save the above code, and view the `index.html` file in your browser.

#### Nesting elements

It is also possible to _nest_ elements, which means having one element contain one or more other elements.

A useful example is a bulleted list. When structuring the list, we need to know a couple of things:

- where the whole list starts and ends
- where each item in the list starts and ends

In HTML, we define the list with what is called an _unordered list_, which is represented by the `<ul>` tag:

```html
<ul>
</ul>
```

So now that we have the start and end of the list, we can add _list items_ inside:

```html
<ul>
  <li>alpha</li>
  <li>beta</li>
  <li>gamma</li>
</ul>
```

Note the following about the above example:

- the `<ul>` element can be referred to as the **parent** element of the `<li>` elements
- the `<li>` elements will then be referred to as **child** elements of the `<ul>` element
- each `<li>` element is a **sibling** element of the other `<li>` elements

> Save and view in your browser.

#### Attributes

There is one final aspect of HTML elements that we need to cover: **attributes**.

Attributes essentially provide additional information about an element.

A useful example is `<img>`, the HTML element that allows us to insert an image:

```html
<img src="http://vignette1.wikia.nocookie.net/suburgatory/images/5/52/Happy_face.jpg" />
```

Note the following about the above HTML snippet:

- `src` is the _attribute name_
- which is followed by the `=` sign
- which is followed by the _attribute value_: `"http://vignette1.wikia.nocookie.net/suburgatory/images/5/52/Happy_face.jpg"` &ndash; the browser knows to interpret this as the location of the image 
- there is no `</img>` element &ndash; this is known as a _self-closing tag_ (in the case of an image, there is no need for the element to have any content)
- HTML attributes are always specified in the _starting tag_.

> Save and view in your browser.


## Constructing a web page

### Basic structure

Using what we have learned so far, we'll now look at the basic structure of an HTML web page.

An HTML document will start off looking like this:

```html
<!DOCTYPE html>
<html>
</html>
```

You can see that `<html>` is the _root_ element: all other elements will be added as a child elements, in a hierarchical manner.

We can now add the `<head>` and `<body>` elements:

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- this section contains information about the HTML document -->
    <title>HTML basics</title>
  </head>
  <body>
    <!-- and this section contains the main body of the HTML document -->
    <p>This is the day your life will surely change.</p>
  </body>
</html>
```

Note the following:

- the `<title>` tag contains the text that is displayed in the tab in your browser
- the syntax of a comment in HTML: it begins with `<!--` and ends with `-->`.

> Save and view in your browser.

### Putting it all together

We can now incorporate all the HTML we have done so far, plus introduce some more HTML tags that are commonly used.

Replace everything that is in your `index.html` file with the following:

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- this section contains information about the HTML document -->
    <title>HTML basics</title>
  </head>
  <body>
    <!-- and this section contains the main body of the HTML document -->
    <h1>The basics of HTML</h1>

    <h2>Several paragraphs</h2>
    
    <p>This is the day your life will surely change.</p>
    <p>Pack my box with five dozen liquor jugs.</p>
    <p>Exploring the zoo, we saw every kangaroo jump and quite a few carried babies.</p>

    <h2>Lists</h2>
    
    <h3>Unordered</h3>
    <ul>
      <li>alpha</li>
      <li>beta</li>
      <li>gamma</li>
    </ul>

    <h3>Ordered</h3>
    
    <ol>
      <li>break eggs</li>
      <li>add flour</li>
      <li>add sugar</li>
      <li>shove in the oven</li>
      <li>hope for the best</li>
    </ol>
    
    <h3>Images</h3>
    
    <img src="http://vignette1.wikia.nocookie.net/suburgatory/images/5/52/Happy_face.jpg" />
    <img src="http://i.ytimg.com/vi/VQtbKGzI9SE/hqdefault.jpg" />
  </body>
</html>
```

> Save and view in your browser.

## Conclusion

### What we've covered

- explained the purpose and use of HTML
- put together a simple HTML page that containing several commonly-used HTML elements

### Further reading

- https://www.w3schools.com/html/html_elements.asp
- https://www.w3schools.com/html/html_attributes.asp
- https://en.wikipedia.org/wiki/HTML5
- http://www.evolutionoftheweb.com/
- https://en.wikipedia.org/wiki/XML

