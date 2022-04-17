---
title: "DeepZoom 2.3.23 Trip editing improvements"
date: "2022-04-16 12:00:00 -0800"
categories: release
lastmod: "2022-01-17T20:41:08.342Z"
og_image: /assets/images/snipVertex.png
---

### New features

![](/assets/images/snipVertex.png){: .align-center}

1. Many improvements to route editing.  Of particular note is the ability to split routes using the snip tool (scissors icon in the above image).
2. Added the ability to attach scripts to Markers.  At present, this means script actions can be triggered at any of the following times.
- When a trip is loaded.
- At a relative point along a trip.
- *New*: **Marker Arrival scripts** execute when in Play mode and the map center is within 1 nMi of the Marker location.  
- *New*: **Marker Departure scripts** execute when in Play mode and the map center moves 1 nMi away from the Marker location.  
In the future, the trigger distance will be programmable.
3. Routes and Markers have a separate button to edit the name.  Editing the name in place was a continuing nightmare so I went with this simpler alternative.

### Bug fixes
2. Markers can now be deleted.


### Up Next
From the outset of DeepZoom V2, I've been contemplating whether to add user generated rich content (text, images, video) to Markers.

There are plenty of websites which attach commercial content to map markers showing marinas, gas prices, and the like, but I've been imagining something closes to a mashup of Twitter and Wikipedia, where you can add comments on anchorages, dive spots, fishing holes, kayaking campgrounds, etc. along with images, videos, and ratings or likes/dislikes.

But entering this arena means higher operating costs and the more serious problem of moderating user submissions.

If you have any ideas or suggestions on this topic, I'd love to hear them.

[https://github.com/jaybo/deepzoom-blog/discussions/3](https://github.com/jaybo/deepzoom-blog/discussions/3)