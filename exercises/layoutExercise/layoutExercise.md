|  Introduction to Interactive Media (IGME-110), Fall 2019 | [Syllabus](https://lawleyfall2019.github.io/110-fall2019/) | [Schedule](https://lawleyfall2019.github.io/110-fall2019/schedule.html#week8) |
|----|----|----|


# CSS Layout Exercise/Homework (Week 8, Thursday 10/17)

Today's exercise is to use CSS Flexbox and CSS Grid to replicate the "Holy Grail" layout.

![holygrail.png]("Holy grail layout image")

(If you're having a hard time with flex and grid concepts, and you haven't already played the [Flexbox Froggy](https://flexboxfroggy.com/) and [CSS Grid Garden](https://cssgridgarden.com) games, I suggest doing that before you start on your own grid.)

## Part 1: Holy Grail Layout Implementation

Wikipedia's description of the Holy Grail layout problem:

>Many web pages require a layout with multiple (often three) columns, with the main page content in one column (often the center), and supplementary content such as menus and advertisements in the other columns (sidebars). These columns commonly require separate backgrounds, with borders between them, and should appear to be the same height no matter which column has the tallest content. A common requirement is that the sidebars have a fixed width, with the center column adjusting in size to fill the window (fluid or liquid layout). Another common requirement is that, when a page does not contain enough content to fill the screen, the footer should drop to the bottom of the browser window instead of leaving blank space underneath.

This was very difficult to accomplish before Grid and Flexbox, but it's relatively simple to do now. 

Here are the requirements in list form:
- Entire grid centered on the page using a flexbox wrapper div
- Grid takes up full viewport height (can use height or min-height)
- Three columns and three rows
- Left and right column fixed width
- Center column fills remaining space
- Top and bottom rows fixed height, span all three columns
- Middle row fills remaining space

You may find it easier to do this if you use different background colors for each of your content elements, and/or turn on borders for everything while you're working.   

(There are a lot of solutions out there on the web, but if you use those you won't learn as much :) 

## Part 2: Your Preliminary Web Project Grid

Once you've finished the holy grail layout, you should have a good sense of how to create a grid-based page. Use that knowledge to create an HTML/CSS grid for your planned website. 

Your grid should have a minimum of two rows and two columns. It should be constrained in width, using either pixels or %, and should also be centered on the page using a flex-based wrapper. 

 
## Deliverables

You do not need to turn in the Holy Grail pages. For your preliminary web project grid, put the HTML and CSS files (and any associated images) into a folder, zip the folder, and submit it to the dropbox in myCourses. 