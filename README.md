# Retro-Encabulator

#### A webpage promoting the Retro-Encabulator, November 17, 2017

#### By **Luke Bertram**

## Description

This is a webpage promoting the groundbreaking Retro Encabulator product now available from Rockwell Automation. Primarily, it is an exercise in styling a webpage using such CSS as floats, pseudo-classes, pseudo-elements, table styling and relative/absolute positioning.

## Setup/Installation Requirements

For greatest ease of use, simply visit [this website](http://lukebertram.github.io/encabulator) in your web browser of choice. However, if you're feeling frisky, you can also use the following steps to clone the project from [GitHub](http://github.com) and run it locally on your own computer:

 * Visit the github page for [this project](http://github.com/lukebertram/encabulator)
 * Click the "Clone or Download" button and copy the address found there. Alternatively, just copy this address to your clipboard: https://github.com/lukebertram/encabulator.git
 * Access your system's command line interface (_ie Terminal, for MacOS Users_) and navigate to your home directory by entering the following magical spell into your command line (note: do not enter the '$' character):
 >$cd ~

 * Next, cast the following, more advanced spell:  
 >$git clone https://github.com/lukebertram/encabulator.git

 * Finally, open the project in your system's default web browser with the following final incantation:
 >$open encabulator/index.html


## Known Bugs

No known bugs as yet.

## Support and contact details

Flag me down in class, or send me a tweetbook on facestagram if you have any troubles.

## Elements Used

This project was completed using only HTML and CSS. The specific CSS elements used are as follows:  

|Term     | Description | Implementation|
|:--------|-------------|--------------:|
|border-box| A value for the 'box-sizing' property that prevents an element's padding and margin values from adding to its total width.| This property value was applied to every element on the page by default by using the * (all) selector at the top of the stylesheet. |
|float| Removes an element from the normal flow of the document, causing it to 'float' either to the left or right depending on the value set.| Both the logo and the navigation links in the page's header are floated - the former to the left and the latter to the right.|
|display: block|Overrides an element's default display style, causing it to display as though it were a block element. By default, block elements take up the full width available and break to their own new line. |Although not explicitly defined, the default display value of every div I used in this web page is 'block'.|
|display: inline|Overrides an element's default display style, causing it to display as though it were an inline element. By default, inline elements take up only as much horizontal space as needed and do not break to a new line. |I applied display: inline to the unordered list items in the navigation portion of my header. Normally, list items behave like block elements in that each one breaks to a new line. Displaying them inline allows them to sit nicely next to each other, all vertically centered within the header. |
|centered content|Content that is either vertically or horizontally positioned in the center of its parent container.| I had initially centered the hero image using absolute positioning combined with a translation transformation. However, after adding the absolutely positioned caption to the hero, I felt the page would be more balanced if I nudged that image just up and left of its previously exactly centered position. The nav links are vertically centered within the header.|
|pseudo-element|An element that is declared in CSS styling rather than directly in the page's markup. ::after and ::before pseudo-element selectors can add content around an element that was not there in the html.|I used a pseudo-element selector to implement a clearfix in the ::after pseudo-element of the .two-col div containing the product description and image gallery. |
|pseudo-class| |The navigation links are styled using the 'hover' and 'active' pseudo-classes. When moused-over or clicked, the links will shift to a brighter color with a sharper drop-shadow. |
|clear-fix|A means of dealing with troublesome float behavior (such as a collapsing parent container), a clearfix is an invisible element set to clear preceding floated elements. | I implemented a clearfix in the ::after pseudo-element of the .two-col div containing the product description and image gallery.|
|Positional selector| A positional selector (such as ":nth-child") allows for the selection of an element based on its position in the order of a group of sibling elements. This can be as simple as selecting a first, second, last, etc child from a group of sibling elements. It can also use maths to select more complicated groups of elements (like every fifth element in a group).| I used a li:not(:last-of-type) positional selector to select each of my list item elements except the last one to have a right-side border bar to separate it from the other navigation links.|
|Selector combinator|These allow you to combine multiple selectors. The '.' used at the beginning of class selectors is technically a combinator, as is the ':' at the beginning of pseudo-classes.| I used a direct child combinator (.hero > h1) to select the h1 that is a direct child of an element of the .hero class. This will select only h1 elements that are direct children of an element with the .hero class.|



### License

MIT License

Copyright (c) 2017 **Luke Bertram**
