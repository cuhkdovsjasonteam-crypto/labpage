---
title: "WCSNG - Research"
layout: gridlay
excerpt: "ScatterMIMO"
sitemap: false
permalink: /scattermimo/
---

# ScatterMIMO: Enabling Virtual MIMO with Smart Surfaces
---
### Mobicom 2020
```
Authors: Manideep Dunna, Chi Zhang, Daniel Sievenpiper, Dinesh Bharadia
```


#### <a href="{{ site.url }}{{ site.baseurl }}/files/scattermimo.pdf" style="background-color: white; color: orange;">[Paper]</a> [Slides] <a href="https://youtu.be/V96rOy8-FF4">[Video]</a>

<iframe width="560" height="315" src="https://www.youtube.com/embed/V96rOy8-FF4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Motivation
In the last decade, the bandwidth expansion and MIMO spatial multiplexing have promised to increase data throughput by ordersof magnitude. However, we are yet to enjoy such improvementin real-world environments, as they lack rich scattering and pre-clude effective MIMO spatial multiplexing. 


<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/scattermimo.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/scattermimo.png" width="70%" style="float: center" > </a>
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

### Overview 
We present
ScatterMIMO, which uses smart surface to increase the scattering
in the environment, to provide MIMO spatial multiplexing gain.
Specifically, smart surface pairs up with a wireless transmitter device
say an active AP and re-radiates the same amount of power
as any active access point (AP), thereby creating virtual passive
APs. ScatterMIMO avoids the synchronization, interference, and
power requirements of conventional distributed MIMO systems
by leveraging virtual passive APs, allowing its smart surface to
provide spatial multiplexing gain, which can be deployed at a very
low cost. We show that with optimal placement, these virtual APs
can provide signals to their clients with power comparable to real
active APs, and can increase the coverage of an AP. Furthermore,
we design algorithms to optimize ScatterMIMO’s smart surface for
each client with minimal measurement overhead and to overcome
random per-packet phase offsets during the measurement. Our
evaluations show that with commercial off-the-shelf MIMO WiFi
(11ac) AP and unmodified clients, ScatterMIMO provides a median
throughput improvement of 2x over the active AP alone.



<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/scattermimo.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/backscatter/scattermimo_prototype.png" width="100%" style="float: center" > </a>
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

### ScatterMIMO prototype

We hierarchically implement the ScatterMIMO smart surface to
simplify the design and ensure scalability.
Each smart surface can contain multiple tiles, which are coordinated
by a central controller through a UART bus. The central controller
communicated with the ScatterMIMO AP to obtain the appropriate phase information, and deliver them to each tile. Each of the
tiles hosts a matrix of phase-shifted reflecting antennas, or namely,
reflector units.
For our implementation, we put 4×4 = 16 reflector units on each
tile. The 2-dimensional design allows us to steer the reflected beam
both horizontally and vertically. 
The reflector unit uses a patch antenna for maximum reflection.
The antenna is then connected to a HMC7992 5-GHz RF switch,
which further connects to 4 open-ended transmission lines. The
transmission lines provide 0, π/2, π, and 3π/2 round-trip phase
shifts.


<br>



<div class="well">
<h3> <font color="red">Press cover:</font>  </h3>
<h4> 04/02/2020:  <a style="display: inline-block;" href="https://bit.ly/2R3r3vy">UCSD News: WiFi-Boosting ‘Smart Surface’ Could Help Remote Workers and Students</a> </h4>
<h4> 04/10/2020:  <a style="display: inline-block;" href="https://www.hackster.io/news/scattermimo-smart-surface-runs-for-a-year-on-a-button-cell-doubles-wi-fi-speeds-8ea4f374cc59">Hackster News: ScatterMIMO Smart Surface Runs for a Year on a Button Cell, Doubles Wi-Fi Speeds</a> </h4>
</div>

