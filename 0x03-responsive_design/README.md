Whatever the browser you use, it’s a good idea from now on, to toggle the device view.

In a normal situation, you should start with “mobile first” in mind and write your CSS first for the mobile. But because we already have a desktop version, we will exceptionally add some media-queries for mobile and tablet.

For extra large devices (no media queries)
For desktop / large devices (max-width: 992px)
For tablet / medium styles (max-width: 767px)
For mobile styles (max-width: 480px)
We will put media queries at the end of each section to facilitate the reading but for performance reasons, the best practice is to unifiy all similar breakpoints at the end of the CSS file.

In your 02-1-styles.css file:

inside the /* Helpers section target all images inside the main section

Property: width, Value: 100%
Property: height, Value: auto
inside the /* Section Latest news section, add a new media query (max-width: 767px)

Target the row inside section-latest-news
Property: flex-direction, Value: column
inside the /* Grid section, at the end, add a new media query (max-width: 767px)

First, redefine the variable section-padding and give that value: 5rem 1.5rem. And redefine the variable section-body-padding with 2rem 0 0
Target the ul.row and the row class
Property: flex-direction, Value: column
Property: margin, Value: 0
Target all the classes that started with col-
Property: margin, Value: 0 0 3rem 0
Target the col-1-3 and col-1-2 classes
Property: width, Value: 100%
The navbar is not allowing the website to fit the window. We will temporarily hide it and create a mobile navbar later.

inside the /* Navbar section, at the end, add a new media query (max-width: 767px)
Target the navbar-menu class
Property: display, Value: none
You should now be able to easily view the website on a device of any screen/window size. I guess you are surprised that was so easy?!

Rendering on wide screen