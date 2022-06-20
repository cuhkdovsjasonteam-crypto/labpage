---
title: "WCSNG - Research"
layout: gridlay
excerpt: "WCSNG -- Research"
sitemap: false
permalink: /greenmo/
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
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}
</style>

<!-- # Wireless Contact Force Sensing
---
 -->

<!-- #### <a href="{{ site.url }}{{ site.baseurl }}/files/scattermimo.pdf" style="background-color: white; color: orange;">[Paper]</a> [Slides] <a href="https://drive.google.com/file/d/1825BK0-l8t_vvKw26bb-Maba-qALoHEl/view?usp=sharing">[Video]</a> -->



# Building next-generation power-efficient base-stations with GreenMO
<div class="row">
<div class="col-sm-6 clearfix">
<br>
<p style="font-size:30px">Motivation</p>
<p align="justify"> 
Today, wireless base-stations consume a lot of power and contribute significantly to the carbon footprint of wireless industry (1.4%), which compares to that of aviation industry (2%).
Further, with next-generation networks connecting more users, and even more devices, the power consumption is only going to increase, with <span style="color:orange;">more antennas</span> and <span style="color:red;">more data backhauling</span> required.
</p>
</div>


<div class="col-sm-6 style=float: right;">
<!-- <div class="videoWrapper">
  <iframe width="560" height="315" src="https://drive.google.com/file/d/1825BK0-l8t_vvKw26bb-Maba-qALoHEl/preview" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div> -->
<a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/greenmo_motiv.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/greenmo_motiv.png" width="100%" style="float: center" > </a>
</div>
</div>

---


<div class="row">


<div class="col-sm-6" style="float: left;">
 <p style="font-size:30px">GreenMO breaks power-spectrum tradeoff</p>
<a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/greenmo_tradeoff.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/greenmo_tradeoff.png" width="100%" style="float: center" > </a>
GreenMO virtualizes a single high bandwidth RF chain over multiple antennas to create a best of both worlds solution which is as power efficient as OFDMA and as spectral efficient as massive MIMO.
</div>

<div class="col-sm-6" style="float: right;">
<p style="font-size:30px">Prototype hardware</p>
<center>
<a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/greenmo_pcb.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/greenmo_pcb.png" width="100%" > </a> <br>
</center>
We design a custom PCB which can allows for 4 users multiplexing via 8 antennas connnected to a single RF chain of WARPv3 SDR
</div>

</div>

---

## Publications

<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="{{ site.url }}{{ site.baseurl }}/files/greenmo.pdf">GreenMO: Flexible and Virtualized Green
Communications Architecture</a> 
    Agrim Gupta, Sajjad Nassirpour, Eamon Patamasing, Manideep Dunna, Alireza Vahid, Dinesh Bharadia<br>
    (Under submission)<br>
</div>
</div>


