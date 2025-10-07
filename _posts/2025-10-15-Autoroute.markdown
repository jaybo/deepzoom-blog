---
title: "Auto routes - v3.18.1"
date: "2025-10-15 12:00:00 -0800"
categories: release 
og_image: /assets/images/AutorouteNY.png
---

### Auto routes


<img src="/assets/images/AutorouteNY.png" style="float: left; margin-right: 16px" width="50%" />

You can now automatically create routes!  

Just click near a small dot marking the start location and an end location of your route. The shortest path through a predefined traffic network will be automatically created.  Click on the route to add more constraint waypoints. Drag either end of the route, or the constraint waypoints to redefine the route.

Once you're satisfied with the route, exit Autoroute mode.  You can then further refine the route using the standard Manual route tools, moving waypoints, adding to either end of the route, or splitting the route into fragments.

Routes can be arbitrarily long and are Fast!  Try something wild like starting in Anchorage, AK and ending in Newport R.I. 

DEEPZOOM IS A PLANNING TOOL.  DO NOT TRUST ANY AUTOMATICALLY GENERATED ROUTE WITHOUT THOROUGH REVIEW.  ROUTES ARE NOT FILTERED BASED ON THE DRAFT OF YOUR VESSEL. 

### How it works

<img src="/assets/images/AutorouteHeatmap.png" style="float: left; margin-right: 16px;"  width="50%" />

Multiple techniques have been used in various products to automatically create routes between a start and end waypoint.  The technique used by DeepZoom is to define a network of nodes and edges.  Auto routes are the the shortest path through the network.  

The network definition is mostly inspired by a cumulative AIS heatmap.  So the resulting network is literally "the wisdom of the crowd".  Further refinement is done manually to avoid obstructions. 


#### Other new features

- Routes are auto named in the format "Start to Finish".  If you reverse the route, the route name is also reversed. 
- When manually editing a route, you can now extend the route from either the start or end waypoint.  Select the waypoint, then click the "+".



#### Bug Fixes

- M