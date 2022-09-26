---
title: "WCSNG - Research"
layout: gridlay
excerpt: "Pointillism"
sitemap: false
permalink: /pointillism/
---

# Pointillism: Accurate 3D Bounding Box Estimation with Multi-Radars
---
### Sensys 2020
```
Authors: Kshitiz Bansal, Keshav Rungta, Siyuan Zhu and Dinesh Bharadia
```
#### <a href="https://dl.acm.org/doi/10.1145/3384419.3430783" style="background-color: white; color: orange;">[Paper]</a> <a href="https://www.youtube.com/watch?v=jiAEwyHjPZs&amp;feature=youtu.be">[Video]</a> <a href="https://github.com/Kshitizbansal/pointillism_rp_net">[Code]</a> <a href="https://github.com/Kshitizbansal/pointillism-multi-radar-data">[Dataset]</a>

<!--<a href="{{ site.url }}{{ site.baseurl }}/files/Pointillism_paper.pdf" style="background-color: white; color: orange;">[Paper]</a> <a href="https://github.com/ucsdwcsng/mMobile" style="background-color: white; color: green;">[Datasets]</a>-->

<iframe width="560" height="315" src="https://www.youtube.com/embed/jiAEwyHjPZs" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<div class="well">
<h3> News: </h3>
<h5> Jul 2022: Open source code for RP-net released. Check it out at <a href="https://github.com/Kshitizbansal/pointillism_rp_net">github</a>!</h5>
<h5> Oct 2021: Multi-radar dataset has been released. Check it out at <a href="https://github.com/Kshitizbansal/pointillism-multi-radar-data">github</a>!</h5>
</div>


### Abstract
Autonomous perception requires high-quality environment sensing
in the form of 3D bounding boxes of dynamic objects. The primary
sensors used in automotive systems are light-based cameras and
LiDARs. However, they are known to fail in adverse weather conditions.
Radars can potentially solve this problem as they are barely
affected by adverse weather conditions. However, specular reflections
of wireless signals cause poor performance of radar point
clouds.We introduce Pointillism, a system that combines data from
multiple spatially separated radars with an optimal separation to
mitigate these problems. We introduce a novel concept of Cross
Potential Point Clouds, which uses the spatial diversity induced by
multiple radars and solves the problem of noise and sparsity in radar
point clouds. Furthermore, we present the design of RP-net, a novel
deep learning architecture, designed explicitly for radar’s sparse
data distribution, to enable accurate 3D bounding box estimation.
The spatial techniques designed and proposed in this paper are
fundamental to radars point cloud distribution and would benefit
other radar sensing applications.

---
<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/Radar/pointillism.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/Radar/pointillism.png" width="40%" style="float: center" > </a>
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/Radar/pointillism_overview.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/Radar/pointillism_overview.png" width="40%" style="float: center" > </a>
</div>

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
### Pointillism data collection platform.
 (Top Left) 16-
channel Ouster LiDAR, RealSense Depth Camera for ground truth
labels. (Top Right) our radars. (Bottom) Our System: Two radars,
LiDAR, Depth camera combined synchronously to common clock.


<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/Radar/pointillism_setup.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/Radar/pointillism_setup.png" width="40%" style="float: center" > </a>
</div>

---

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

### Supporters
<div class="col-sm-5 clearfix">
  <a href="https://ti.com"><img src="https://www.ti.com/content/dam/ticom/images/identities/ti-brand/ti-stk-2c-pos-rgb-logo.png" width="40%" style="float: left" > </a>

  <a href="https://toyota.com"><img src="https://www.carlogos.org/car-logos/toyota-logo-2019-3700x1200.png" width="40%" style="float: center" > </a>

  <a href="https://qualcomm.com"><img src="https://i.pinimg.com/originals/ba/68/1b/ba681b818f8160b96b29b41d8a639f2c.jpg" width="40%" style="float: right" > </a>
</div>




### Cite the paper
Kshitiz Bansal, Keshav Rungta, Siyuan Zhu and Dinesh Bharadia†. 2020.
Pointillism: Accurate 3D Bounding Box Estimation with Multi-Radars. In
The 18th ACM Conference on Embedded Networked Sensor Systems (SenSys
’20), November 16–19, 2020, Virtual Event, Japan. ACM, New York, NY, USA,
14 pages. https://doi.org/10.1145/3384419.3430783




<div class="well">
<h3> <font color="red">Press cover:</font>  </h3>
<h4> 11/20/2020:  <a style="display: inline-block;" href="https://www.10news.com/news/local-news/uc-san-diego-researchers-find-ways-to-make-self-driving-cars-safer">10News.com: UC San Diego researchers find ways to make self-driving cars safer</a> </h4>
<h4> 11/17/2020:  <a style="display: inline-block;" href="https://www.sciencedaily.com/releases/2020/11/201117192605.htm#:~:text=2-,Upgraded%20radar%20can%20enable%20self%2Ddriving%20cars%20to,clearly%20no%20matter%20the%20weather&text=Electrical%20engineers%20at%20the%20University,of%20objects%20in%20the%20scene.">ScienceDaily</a> and  <a style="display: inline-block;" href="https://jacobsschool.ucsd.edu/news/release?id=3161">UCSD News</a>: Upgraded radar can enable self-driving cars to see clearly no matter the weather. </h4>
</div>


