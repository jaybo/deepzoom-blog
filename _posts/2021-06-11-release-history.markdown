---
title: DeepZoom Release History
date: 2021-06-11 15:41:20 -0800
categories: release 
lastmod: 2021-06-11T20:44:01.227Z
og_image: /assets/images/WeatherHUD.png
draft: false
---


<div style="background-color: lightblue; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.14.0
</span>  
<span style="float: right; margin: 6px;"  >
2024.03.14
</span>
<hr style="clear: both"/> 
</div>

#### New features
- Updated NOAA charts.  All NOAA chart depths are now in feet.
- Updated NOAA tides and currents data to January 2024 release.
- New route and marker creation and editing dialog.
- New dialog to publish a private marker collection onto the public map.
- Tracks are now timeline aware
- Routes can be disabled.  This is useful for boundary marking.
- Marker star ratings are now displayed on the map.
- Many improvements in editing routes and markers, both touch and mouse.
- Many UI improvements throughout.


#### Bugs fixed
- Many



<div style="background-color: lightblue; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.1.4
</span>  
<span style="float: right; margin: 6px;"  >
2023.05.16
</span>
<hr style="clear: both"/> 
</div>


#### Bugs fixed
- Sometimes tides and currents would not get updated without initially moving the chart.
- A big deal! **Instantaneously update time when changing route departure date/time or speed.**  This feature was present on many early versions of DeepZoom but was problematic because routes were sometimes autoselected in a confusing fashion. I think this is finally fixed, enjoy!










<div style="background-color: lightblue; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.0.99
</span>  
<span style="float: right; margin: 6px;"  >
2023.05.08
</span>
<hr style="clear: both"/> 
</div>


#### Bugs fixed
- the **Now!** button would sometimes switch the time zone display to UTC.
- +/- day or week increment buttons under the tide graph were not working correctly.
- Verification email confirmation was sometimes silently ignored.




<div style="background-color: lightblue; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.0.89
</span>  
<span style="float: right; margin: 6px;"  >
2023.04.28
</span>
<hr style="clear: both"/> 
</div>


#### Bugs fixed
- Never change map center when selecting a route.
- Propogate route name changes onto time slider.
- Update browserlist to handle 89% of all browsers.
- Make changing timebase settings rational.





<div style="background-color: lightblue; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.0.75
</span>  
<span style="float: right; margin: 6px;"  >
2023.04.01
</span>
<hr style="clear: both"/> 
</div>

#### New features
- When used in iFrame, each instance of DeepZoom uses a unique localstorage.

#### Bugs fixed
- Position marker correctly at start or end of route when using Timewarp.
- fix getLayer() error at startup on some devices.




<div style="background-color: lightblue; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.0.51
</span>  
<span style="float: right; margin: 6px;"  >
2023.03.08
</span>
<hr style="clear: both"/> 
</div>

#### New features
- Added 3 day weather sample trip

#### Bugs fixed
- Clicking "Now" in "Animation Settings" no longer changes duration to one day unless "now" is outside animation duration
- `loopCount` value is incremented after trip is completed, but *before* any "post" scripts are executed.
- Graticule no longer overwrites the top longitude lines at low zoom values


<div style="background-color: lightblue; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.0.48
</span>  
<span style="float: right; margin: 6px;"  >
2023.03.06
</span>
<hr style="clear: both"/> 
</div>

#### New features
- added Graticule (lat, lon lines).  Enable them on the Settings page.

#### Bugs fixed
- Improved wind directional accuracy



<div style="background-color: lightblue; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.0.34
</span>  
<span style="float: right; margin: 6px;"  >
2023.03.01
</span>
<hr style="clear: both"/> 
</div>

#### New features
- Total redo of weather display
- Toggle buttons for chart, weather, pilot charts, tides and currents
- Fast access to route creation via Plus button
- Disable 3D, tilt, pitch.
- Scripting, added 'if' for condition event execution
- Scripting, added timezone event
- Scripting, show script error position
- Scripting, halt playback on error


#### Bugs fixed
- Sometimes route duration wasn't updated properly after changing route speed.


<div style="background-color: lightblue; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 2.0
</span>  
<span style="float: right; margin: 6px;"  >
2021.06.12
</span>
<hr style="clear: both"/> 
</div>

- Introduced 3D display, rotation, and tilt
- Introduced trip scripting

<div style="background-color: lightblue; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 1.0
</span>  
<span style="float: right; margin: 6px;"  >
2007.??.??
</span>
<hr style="clear: both"/> 
</div>

Just tides, currents, NOAA nautical charts