---
title: Embed DeepZoom - v2.8
date: 2022-10-01 15:41:20 -0800
categories: release 
lastmod: 2022-10-01T20:44:01.227Z
og_image: /assets/images/trip-icw.png
draft: false
---
## Embedding DeepZoom in your own website

DeepZoom can be embedded in your own website via an iframe.  You can specify a particular trip or page to be loaded via the Url passed in the `src` parameter.
Here are some typical examples

<div>
<iframe id="theIframe"
    title="DeepZoom embedded"
    width="100%"
    height="600"
    src="https://www.deepzoom.com/trip/yzahbfym">
</iframe>
</div>

The code:
```
<div>
<iframe id="theIframe"
    title="Inline Frame Example"
    width="100%"
    height="600"
    src="https://www.deepzoom.com/trip/yzahbfym">
</iframe>
</div>
```

You can specify a particular trip or page to be loaded via the Url passed in the `src` parameter of the iframe.
Here are some typical examples:

### Load a trip
This is the most flexible means of specifying the location, zoom, layers, tab displayed, and virtually all of the settings in DeepZoom.
You can optionally customize the user experience by adding a script to the trip.

[https://www.deepzoom.com/trip/4jvmcnf6](https://www.deepzoom.com/trip/4jvmcnf6)
{: .notice--warning}

### Load a marker
If you want to always zoom to a particular public or private marker use `marker/{markerID}` as in:

[https://www.deepzoom.com/marker/a61cae5ca877eb87218b82fbdaebe599](https://www.deepzoom.com/marker/a61cae5ca877eb87218b82fbdaebe599)
{: .notice--warning}

Or you could have more elaborate scenarios with buttons to load different markers or trips:

```
<script >
    let changeSrc = function (src) {
        let iFrame = document.getElementById("theIframe");
        iFrame.src = src;
    }
    changeSrc("https://www.deepzoom.com/trip/4jvmcnf6");
</script>

<btn 
  onclick="changeSrc('https:\/\/www.deepzoom.com/marker/a61cae5ca877eb87218b82fbdaebe599')" > 
  Jump to marker ID: a61cae5ca877eb87218b82fbdaebe599 
</btn>
```


