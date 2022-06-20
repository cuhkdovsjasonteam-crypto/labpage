---
title: "WCSNG - Research"
layout: gridlay
excerpt: "SyncScatter"
sitemap: false
permalink: /syncscatter/
---

# SyncScatter: Enabling WiFi like synchronization and range for WiFi backscatter Communication
---
### NSDI 2021
```
Authors: Manideep Dunna, Miao Meng, Po-Han Wang, Chi Zhang, Patrick Mercier, and Dinesh Bharadia
```


#### <a href="{{ site.url }}{{ site.baseurl }}/files/syncscatter.pdf" style="background-color: white; color: orange;">[Paper]</a> <a href="{{ site.url }}{{ site.baseurl }}/files/nsdi21_slides_dunna.pdf" style="background-color: white; color: purple;">[Slides]</a> <a href="https://drive.google.com/file/d/1HLOmupRVde8Akssg3BT88-4PR7vTBsR5/view?usp=sharing">[Video]</a>



### Motivation
WiFi backscattering can enable direct connectivity of IoT de-vices with commodity WiFi hardware at low power. However,most existing work in this area has overlooked the importanceof synchronization and, as a result, accepted either limitedrange between the transmitter and the IoT device, reducedthroughput via bit repetition, or both. 


<div class="col-sm-12 clearfix">
  <center><a href="{{ site.url }}{{ site.baseurl }}/images/respic/backscatter/syncscatter.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/backscatter/syncscatter.png" width="60%"  > </a>
  </center>
</div>


### Overview 
we present SyncScatter, which achieves accurate synchronization with incident signals at the IoT device level while realizing maximum possible sensitivity afforded by a backscatter link budget. SyncScatter creates a novel modeling framework and derives the maximal optimal range and synchronization error that the receiver can tolerate without significant performance compromises. Next, SyncScatter builds a novel hierarchical wakeup protocol, which, together with a custom ASIC, achieves arange of 30+ meters and the peak throughput of 500Kbps, with an average power consumption of 30μW.




