# Nested HTML Tags And Attributes

## Problem Statement

When you take a look at an entire HTML document, it's sometimes challenging to
keep track of where tags begin and end. But understanding more about HTML tag
nesting and attributes can help everything fall into place.

## Objectives

1. Assess HTML document structure

## Assess HTML Document Structure
Whenever we nest an HTML tag inside of another tag, we indent the inner tag so
that the overall tag hierarchy is clear. Take a look at the following example of
a well-structured HTML document.

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

Keeping your HTML well indented so that every tag and "level" of nesting is
aligned will make your code easier to read and maintain. It also helps us keep
to separate content and keep blocks of information organized. 

**NOTE:** Nested tags may not always appear on separate, individual indented lines. 
Nested tags can appear in a single line, with opening and closing tags inside
of another opened tag that represents the nested elements in HTML.

## Conclusion

We use nesting to keep the elements of our HTML document organized, and we use
attributes to give our elements more power. With these strategies, we can
construct a solid HTML structure that serves as a foundation for anything else
we want to build.

## Resources

* [Nested Tags](http://www.bu.edu/tech/services/cccs/websites/www/non-wordpress/start/html-introduction/syntax/nesting-tags/) More on Nested
* [Tags](https://www.thoughtco.com/nesting-html-tags-3466475) More on Nesting...
* [Best Practices Web Design](http://www.iraqtimeline.com/maxdesign/basicdesign/principles/prinnest.html)

