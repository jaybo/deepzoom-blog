---
title: "DeepZoom 2.2.17 Tide selection annoyance"
date: "2022-02-01 15:41:20 -0800"
categories: trip
lastmod: "2022-01-17T20:41:08.342Z"
og_image: /assets/images/save-trip.png
---

### Oops, I broke backwards compatibility 

V2.2.17 uses a slightly modified trip storage format.  If you have a tide  or current station selected in your old file, it will not be auto selected in a newer version of DeepZoom. Sorry, but this is a one time upgrade and it wasn't trivial to maintain backwards compatibility. 

To fix this problem, open the trip in DeepZoom. Select the station again, and then resave the trip. <br/> Make sure **Include view settings** is *Yes*.
{: .notice--warning}

![save a trip](/assets/images/save-trip.png){: .align-center}

If you're one of the adventurous few who is actually writing a scripted trip, then you'll need to manually update the **tideOrCurrent** entries within the script.