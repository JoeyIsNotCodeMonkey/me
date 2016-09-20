---
layout: post
title:  "Responsive Theme Design for The Website of CS Department in SBU"
date:   2016-09-19 23:24:22
description: A Web Application
categories:
- project
---

This documentation briefly records what I did to turn the compsci theme into responsive version.

The sites remains exactly same as before when the screen size is larger than 960px, while the layout starts to change when the size reach 960px. All the changes I made on the theme mainly rely on the important media tag (@media only screen and (max-width: 960px) {...}).
	
### Front page
	The most complicated part of this project is the front page of the site. The the width main container used to be a fixed size 960px. I set it to be 100% when the screen width is less than 960. This is the first step to make the content fluid with change of the screen size. 
	
	Since the main container breaks into “header”, “navWrap”, “container” and “footer”, and all of them were set to fixed size of 960px, I had to reset their width to 100%. 

### Responsive Menu
	I tried to use module to achieve responsive effect since it should be more simple and easy to be managed, while the result proved that I was so wrong. The responsive menu seems does not work with Zen theme (I also saw the complaining of the issue on google but no decent solution yet). So instead, I made a responsive menu by css manually and it works perfectly. The css file is called “responsive-menu.css”, check out to see more in detail. 

### Responsive header
	The header is divided by logo container, banner and search box.
	Logo container: I made the logo float to none and everything align center when it is small screen size. [logo_container.css]
	Banner: Since I made all the images {max-width: 100%, height: auto}, so the banner is also responsive now.
	Search box: Click the button on the up-right corner to display the search box. The old “searchblack.css” is no more used. [search_responsive.css]

### Container
	Main content container has three column on the top, which are “Spotlight”, “News&Events” and “Video”. There are four cards below the three column section. When the screen size is less than 960px, each column of the three column becomes full width, and four cards takes two column. When the width is smaller than 640px, four cards line in one column.[front.css]

### Basic page
	When screen size is less than 960, the side bar will be hided and main content become full width. See “basicpage.css” for more detail.

### UI Changes
Faculty page: [faculty.css]
	added a “faculty profile” class for faculty personal page.
added a “faculty-intro” class for the region next to faculty pic.

About us > Photo Gallery: [photo-gallery.css]
	added a “photo-gallery” class (to the view) on about us > photo gallery page and also for the next level page. Besides, change the format of the view from “Grid” to “unformat list”

Faculty-only page: [faculty-only.css]
	Change all the tables to 100% width.

	
### Theme changes
Add the following lines of code to the html.tpl.php file so that the responsive site is viewable as responsive on a mobile device. These lines are added where metatag is or under the head title

~~~ html
 <!-- meta tag insert for mobile devices-->
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <!-- End Insert -->
~~~

Click [here](https://www.cs.stonybrook.edu/) to go to the website. 





