---
title: "Automatic routes - v3.18"
date: "2025-10-14 12:00:00 -0800"
categories: release 
og_image: /assets/images/AutorouteNY.png
---

### Automatic routes


<img src="/assets/images/AutorouteNY.png" style="box-shadow: 4px 4px 4px 0px rgba(0,0,0,0.5); margin-top: 12px; margin-bottom: 12px" width="40%" />{: .shadow .align-left .toc}

You can now automatically create routes!  

Just click (or tap and hold on touchscreens) near a small bullseye <img src="/assets/images/node.png"  style="margin-left: 4px; margin-right: 4px;" /> to add waypoints at the start and end of your route. 

The route will be the shortest path through a predefined traffic network.  Click on the route to add more constraint waypoints. Drag either end of the route, or the constraint waypoints to redefine the route.

{: .cf}
Once you're satisfied with the route, exit Autoroute mode.  You can then further refine the route using the standard **`Manual`** route tools, moving waypoints, adding to either end of the route, or splitting the route into fragments.

Routes can be arbitrarily long and are pretty fast!  Try something wild like starting a route in Anchorage, AK and ending in Newport R.I. 

<!-- <div class="fitvidsignore">
    <iframe  width="540" height="960" style="max-height: 80vh" src="https://www.youtube.com/embed/XbvrlLgNYgg?si=AS3kMS_gn6c_JKKy" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen> </iframe>
</div> -->

DEEPZOOM IS A PLANNING TOOL.  DO NOT TRUST ANY AUTOMATICALLY GENERATED ROUTE FOR NAVIGATION WITHOUT THOROUGH REVIEW.  AUTO CREATED ROUTES ARE NOT FILTERED BASED ON THE DRAFT OF YOUR VESSEL. SOMETIMES THE AUTO ROUTE IS ONLY A FEW FEET DEEP SUCH AS THE GULF ICW!
{: .notice--danger}

### How it works

<img src="/assets/images/AutorouteHeatmap.png"  style="box-shadow: 4px 4px 4px 0px rgba(0,0,0,0.5); margin-top: 12px; margin-bottom: 12px "   width="50%" />{: .border .align-left .toc}

DeepZoom uses the "wisdom of the crowd" to define the auto routing network. 

A heatmap of the frequency of AIS tracks over the course of a full year is used to create a network of nodes and edges. 
Manual editing further refines the network, avoiding obstructions and shallow areas. 

Each edge is a potential pathway. <br>
Each node is a potential waypoint.  

{: .cf}
Auto routes are the the shortest path through the network between the waypoints you place at two or more nodes.  The route follows waypoints you've placed in numerical order.  

To remove a waypoint, drag it onto another waypoint which will merge them into a single waypoint. 


Editing and verifying the network is a massive undertaking.  I started with waters I've frequented, and expanded from there.  Feedback is welcome!  What works, what doesn't.
The best way to show an error is either a screen shot with LatLong displayed, or click on the copy link button in the upper left corner of the display and paste that into an email
to jay at deepzoom.com. 
{: .notice--warning}

Do you have an interest in helping edit the network? If so, drop me an email, again jay at deepzoom.com.
{: .notice--warning}


### Other new features

- Routes are auto named in the format "Start to Finish".  If you reverse the route, the route name is also reversed. If you name a Trip in the format "Start to Finish", reversing the whole trip will swap the Start and Finish names.
You can disable auto renaming at `Settings.Routes.NameRouteFromEndpointLocations`.  If you manually edit a route name, your edits will be preserved.
- When manually editing a route, you can now extend the route from either the start or end waypoint.  Select the waypoint, then click the "+".

