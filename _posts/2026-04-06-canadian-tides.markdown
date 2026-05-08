---
title: Canadian tides and currents - v3.26
date: 2026-04-06 15:41:20 -0800
categories: release 
lastmod: 2026-04-06 15:41:20 -0800
draft: false
---


<div style="margin-top: 20px">
<iframe id="theIframeCanadaTides"
    title="DeepZoom embedded"
    width="100%"
    style="min-width: 375px; height: 85vh; max-height: 700px"
    allow="clipboard-read; clipboard-write"
    src="https://www.deepzoom.com/s/20260407-0ujdWAm9ZW">
</iframe>
</div>

Finally added Canadian tides and currents. These are derived from the API at [Canadian Hydrographic Service](https://tides.gc.ca/en/web-services-offered-canadian-hydrographic-service), and thus presumably "exactly" match official distributions.  

For the moment only 2026 is available, and the CHS API only supports a limit future range.  But future predictions await the release of 
an update to the time processing package used by DeepZoom called [moment-timezone](https://github.com/moment/moment-timezone/issues/1141#issuecomment-4015594101). This is complicated by the recent change to DST for British Columbia.

The somewhat hilarious holdup is that the BC Parliment chose a name for the new Timezone designation which overlaps preexisting usage.

>In fact, it's this long-standing colloquial usage that is causing consternation on the tzdb list at the moment. Due to this poorly-consulted decision from the BC government, the term "Pacific Time" will now mean two completely different time offsets for half the year, depending on where it's used. 

So I'm holding off on extending the prediction horizon until this is resolved.


#### Bug Fixes

- DeepZoom has possibly forever miscredited some percentage of user subscriptions. Somewhat randomly, accounts were either overcredited or undercredited for the subscription ending date. DeepZoom was misinterpreting a field from a Stripe webhook describing the transaction.  <b> Uff da!  I am massively sorry! </b> 


I believe all accounts have been corrected.  If you feel your account has not been properly credited please contact jay @ deepzoom . com.
{: .notice--warning}