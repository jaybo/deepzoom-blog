---
title: DeepZoom Release History
date: 2021-06-11 15:41:20 -0800
categories: release 
lastmod: 2021-06-11T20:44:01.227Z
og_image: /assets/images/WeatherHUD.png
draft: false
---

**v 3.0.51**  <span style="float: right"  >2023.03.08</span>
{: .notice--warning}

#### New features
- Added 3 day weather sample trip

#### Bugs fixed
- Clicking "Now" in "Animation Settings" no longer changes duration to one day unless "now" is outside animation duration
- `loopCount` value is incremented after trip is completed, but *before* any "post" scripts are executed.
- Graticule no longer overwrites the top longitude lines at low zoom values


**v 3.0.48**  <span style="float: right"  >2023.03.06</span>
{: .notice--warning}

#### New features
- added Graticule (lat, lon lines).  Enable them on the Settings page.

#### Bugs fixed
- Improved wind directional accuracy




**v 3.0.34**  <span style="float: right"  >2023.03.01</span>
{: .notice--warning}

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


**v 2.0**  <span style="float: right"  >2021.06.12</span>
{: .notice--warning}

- Introduced 3D display, rotation, and tilt
- Introduced trip scripting


**v 1.0**  <span style="float: right"  >2007.??.??</span>
{: .notice--warning}
Just tides, currents, NOAA nautical charts