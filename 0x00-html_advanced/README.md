HTML - elements of a web page
Create the foundation of any HTML page.

HTML is about content. CSS is about the look and feel.

Doctype
The <doctype> is necessary at the top of every HTML page to force the browser to render the page according to relevant specifications.

<!-- Doctype HTML5 -->
<!DOCTYPE html>
<!-- Lowercase is also valid -->
<!doctype html>
Resources
Doctype - MDN Web Docs Glossary: Definitions of Web-related terms | MDN
HEAD - A free guide to head elements
HTML tag
The <html> HTML tag tells the browser that the document is an HTML webpage. It is used as a container for all the HTML elements.

Warning!

The doctype is the only element living outside the html tag.

<html lang="fr" dir="ltr">
Language and reading direction
Building RTL-Aware Web Apps & Websites: Part 1 - Mozilla Hacks - the Web developer blog
head tag
The head tag element contains all the metadatas related to your page. All the elements put in the head are not visible in the window of the browser.

A lot of metadatas exist, some specific to some CMS.

Usage
You can find inside the head:

title of the webpage
asynchronous script calls
metadata
CSS code embed (critical CSS)
JavaScript code embed
Resources
HEAD - A free guide to head elements
Meta charset
The meta charset declares the page’s character encoding.

...
<head>
    <!-- Set character encoding for the document -->
    <meta charset="value">
</head>
...
Resources
meta: The Document-level Metadata element - HTML: Hypertext Markup Language | MDN
Declaring character encodings in HTML
Meta Charset
Viewport
The meta viewport gives information about the initial size of the viewport.

Tip: The viewport is used by mobile devices only.

Accessibility tip: Never use maximum-scale=1.0. It prevents the user from zooming in on the website. It causes an accessibility issue.

...
<head>
    ...
    <!-- Viewport for responsive web design -->
    <meta name="viewport" content="key=value, key=value">
</head>
...
Resources
Responsive Design With Viewport Control
Title
The title meta tag defines the title of the web page.

Tip: The title is only visible on the tab/window of your browser.

Warning! The title should always have less than 56 characters.

...
  <head>
    ...
    <!-- Document Title -->
    <title>Page title</title>
  </head>
...
Resources
The ideal width of the SEO title • Yoast
Meta description
<head>
    ...
    <!-- Meta Description -->
    <meta name="description" content="Description of the page less than 150 characters">
  </head>
Resources
The ideal length of a meta description • Yoast
Favicons
<head>
    ...
    <!-- Standard favicon -->
    <link rel="icon" type="image/x-icon" href="https://example.com/favicon.ico">
    <!-- Recommended favicon format -->
    <link rel="icon" type="image/png" href="https://example.com/favicon.png">
    ...
  </head>
Resources
Favicon & App Icon Generator
Favicon Generator for all platforms: iOS, Android, PC/Mac…
Obsessive cheat sheet to favicon sizes/types.)
Favicons, Touch Icons, Tile Icons, etc. Which Do You Need? | CSS-Tricks
PNG favicons - caniuse
Tag attributes
Attributes provide additional information or instruction for an HTML element. It is always included inside the opening tag.

Data-* attribute
It is possible to declare any attribute using the data- prefix

<tag data-extra-attr="value">some content</tag>
Resources
HTML attribute reference - HTML: Hypertext Markup Language | MDN
header tag
The <header> HTML tag element is used to identify the top of a webpage, article, section, or other segment of a page. The header is normally always the same across all pages of your website.



Usage
logo of the website
navigation
search form
...
<body>
    <header>This is my header<header/>
</body>
Warning! The main element should never be a descendant of an article, aside, header, footer, or nav element.

Don’t confuse header with the head element of the page.

Resources
header - HTML: Hypertext Markup Language | MDN
