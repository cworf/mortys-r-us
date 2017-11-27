
### CSS Week 1 Code Review - Epicodus

# Morty's-R-Us

### Author: Colin Worf

## Description

This is a single page website which uses floats to accomplish the basic layout. I added some various hover effects and built

## Instructions

1. Clone project ```$ git clone https://github.com/cworf/mortys-r-us.git ```
2. enter project by opening the repository and selecting index.html
3. view final project online by visiting https://cworf.github.io/mortys-r-us/

## Specifications
### (in order of first use)
|Term|Description|Implementation|
|----|-----------|--------------|
|box-sizing|the box-sizing property tells the browser how to handle sizing on a particular element. should the total size of the element include just the content? or the padding and border?| I used box-sizing:border-box on all div's as well as all labels, basically anything that is floated or flexed, so that when using precise percentages for thirds (33.3333%) or half's(50%) or fifths (20%) I did not need to worry about the padding or border causing unwanted sizing changes|
|Float|Float takes elements out of the document flow and into their own separate flow, only bound by other content on the page, the element floats upward until it hits a block element which takes up more than 100% - the floated element's width, or it hits the top of its parent, then floats in the direction specified|I used floats to construct the base structure of the page, fifths, halfs, and thirds. (I later changed certain elements to flexboxes instead of floats to achieve a better looking design)|
|display|the display property is used to change an element from its default box type| <ul><li>I used display:block on the "other ricks lost these morties" section so that I could treat the links as block elements with multiple child elements within, I also used it on the price tag so that I could give it a specific width of 80% and center it with margin:auto.</li><li>I used display:inline-block on nav links so that I could treat them as block elements but they would also stack left to right.</li><li>I used display:flex on a couple elements to achieve my design priorities without having to change default overflow settings and to achieve equal height on all elements within a row</li></ul>|
|Margin|Margin specifies outside-the-box spacing for a block element this space is not included in any box sizing options|I used margin:auto; to center block elements that have a specific width, such as the main container as well as the price tag, otherwise margin is used frequently throughout the page to provide spacing between elements|
|text-align|Text align is used to specify which side of the parent container the text should be aligned with, or if it should be centered|I used text-align:center on all .box elements so that all text within them was centered no matter what type of element was being used, I also used center on the H2 tag (title of the product)|
|Pseudo-elements|each element has specific parts within it called pseudo-elements these can be styled differently depending on which element is selected|I used the :after pseudo element on the .other-images class (grid of 6 small images in two columns) as a clear-fix for the floated elements, I also used the :before element on the price tag to create both the pointed black line, as well as to place the flurbo symbol. Finally, I used it to display a large quotation mark in the "favorite quote" section.|
|pseudo-classes|pseudo classes are used to style an element based on its specific state or location within the its parent|I used :checked to visually specify which tab is currently selected in the product description area, I used :nth-child(3n) to remove the margin-right on the last tab button in each row so they would align perfectly to the right of the container, I used :hover to create special styling when the user hovers their mouse over elements such as buttons, table rows, each image within the image grid, and the links within the "other products" section.|
|Clear-Fix|Clear Fixes are used to define new rows within floating elements as well as to force parent elements to wrap around their floating elements.|I used the pseudo-class clear-fix on the 6 image grid of thumbnails to force its parent to wrap around them so the two buttons underneath the box would align properly|
|positional selector|these are pseudo-classes used to select elements in specific positions within their parent|I used :nth-child(3n) to remove the margin-right on the last tab button in each row so they would align perfectly to the right of the container|
|Selector Combinator|There are 4 selector combinators "~", "+", ">", " ", they are used to specify elements relative to each-other within the html document|<ul><li>I used all 4 of these elements heavily, mostly the space combinator which is used to select all descended child elements of a specific type within the specified parent</li><li>I used the ">" combinator to select only the dierct child divs inside the .container class to place a margin-bottom on all except for the last child</li><li> I used the + combinator to accomplish the hover and checked effects on the labels of the radio buttons (6 tabs) as well as the hover effect of the main logo link in the nav-bar </li><li>I used the ~ combinator to accomplish the hover effects on the 6 small image grid to activate the hidden larger image containers for each upon hover of the correct sibling</li></ul>|

## Technologies used

HTML
CSS

## Copyright

Creative Commons
