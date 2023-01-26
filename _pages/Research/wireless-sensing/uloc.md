---
title: "ULoc"
layout: gridlay
excerpt: "UWB Localization"
sitemap: false
permalink: /uloc/
---
<style type="text/css" rel="stylesheet">
.videoWrapper {
    position: relative;
    padding-bottom: 56.25%; /* 16:9 */
    padding-top: 25px;
    height: 0;
}
.videoWrapper iframe {
    position: absolute;
    top: 200;
    left: 0;
    width: 100%;
    height: 100%;
}
</style>

<!-- # Wireless Contact Force Sensing
---
 -->

<!-- #### <a href="{{ site.url }}{{ site.baseurl }}/files/scattermimo.pdf" style="background-color: white; color: orange;">[Paper]</a> [Slides] <a href="https://drive.google.com/file/d/1825BK0-l8t_vvKw26bb-Maba-qALoHEl/view?usp=sharing">[Video]</a> -->



# ULoc: a cm-accurate, low-latency and power-efficient UWB tag localization system
<div class="row">
<div class="col-sm-5 clearfix">
<br>
<p style="font-size:30px">Motivation</p>
<p align="justify"> 
	A myriad of IoT applications demand centimeter-accurate localization that is robust to blockages from hands, furniture, or other occlusions in the environment. To address these needs, we developed ULoc, a scalable, low-power, and cm-accurate UWB localization and tracking system. ULoc's builds a multi-antenna UWB anchor and develops a novel 3D tracking algorithm to deliver a stationary localization accuracy of less than 5 cm and a tracking accuracy of 10 cm in mobile conditions. Follow the demo links below to see ULoc in action. Furthermore, we have also open sourced our hardware design files and source code. 
</p>
</div>


<div class="col-sm-7 clearfix">
<div class="videoWrapper">
  <!-- <iframe width="560" height="315" src="https://www.youtube.com/watch?v=04yScpakpPc" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
 -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/i4WKW57hmog" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
</div>
</div>

---


<div class="row">

<div class="col-sm-6" style="float: left;">
<p style="font-size:30px">A UWB tag can be located with cm-scale accuracy in 3D with just a single beacon transmission</p>
<center>
<a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/uloc/overview.jpg"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/uloc/overview.jpg" width="90%" > </a> <br>
</center>

ULoc's core design principle is to enable localizing the simplest tag. We note the surprising realization that receiving a UWB packet can consume over 50% more power than a tranmission. Equipped with this knowledge, ULoc's protocol relies only on a single beacon packet to be transmitted by the tag to localize it in 3D space. We push the complexity of providing the location to the deployed infrastrucutre and the ULoc Anchors. In this manner, the tag can remain power efficient. Furthermore, the single-packet location estimation reduces the latency of the entire system.

</div>

<div class="col-sm-6" style="float: center;">
 <p style="font-size:30px">ULoc Anchors's 2D-antenna array capable of furnishing 3D-AoA</p>
<a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/uloc/uloc-images-large.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/uloc/uloc-images-large.png" width="100%" style="float: center" > </a>
For the first time, ULoc developed and tested a UWB Anchor with 8 antennas placed in an L-shaped to measure both the azimuth and polar angle of arrival (3D-AoA) of a UWB pulse. Using trilateration, these 3D-AoA measurements are combined over at least 2 AP's to provide cm-accuarate tag localization.  
</div>

</div>

---

## Publications

<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="{{ site.url }}{{ site.baseurl }}/files/uloc.pdf">ULoc: Low-Power, Scalable and cm-Accurate UWB-Tag Localizationand Tracking for Indoor Applications</a> 
<a style="background-color: white; color: blue;" href="https://youtu.be/-g2nTatJDQk">[Demo 1]</a>
<a style="background-color: white; color: blue;" href="https://youtu.be/8EU1JmH-dto">[Demo 2]</a>
<a style="background-color: white; color: blue;" href="https://github.com/ucsdwcsng/ULoc-public">[Source]</a>
<br> Minghui Zhao, Tyler Chang, Aditya Arun, Roshan Ayyalasomayajula, Chi Zhang, Dinesh Bharadia
<br>IMWUT 2021<br>
</div>
</div>

