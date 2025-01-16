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
    style="min-width: 375px; height: 80vh;"
    src="https://www.deepzoom.com/trip/yzahbfym">
</iframe>
</div>

The code:
```
<div>
<iframe id="theIframe"
    title="Inline Frame Example"
    width="100%"
    style="min-width: 375px; height: 80vh;"
    src="https://www.deepzoom.com/trip/yzahbfym">
</iframe>
</div>
```

Notice that these are fully functional instances of DeepZoom,  not just a movie playing.  A few features are disabled by browser security when running in an iFrame such
as all geolocation APIs.

### Load a trip
This is the most flexible means of specifying the location, zoom, layers, tab displayed, and virtually all of the settings in DeepZoom.
You can optionally customize the user experience by adding a script to the trip.

[https://www.deepzoom.com/trip/4jvmcnf6](https://www.deepzoom.com/trip/4jvmcnf6)
{: .notice--warning}

### Load a marker
If you want to always zoom to a particular public or private marker use `marker/{markerID}` as in:

[https://www.deepzoom.com/marker/a61cae5ca877eb87218b82fbdaebe599](https://www.deepzoom.com/marker/a61cae5ca877eb87218b82fbdaebe599)
{: .notice--warning}

### Load a clipboard link
Clipboard links let you set most state variables in DeepZoom. Use `s/{StateID}` as in:

[https://www.deepzoom.com/s/20250101-6TTprQ1xJf](https://www.deepzoom.com/s/20250101-6TTprQ1xJf)
{: .notice--warning}

For more info on clipboard links, see [https://blog.deepzoom.com/release/copy-link/](https://blog.deepzoom.com/release/copy-link/)
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

### Hoboken to Carnegie Hall

Hey, how do you get from Hoboken to Carnegie Hall?

<div>
<iframe id="theIframe2"
    title="DeepZoom embedded"
    width="100%"
    style="min-width: 375px; height: 80vh;"
    src="https://www.deepzoom.com/trip/dwmfjt2f">
</iframe>
</div>


