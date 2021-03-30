# Links in HTML

Links are created using the ***< a >*** then using the **href** attribute to specify which page to link
  ***< a href="link">link text< /a >***

Email Links created using the ***< a >*** then using the **href** attribute that starts with **mailto** to specify the email address to link
  ***< a href="mailto:email address">email name< /a >***

**Opening links in a new window**

by using the target attribute on the opening ***< a >*** tag with be _blank value

**Linking to a specific part of the same page**

To add a list of contents at the top of a long page that links to the corresponding sections, or to add a link from the bottom to the top of the page. By identify the points in the page that the link will go to by using the **id attribute** and the href attribute should starts with ***#***


# Layout

CSS treats each HTML element as if it were in its own box. This box will be either:
* **Block-level box** start on a new line and act as the main building blocks of any layout ***< h1 > < p > < ul > < li >*** ...etc
* **Inline box** flow between surrounding text ***< img > < b > < i >*** ...etc

**Containing element:** is the outer box of block-level element that contains another block-level element inside 


### Positioning Schemes

* **Normal Flow** (***position:static***) the default way where each block-level element sits on top of the next one
* **Relative Positioning** (***position:relative***) moves an element in relation to where it would have been in normal flow
* **Absolute Positioning** (***position:absolute***) the element box is taken out of normal flow and no longer affects the position of other elements on the page

**Fixed Positioning** (***position:fixed***) type of absolute positioning that positions the element in relation to the browser window not another elements and stays in the exact same place when scrolling the page

***z-index*** property used to control which element sits on top elements overlapping, the higher the value number the closer that element is to the front

***float property*** allows to take an element in normal flow and place it as far to the left or right of the containing element, then the width property should also be used to indicate how wide the floated element should be


### Screen and Page Sizes

**Screen Resolution:** the number of dots a screen shows per inch

Because screen sizes and display resolutions vary so much, web designers often try to create pages of around **960-1000** pixels wide (since most users will be able to see designs this wide on their screens).

Designers assumed that users would see the top **570- 600** pixels of a page without having to scroll and some tried to fit all of the key messages in this area, as well as hint at more content below this point


### Fixed Width Layouts
By using fixed pixel sizes

**Advantages**

* Pixel values are accurate at controlling size and positioning of elements
* The designer has far greater control over the appearance and position of items on the page
* lengths of lines of text can be controlled regardless of the size of the user's window
* The size of an image will always remain the same relative to the rest of the page

**Disadvantages**

* Boxes can end up with big gaps around the edge of a page
* The page can look smaller and text can be harder to read if the user's screen is higher in resolution 
* If a user increases font sizes, text might not fit into the allotted spaces
* The design works best on devices that have a site or resolution similar to that of desktop or laptop computers


### Liquid Layouts
By using percentage sizes

**Advantages**

* Pages expand to fill the entire browser window so there are no spaces around the page on a large screen
* If the user has a small window, the page can contract to fit it without the user having to scroll to the side
* The design is tolerant of users setting font sizes larger than the designer intended

**Disadvantages**

* The design can look very different than designer intended, with unexpected gaps around certain elements
* If the user has a very narrow window, words may be squashed and can end up with few words on each line.
* If a fixed width item is in a box that is too small to hold it, the item can overflow over the text.


### Layout grids

**Composition:** the placement or arrangement of visual elements — how they are organized on a page

**Advantages of using grids:**

* Creates a continuity between different pages which may use different designs
* Helps users predict where to find information on various pages
* Makes it easier to add new content to the site in a consistent way
* Helps people collaborate on the design of a site in a consistent way


### CSS Frameworks
Libraries of code that contain common tasks, such as creating layout grids, styling forms ...etc

**Advantages**

* They save coder from repeatedly writing code for the same tasks
* They will have been tested across different browser versions (which helps avoid browser bugs)

**Disadvantages**

* They often require use class names in HTML code that only control the presentation of the page
* They often contain more code than coder need for particular web page in order to satisfy a wide variety of needs

**960.gs CSS Framework:** A website provides a style sheet that can included in HTML page, also provides templates that can downloaded to help design the pages using 12 or 16 column grid


### Multiple Style Sheets

Some web page authors split up their CSS style rules into separate style sheets. For example, they might use one style sheet to control the layout and another to control fonts, colors and so on


# Functions & Methods

**Functions** consist of a series of statements that have been grouped together because they perform a specific task

**Methods** are the same as functions, except methods are created inside (and are part of) an object

