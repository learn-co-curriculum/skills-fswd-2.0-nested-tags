# Nested HTML Tags

## Problem Statement

HTML elements are like boxes that hold content. You can think of the structure somewhat
like a Matryoshka doll set, which has a wooden doll, inside of a wooden doll, and 
**This is a bit of a culturally specific reference. Would it be better to use something like an onion?**
so on. These HTML elements that are "inside" of other are what are known as 
"nested elements", and they are essential to building web pages of any kind.

## Objectives

1. Assess HTML document structure
2. Explain the Depth (Integer) of an HTML Tag Node Within the Document
3. Identify Invalid Nesting

## Assess HTML Document Structure

Nesting is a fundamental feature of the HTML document. Take a look at the following
example of a well-structured HTML document:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Web development course</title>
  </head>
  <body>
    <header>
    <!-- header element documentation: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/header -->

      <nav id="main-navigation">
      <!-- nav element documentation: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav -->

        <ul>
        <!-- ul element documentation: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul -->

          <li><a href="/web">Introduction to the web</a></li>
          <!-- li element documentation: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/li -->

          <li><a href="/html">Learn HTML</a></li>
        </ul>
      </nav>
    </header>
  </body>
</html>
```
It's easy to see the document structure with the inner tags indented. 
However, note that nested elements may not always be placed on separate,
indented lines. 
**I like this note**

## Explain the Depth (Integer) of an HTML Tag Node Within the Document

The topmost tree nodes in the HTML document structure are `<html>`, `<body>`, and `<head>`.
Understanding HTML nesting allows us to be able to manipulate HTML elements and their contents.
Child nodes are elements that are direct children of a given node. In other words, they are
nested exactly in its parent. For example, `<head>` and `<body>` are children of `<html>` element.
Descendants are _all_ elements that are nested in the parent node. For example, `<header>`,
`<nav>`, and `<ul>`, `<li>` are all children of `<body>` or `<html>` element. Why is this important?
This will be more valuable as we start to apply styles or perform operations on the DOM. Both start
with the document object and from it we can access or reference any node.
**This whole paragraph feels a bit dense. It's a lot of vocab in a very small space (tree nodes, child nodes, nested, descendents), that we feel pretty comfortable with as developers, but might be really scary with to newbies. I think it just need a little explanation that elements can also be referred to as nodes, since it's not specified before this.**

## Identify Invalid Nesting

When tags are nested, it is important that they are closed in the opposite order
that they were opened. Valid HTML allows for accessibility and browser compatibility.
If your HTML is incorrectly nested, it won't be as accessible to screen readers and
older browsers. It could can also break the visual appearance of a page if the
browsers cannot render the page properly because HTML elements and tags are unclosed
or out of place.

```html
<li><a href="/html">Learn HTML</li>
```

In the example above, the `<a>` tag is unclosed. This may cause the rest of the document
following this element to inherit the properties of this link.

```html
<li><a href="/html">Learn HTML</li></a>
```

The above HTML is also invalid, and may cause unpredictable behavior in the page.
It can be challenging to keep track of where content begins and ends. Keeping your
HTML well indented so that every tag and "level" of nesting is aligned will make
your code easier to read and maintain. It also helps us keep to separate content
and keep blocks of information organized.

## Conclusion

We use nesting to keep the elements of our HTML document organized into containers
of content. With valid and well-written HTML, we can construct a solid page structure
that serves as a foundation for anything else we want to build.

## Resources

* [Nested Tags](http://www.bu.edu/tech/services/cccs/websites/www/non-wordpress/start/html-introduction/syntax/nesting-tags/) More on Nested
* [Tags](https://www.thoughtco.com/nesting-html-tags-3466475) More on Nesting...
* [Best Practices Web Design](http://www.iraqtimeline.com/maxdesign/basicdesign/principles/prinnest.html)

