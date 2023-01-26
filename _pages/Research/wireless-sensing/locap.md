---
title: "WCSNG - Research"
layout: gridlay
excerpt: "LocAP"
sitemap: false
permalink: /locap/
---

# LocAP: Autonomous Millimeter Accurate Mapping of WiFi Infrastructure
---
### NSDI'20
```
Authors: Roshan Ayyalasomayajula, Aditya Arun, Chenfeng Wu, Shrivatsan Rajagopalan, Shreya Ganesaraman, Aravind Seetharaman, Ish Kumar Jain, and Dinesh Bharadia
```


#### <a href="{{ site.url }}{{ site.baseurl }}/files/LocAP_paper.pdf" style="background-color: white; color: #BA4A00;">[Paper]</a> <a href="{{ site.url }}{{ site.baseurl }}/files/LocAP_NSDI_slides.pdf" style="background-color: white; color: purple;">[Slides]</a> <a href="https://youtu.be/ZErYjC4Em5o" style="background-color: white; color: blue;">[Video]</a>

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZErYjC4Em5o" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Motivation
Indoor localization has been studied for nearly two decades fueled by wide interest in indoor navigation, achieving the necessary decimeter-level accuracy. However, there are no real-world deployments of WiFi-based user localization algorithms, primarily because these algorithms are infrastructure dependent and therefore assume the location of the Access Points, their antenna geometries, and deployment orientations in the physical map. In the real world, such detailed knowledge of the location attributes of the access point is seldom available, thereby making WiFi localization hard to deploy. 

<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/locap_main.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/locap_main.png" width="70%" style="float: center" > </a>
</div>
<br>


LocAP is an autonomous system to physically map the environment and accurately locate the attributes of existing wireless infrastructure in the physical space down to the required stringent accuracy of 3 mm antenna separation and 3 degree deployment orientation median errors, whereas state-of-the-art algorithm reports 150 mm and 25 degree respectively.

<br>
<br>
<br>
<br>
<br>



<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/locap_deployed.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/locap_deployed.png" width="90%" style="float: center" > </a>
</div>
LocAP is deployed on an autonomous bot which hosts a Lidar and a WiFi client. The bot moves around in a specific path and builds indoor maps using standard SLAM algorithms. Concurrently, the WiFi client on the bot collects channel state information (CSI) data from existing access points and run a novel algorithm on this data to estimate the access point attributes-- location, orientation, and antenna placement.
<br>
<br>
<br>
<br>

***


#### See similar papers: <a href="{{ site.url }}{{ site.baseurl }}/dloc" style="background-color: white; color: blue;">DLoc (deep learning based localization)</a>
