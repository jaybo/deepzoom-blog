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