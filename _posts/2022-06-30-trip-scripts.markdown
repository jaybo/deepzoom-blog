---
title: "Scripting Routes - v2.5"
date: "2022-06-30 12:00:00 -0800"
categories: release trip
lastmod: "2022-06-30T20:34:20.077Z"
og_image: /assets/images/HowScriptsWork.png
---

### New features

1. You can now add script events to any route (previously scripts were only attached to the whole trip).  

    ![](/assets/images/HowScriptsWork.png){: .align-center style="border: 1px solid #aaa"}

Script events are added to one of three groups, depending on the selection of the topmost tab:

- **before:** All of these events run before the route or trip is activated.
- **during:** These events are activated relative to the route or trip completion (0.0 to 1.0, or time slider full left to slider full right).
- **after:** All of these events run after the route or trip completes.

In the example above, two events have been added to the **before** group of a route, setting the chart opacity to zero and selecting a current station before the route becomes active.

- Use the **+** button to add a new event, previously selected from the event type list.
- Use the garbage can button to delete any selected events from the list.
- Use the **Δ t** button to reassign the relative time of all selected events in the **during** group.  (First  drag the time slider to the moment you want the event to occur).

By default, adding a script event stores the current value of that setting, such as opacity, zoom, location, selected marker, selected tide station, etc.
But you can always edit the default setting by just clicking on the value in the list box.

***Trip Events vs Route Events***

While conceptually very similar, trip **during** events are relative the entire trip, while route **during** events are relative the particular route.
Also, trip **before** events are only executed once when the trip is first loaded.  Trip **after** events execute as the timeline loops back to the beginning.

### Bug fixes

1. After saving a trip, the timebase sometimes did not account for the last route in the trip.  

### Seattle to Glacier Bay updated

This trip has been updated to use route scripts, changing the nautical chart opacity to "0" during the Canadian routes.

Try it: [https://www.deepzoom.com/trip/4jvmcnf6](https://www.deepzoom.com/trip/4jvmcnf6)
{: .notice--warning}