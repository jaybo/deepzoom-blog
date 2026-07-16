---
title: Spatial Currents - v3.28
date: 2026-07-15 15:41:20 -0800
categories: release 
lastmod: 026-07-15 15:41:20 -0800
draft: false
---


<div style="background-color: #eee; margin-top: 20px">
<iframe id="theIframeSpatialCurrents"
    title="SpatialCurrents"
    width="98%"
    style="min-width: 375px; height: 100vh; max-height: 720px"
    allow="clipboard-read; clipboard-write"
    src="https://www.deepzoom.com/s/20260715-pdNbrnHXa8">
</iframe>
</div>


DeepZoom has always shown tidal currents as arrows at official current stations — NOAA in the US, CHS in Canada. **Spatial Currents fills in the gaps:** a continuous, color-coded, animated tidal-current field.

Turn it on and you get three things:

- **Color** for speed. The scale is stepped in discrete bands of an eighth of a knot each, so equal-speed regions read as a filled contour.
- **Streamers** — show direction, speed, and structure. 
- **Speed readout** (optional) at the center crosshair, in your chosen units. Off by default, but you can enable this at <i>Settings → Map → Show spatial current velocity at center</i>, but, see below...

Like everything in DeepZoom it animates through time, so you can scrub to any date and time and watch the whole field flood and ebb.

## Where it comes from

The data is the **ADCIRC tidal constituent databases**: EC2015 for the Atlantic, Gulf, and Caribbean, and ENPAC15 for the Pacific coast including British Columbia and southern Alaska. They were produced by the University of Oklahoma together with NOAA's Coast Survey Development Laboratory, using the ADCIRC coastal circulation model developed at UNC Chapel Hill and Notre Dame. Together they model the coastal ocean as an unstructured triangular mesh of roughly two million nodes, refined down to tens of meters inside harbors and inlets.

At each node the database stores the amplitude and phase of several dozen tidal constituents — the same M2, K1, O1 and friends behind the station tide predictions DeepZoom already computes for NOAA and CHS tide stations.

## Why it won't match the current tables — and why that's expected

You'll likely notice discrepancies between Spatial Currents and the NOAA/CHS current station arrows. It's not a bug. The two models are answering slightly different questions.

**A NOAA current station is local truth; the Spatial Currents field is a regional model.** NOAA and CHS derive their predictions from harmonic analysis of actual current measurements at an exact geographical location, so they capture the reality of that particular spot. Spatial Currents is a smooth regional model — excellent for the big picture, but only approximate at any single point.

**Depth-averaged vs. a specific depth.** The ADCIRC field is a single **depth-averaged** velocity for the whole water column. A NOAA/CHS prediction is for a **specific depth** — usually well up in the column, where the water runs faster than the column average. Even with a flawless model, comparing a depth-average against a near-surface reading can differ wildly.

**Currents are spatially violent, and current stations sit in the worst spots.** Speed can double over a few tens of meters near a sill, a narrows, or a headland — and current stations are almost always placed in exactly those pinch points (Deception Pass, Cape Cod Canal, Seymour Narrows). 

**Currents are harder to model than tide height.** The ADCIRC databases were validated mostly against tidal *heights*, where they're very good — errors of a few percent. Velocity is essentially the gradient of the height field, which amplifies every small error, and the sharp flood/ebb asymmetry of a real rapids depends on shallow-water overtides that a regional model under-represents.


The practical rule: **where a current station exists, trust it.** Use Spatial Currents for what the stations can't give you — the shape and timing of the flow *between* stations, across a whole region at once. Expect the biggest disagreements precisely in the strong, narrow rapids boaters care about most, for all the reasons above.


## Sources

- ADCIRC tidal databases (EC2015, ENPAC15): <a href="https://adcirc.org/products/adcirc-tidal-databases/">https://adcirc.org/products/adcirc-tidal-databases/</a>
- EC2015 paper: <a href="https://doi.org/10.3390/jmse4040072">https://doi.org/10.3390/jmse4040072</a>
- ENPAC15 paper: <a href="https://www.mdpi.com/2077-1312/6/4/131">https://www.mdpi.com/2077-1312/6/4/131</a>


## Other features

- Images on the clipoard can be directly pasted into the Images section of a comment.
- A cartoon of the tidal bulge is drawn on the <i> Relative angular positions of the earth, sun, and moon </i> animation on the Tides tab.

## Bug Fixes

- the script `loopCount` variable was sometimes incrementing twice per execution of the timeline.
- Route speeds and lengths now respect Settings → Units → Distance instead of always showing nMi.
- Tidal events in the <i>Tides → Table</i> view were showing events in UTC instead of local time for the station.



