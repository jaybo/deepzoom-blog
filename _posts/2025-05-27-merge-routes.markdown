---
title: "Merge routes - v3.16.6"
date: "2025-05-28 12:00:00 -0800"
categories: release 
lastmod: "2025-05-28:34:20.077Z"
og_image: /assets/images/merge-routes.png
---

### Merging routes

You can now merge routes by dragging endpoints together.  The route endpoint being dragged is the source route, the other route is the destination route.
                                The name, direction, speed, and color properties of the destination route are preserved.

<img src="/assets/images/merge-routes.png"  width="50%" style="border: 2px solid #777;"/>


#### Other new features

- An account now includes boatname, which is going to be displayed as part of a future tracking feature.
- Added webcam marker icon.
- Added bidirectional client/server communication using signalR.  At present this is used to indicate when the server will be going down for maintenance.



#### Bug Fixes

- Markers were sometimes not saved in a trip. Doh! Sorry! Fixed.
- Improved route editing by eliminating spurious route snipping and vertex deletion.
