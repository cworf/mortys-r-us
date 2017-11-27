
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

## Technologies used

HTML
CSS

## Copyright

Creative Commons
