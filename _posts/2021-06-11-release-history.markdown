---
title: DeepZoom Release History
date: 2021-06-11 15:41:20 -0800
categories: release 
lastmod: 2021-06-11T20:44:01.227Z
og_image: /assets/images/WeatherHUD.png
draft: false
---


<div style="background-color: #e0ecff; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.18.1
</span>  
<span style="float: right; margin: 6px;"  >
2025.10.15
</span>
<hr style="clear: both"/> 
</div>



#### New features
- Auto routes.
- Auto route names.
- Extend manual routes.


<div style="background-color: #e0ecff; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.16.8
</span>  
<span style="float: right; margin: 6px;"  >
2025.06.04
</span>
<hr style="clear: both"/> 
</div>



#### New features
- Undo / Redo.  Geometry (routes and markers) modifications automatically trigger an addition to the undo stack. The undo and redo stacks are of unlimited size.
Note that changing route properties does *not* trigger an undo stack addition unless the geometry is altered. 




<div style="background-color: #e0ecff; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.16.6
</span>  
<span style="float: right; margin: 6px;"  >
2025.05.28
</span>
<hr style="clear: both"/> 
</div>



#### New features
- Merge routes. Just drag route endpoints togeter to merge.

#### Bugs fixed
- Save a trip with Markers somewhat randomly failed to save the markers. Doh!
- Reduced the incidence of spurious route snipping and vertex deletion.




<div style="background-color: #e0ecff; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.15.7
</span>  
<span style="float: right; margin: 6px;"  >
2025.01.01
</span>
<hr style="clear: both"/> 
</div>



#### New features
- Clipboard links now include most application state.
- Change portrayal of tide stations to circular shape.

#### Bugs fixed
- Handle lazy loading when embedded in iFrame.
- Improve time zone list usability.




<div style="background-color: #e0ecff; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.14.93
</span>  
<span style="float: right; margin: 6px;"  >
2024.10.03
</span>
<hr style="clear: both"/> 
</div>



#### New features
- Show NBDC buoys with real time weather data.
- Search: find tides and current stations by name.

#### Bugs fixed
- Touchscreen premature route creation termination fixed.
The gory details are [here](https://github.com/mapbox/mapbox-gl-draw/issues/1212). 
- Settings: The Celsius selection now actually does something.
- Login: login status is now more sticky during refreshes.








<div style="background-color: #e0ecff; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 3.14.88
</span>  
<span style="float: right; margin: 6px;"  >
2024.05.27
</span>
<hr style="clear: both"/> 
</div>

#### New features
- Update route and marker properties (name, departure date and time, speed, color) within the edit dialog.
- Scripting: [documentation](https://www.deepzoom.com/doc/index.html) added.
- Scripting: `id` for route or marker is now a regular expression, allowing wildcard matches.  
    See: [https://www.deepzoom.com/doc/variables/id.html](https://www.deepzoom.com/doc/variables/id.html)
- Scripting: added [routeProperties](https://www.deepzoom.com/doc/functions/routeProperties.html) event.
- Documents: Image links can now be added to a document.  This is useful for webcams: [Seattle ferry dock](https://deepzoom.com/marker/8866753532864865/0)
- Documents: Added a button to remove formatting.
- Documents: Ensure all images are loaded before allowing save.
- Allow changing the departure time for **all** routes simultaneously in the departure time dialog.
- Always show the timebase duration above the time readout.
- Added [UTC](https://deepzoom.com/settings) to the timezone list.


#### Bugs fixed
- Changing a route departure time by clicking the clock icon wasn't working.
- Searching for lat/lng coordinates handles more formats.
- Null exception in TripFind if no firstName.
- Allow marker selection except when creating or editing routes.
- Copy postion or marker link to clipboard failed in Prodction.
- Refreshing the PWA version when a new version is released seems happier. ☺







<div style="background-color: #e0ecff; " >
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



<div style="background-color: #e0ecff; " >
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










<div style="background-color: #e0ecff; " >
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




<div style="background-color: #e0ecff; " >
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





<div style="background-color: #e0ecff; " >
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




<div style="background-color: #e0ecff; " >
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


<div style="background-color: #e0ecff; " >
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



<div style="background-color: #e0ecff; " >
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


<div style="background-color: #e0ecff; " >
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

<div style="background-color: #e0ecff; " >
<span style="float: left; font-size: 24px; font-weight: bold; margin: 6px;"> 
v 1.0
</span>  
<span style="float: right; margin: 6px;"  >
2007.??.??
</span>
<hr style="clear: both"/> 
</div>

Just tides, currents, NOAA nautical charts