---
title: "WCSNG - Research"
layout: projectnewslay
excerpt: "BLoc"
sitemap: false
permalink: /bloc/
---

# BLoc: CSI-based accurate localization for BLE tags
---
### CoNEXT'18
```
Authors: Roshan Ayyalasomayajula, Deepak Vasisht, and Dinesh Bharadia
```


#### <a href="{{ site.url }}{{ site.baseurl }}/files/bloc_paper.pdf" style="background-color: white; color: orange;">[Paper]</a> <a href="{{ site.url }}{{ site.baseurl }}/files/bloc-ppt.pdf" style="background-color: white; color: green;">[Slides]</a> <a href="https://youtu.be/tC70Hs8cjwI">[Video]</a>

### Motivation
State of the art localization using Bluetooth Low Energy (BLE) devices uis based on RSSI, while Wi-Fi has achieved decimeter level localization using Channel State Information (CSI) based localization. With this work we bring CSI based sub-meter level accurate localization for BLE tags. We achieve this by enabling relative wideband CSI measurements for BLE devices with following three main contrinutions. Further details and implementaiton of BLoc can be found in our <a href="{{ site.url }}{{ site.baseurl }}/files/bloc_paper.pdf">paper</a> published in CoNEXT 2018.

<div class="col-sm-8 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/bloc_1st_contribution.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/bloc_1st_contribution.png" width="100%" style="float: right" > </a>
</div>
BLE devices employ GFSK modulation which makes the frequency continuously vary at the receiever end. To oevercome this BLoc employs un-whitened long sequences of 1's and 0's to stabilize the frequency as shown.
<br>
<br>

***

<div class="col-sm-8 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/bloc_2nd_contribution.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/bloc_2nd_contribution.png" width="100%" style="float: right" > </a>
</div>
Further BLE trnasmissions hapen in a band of 2MHz bandwidth, we overcome this limited bandwidth by extending the bandwidth by stitching across all the 37 data bands of BLE device.
<br>

***

<div class="col-sm-8 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/bloc_3rd_contribution.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/bloc_3rd_contribution.png" width="100%" style="float: right" > </a>
</div>
<br>
<br>
Finally, as the transmitter and receiver have heir unique clocks based intial phases that differe for each band making the phase across the 37 bands highly non-linear. We overcome this by measureing relative channels.
<br>
<br>
<br>
<!-- <br> -->

***
These contributions enable relative wideband CSI measurements for BLE devices thus enabling sub-meter accurate, robust indoor localization for BLE tags. You can find further details in the following video and implementation details in our paper.


### Watch the Video
<iframe width="900" height="506" src="https://www.youtube.com/embed/tC70Hs8cjwI" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
