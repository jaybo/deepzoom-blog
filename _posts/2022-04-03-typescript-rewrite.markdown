---
title: "The TypeScript rewrite - v2.3"
date: "2022-04-03 12:00:00 -0800"
categories: release trip
lastmod: "2022-01-17T20:41:08.342Z"
og_image: /assets/images/save-trip.png
---

### JavaScript, the quandary 

I started writing DeepZoom in 2007??? when I knew just about nothing about the lingua franca of the web: JavaScript.  Over the intervening decade and a half, I've worked on the code sporadically, 
but then really kicked into gear again in 2020 as Covid hit.  As a result, the codebase was a mashup of different styles, reflecting changes in my understanding of JavaScript best practices, 
and adopting modern features of the language as it evolved every few years.

Overall, the experience has been terrifying.  Coming from a background in strongly typed languages such as C, C++, and C#, the whole dynamic nature of JavaScript where a variable can
morph to contain content of any type has been disquieting.  Gary Bernhardt has a fun video on the subject of JavaScript inconsistencies: <a href="https://www.destroyallsoftware.com/talks/wat" target="_blank"> Wat</a>

<a href="https://www.destroyallsoftware.com/talks/wat" target="_blank"> <img src="/assets/images/WAT.png"/></a>{: .align-center}

Some typical JavaScript madness:

```
// random JavaScript: Is k a string, a number, or something else?
let k = "you'll never take me alive, Copper!"
k = 42
k = lifeTheUniverseEverything(k)
```

Equally frightening, DeepZoom is directly dependent on ~40 other NPM packages (code libraries), which in turn rely on over 1,300 other libraries.  Any 
of which can be randomly updated, bugs added or fixed, and behaviors changed.  In a typical week two or three of the direct dependency libraries will be updated.

Meanwhile DeepZoom continues to grow.  It's currently about 80 files, and about 30,000 lines of code (not counting images and other assets).  

`find ./ -type f -regex '.*\.\(vue\|js\|ts\)$' -print0 | wc -l --files0-from=-  // LOC js, ts, vue`
{: .notice--warning}

Not huge by any means, but large enough that attempting non-trivial enhancements was a challenge.  Partly because I lacked the discipline to document every function, variable, and return value, but also due to the nature of JavaScript itself.
Enter ... TypeScript.

### The TypeScript rewrite

I've been casting longing glances in the direction of TypeScript for a few years.  And I finally took the plunge.  After flicking some switches in the Quasar tooling to enable TypeScript, I started  with the simplest modules with the fewest dependencies, and just changed the
file extension from `.js` to `.ts`.  Add a few type definitions, and it's working!  VSCode starts showing intellisense for all variables and functions.  Errors pop up when types don't match. 

The largest modules took a few days to port over; overall I spent about two months on the rewrite. During the rewrite maybe two dozen real bugs popped up due to type checking.  And there were a few sections of code that I just scratched my head and wondered how/if it ever really worked.

The relief is palpable.  


### Fixes

- New drawer menu on mobile devices
- Handle the iPhone "notch" and `env(safe-area-inset-*)`
- Fix all known issues with changing route names

### Seattle to Glacier Bay

To test all this new functionality, I created a Trip based on our 2001 expedition from Seattle to Glacier Bay aboard s/v Serenade.  The trip includes 28 routes, and has a duration of about a month.

[![](/assets/images/iPhoneGlacierBay.png)](https://www.deepzoom.com/trip/bjwhbzpv)

Try it: [https://www.deepzoom.com/trip/bjwhbzpv](https://www.deepzoom.com/trip/bjwhbzpv)
{: .notice--warning}