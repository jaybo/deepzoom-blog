---
title: Rich Media - v2.7
date: 2022-09-25 15:41:20 -0800
categories: release trip
lastmod: 2022-09-25T20:44:01.227Z
og_image: /assets/images/rich-media-langley.png
draft: true
---
## Rich Media
I'm a daily user of Wikipedia and Twitter.  And 
I've long imagined adapting the spirit of these innovations into DeepZoom, creating an authoritative information source for trips and markers (the Wikipedia part) along with user contributions including comments, images, videos, and ratings (the Twitter part).

This release marks the introduction of both of these features.

![](/assets/images/rich-media-langley.png){: .align-center .toc} 

To some extent, these features overlap those offered by [https://activecaptain.com](https://activecaptain.com) and [https://marinas.com](https://marinas.com).  Since I don't have the bandwidth/time/money to keep track of all of the details for every commercial establishment, DeepZoom will just provide a link to the authoritative source at the top of each marker description.

But what is unique here is that each marker and trip can optionally include a series of comments with images and video.  The user interaction model is similar to Twitter, and you can comment on others comments.

Anyone who has tried to spelunk through Amazon product reviews for valid information knows that the tragedy of the commons applies to the internet.  Mindless and irrelevant comments and reviews seem to be the norm, and bots are rapidly taking over.
To try and limit such flotsam and jetsam on DeepZoom, only subscribers can post new content or add ratings.

There are two classes of markers:  **public** markers appear on everyone's chart, and **private** markers are only stored within a Trip. The next planned feature will allow users to promote their private markers into the public arena.  For example, if you have a collection of Puget Sound SCUBA sites with accompanying rich media you'll be able to have these show up on everyone's chart.  Just mark the Trip containing the markers as **public** and if the trip garners a high enough star ranking and votes (number to be determined) the markers will become automagically become public.  To be eligible to transition to public marker status, the Trip must *only* contain markers and no routes.

### The content editor

The editor is divided into three sections: text, images, videos.  Each section is optional.  
Both images and videos can be drag and dropped onto the editing page. Images retain their full original resolution. At this time, videos must be hosted on YouTube. 


![](/assets/images/LangleyEdit.png){: .align-center .toc} 


### Seattle to Lopez Island Loop

This trip has been updated to demonstrate adding rich media at each port of call.

Try it: [  https://www.deepzoom.com/trip/yzp5ybrk ]( https://www.deepzoom.com/trip/yzp5ybrk)
{: .notice--warning}


### Seattle To Glacier Bay via Inside Passage

This trip has been updated to demonstrate adding rich media to the trip itself.
Scroll down on the "Trip" tab to see comments and images.

Try it: [https://www.deepzoom.com/trip/4jvmcnf6](https://www.deepzoom.com/trip/4jvmcnf6)
{: .notice--warning}

### Bug fixes

1. Sometimes when changing properties of a route another route would be incorrectly selected.  Sorry for all the aggravation this bug has caused, but it is now fixed!
2. The "Kingman - Cuttyhunk" Trip could hang the app.  Fixed.
