---
title: "DeepZoom - v3.14.84"
date: "2024-05-26 12:00:00 -0800"
categories: release 
lastmod: "2024-05-26:34:20.077Z"
og_image: /assets/images/HowScriptsWork.png
---

### Scripting

Finally completed the scripting [documentation](https://deepzoom.com/doc/index.html).

#### New scripting features:
- `id` for route or marker is now a regular expression, allowing wildcard matches.  
    See: [https://www.deepzoom.com/doc/variables/id.html](https://www.deepzoom.com/doc/variables/id.html)
- added [routeProperties](https://www.deepzoom.com/doc/functions/routeProperties.html) event.

#### New document features:
- Image links can now be added to a document.  This is useful for webcams: [Seattle ferry dock](https://deepzoom.com/marker/8866753532864865/0)
- Added a button to remove formatting.
- Ensure all images are loaded before allowing save.

#### Other new featues
- Allow changing the departure time for **all** routes simultaneously in the departure time dialog.
- Always show the timebase duration above the time readout.
- Added [UTC](https://deepzoom.com/settings) to the timezone list.


#### Editing Route and Marker properties

You can now change a route name, departure date, departure time, speed, and color right from the route edit dialog.

For example, to change the speed, click on the speed readout and then drag the slider.

![](/assets/images/route-edits.png){: .align-left .toc} 
![](/assets/images/route-edit-speed.png){: .align-left .toc} 

<br/>
<div style="clear: left"></div>

Close the routes/markers dialog to exit **edit** mode.

Tip! To quickly toggle between routes and markers click the "routes" or "markers" label in the upper left corner of the dialog.
{: .notice}

#### Update all NOAA charts

Updated all NOAA charts to the 2024.05.28 NOAA release.
Charts were publilshed to DeepZoom on 2024.06.11.


