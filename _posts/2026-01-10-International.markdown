---
title: "International charts - v3.20"
date: "2026-01-10 12:00:00 -0800"
categories: release 
og_image: /assets/images/og_image.png
---


### International Charts

Nautical chart imagery has been added for Canada, Australia, New Zealand, and Norway. 

Each country, and sometimes different regions within each country may use different datums for
establishing the zero reference point for depth measurements.  For example, coastal USA depths are measured relative to mean lower low water (MLLW) in feet.  

Charts for almost all of the rest of the world use metric units.

Coastal Canadian waters measure depths relative lower low water, large tide (LLWLT), while depths in the Great Lakes are referenced to International Great Lakes Datum (IGLD).

Definitions:  <a href="https://en.wikipedia.org/wiki/Chart_datum" target="_blank"> Chart datums</a>

When DeepZoom displays chart areas with differing units, the units are shown as **mixed**, as below.

<img src="/assets/images/mixed.png"  style="box-shadow: 4px 4px 4px 0px rgb(128,128,128); margin-top: 12px; margin-bottom: 12px "   width="60%" />{: .border .align-center .toc}


### USA Tides and currents refresh 

All of the USA tides and currents are now updated to the latest NOAA December 2025 data release.
Tide and current data is available between the dates of 2020.01.01 through 2040.12.31 inclusive.

<img src="/assets/images/chesapeake-currents.png"  style="box-shadow: 4px 4px 4px 0px rgb(128,128,128); margin-top: 12px; margin-bottom: 12px "   width="60%" />{: .border .align-center .toc}


Thanks, as always to David Flater  [(xtide)](https://flaterco.com/xtide/files.html) for collecting and publishing the .tcd files which I use to generate the the millions of 
tide fragment files which enables DeepZoom's rapid display. 


### International tide stations, NOT!

I attempted to add International tides using TICON-4 harmonics, but gave up when the results seemed close, but not close enough. See: [(Github: deepzoom-ticon4)](https://github.com/jaybo/deepzoom-ticon4).  Just figuring out which of the differing online tidal websites was authoritative is the first hurdle.  Then there is a dearth of information regarding datum and active time zone.  So verification proved challenging.

If you feel like hacking away at the TICON-4 code, I'd be delighted to help!
{: .notice--warning}


### Magnetic Variation update 

DeepZoom optionally displays the magnetic heading for each leg of a route (see the Settings page).  The model used to compute this value has been updated to the World Magnetic Model 2025-2030. [(NOAA)](https://www.ncei.noaa.gov/products/world-magnetic-model)


### Serenade is for sale 

<img src="/assets/images/Serenade4.jpg" style="box-shadow: 4px 4px 4px 0px color:rgb(128,128,128); margin-top: 12px; margin-bottom: 12px" width="100%" />{: .shadow .align-left .toc}

<img src="/assets/images/Serenade2.jpg" style="box-shadow: 4px 4px 4px 0px color:rgb(128,128,128); margin-top: 12px; margin-bottom: 12px" width="100%" />{: .shadow .align-left .toc}

<img src="/assets/images/Serenade1.jpg" style="box-shadow: 4px 4px 4px 0px color:rgb(128,128,128); margin-top: 12px; margin-bottom: 12px" width="100%" />{: .shadow .align-left .toc}


It is with great sadness that we've decided to put Serenade up for sale.  Serenade is a 1997 40' Pacific Seacraft cutter designed by Bill Crealock.  We have been through many adventures together over the last 25 years and I can vouch that Serenade is a sturdy and stalwart companion, a beautiful and safe haven in any and every storm.  

While cruising last summer north of Vancouver Island, ML took a tumble while hiking (she claims forest trolls pushed her) and has had a two surgeries to fix a badly broken elbow. And I have a shoulder which is unraveling a few decades after a serious motorcycle accident, so it's time to introduce Serenade to new traveling companions.


Full listing is at [https://www.yachtworld.com/yacht/1997-pacific-seacraft-40-10013258/](https://www.yachtworld.com/yacht/1997-pacific-seacraft-40-10013258/)