---
title: "WCSNG - Research"
layout: gridlay
excerpt: "P2SLAM dataset"
sitemap: true
permalink: /wiros/
---

### WiROS: WiFi sensing toolbox for robotics
```
Authors: William Hunter*, Aditya Arun*, Dinesh Bharadia
*Equal contribution
```


<div class="well">
 <center>
 <h4><A href="#demo"> Demo Video</A>&emsp;<A href="#working"> Process block-diagram </A>&emsp;<A href="https://github.com/ucsdwcsng/WiROS" target="_blank">GitHub</A>&emsp;<A href="#cite">Citation</A> &emsp;<a href="TODO" target="_blank"> Paper download [PDF] </a> </h4>
 </center>
</div>

---

<div class="row">
<div class="col-sm-5 clearfix">
<br>
<div class="well">
<h3 id="abstract">Abstract</h3>
<p align="justify">
  Many recent works have explored using WiFi-based sensing to improve SLAM, robot manipulation or exploration. Moreover, widespread availability makes WiFi the most advantageous RF signal to leverage. But WiFi sensors lack an accurate, tractable, and versatile toolbox, which hinders their widespread adoption with robot's sensor stacks. 

  We develop WiROS to address this immediate need, furnishing many WiFi-related measurements as easy-to-consume ROS topics. Specifically, WiROS is a plug-and-play WiFi sensing toolbox providing access to coarse-grained WiFi signal strength (RSSI), fine-grained WiFi channel state information (CSI), and other MAC-layer information (device address, packet id's or frequency-channel information). Additionally, WiROS open-sources state-of-art algorithms to calibrate and process WiFi measurements to furnish accurate bearing information for received WiFi signals. The open-sourced repository is [here](https://github.com/ucsdwcsng/WiROS). 
</p>
</div>
<br>
</div>

<div class="col-sm-7 clearfix">
<h3 id="idea">High-level idea</h3>

WiROS makes three concrete contributions, in order to deliver an accurate, versatile and tractable WiFi-sensor framework for ROS. First, it provides a C++ framework to integrate WiFi-sensor specific API's into ROS. We accomplish this for [Nexmon API](https://github.com/IMDEANetworksWNG/UbiLocate), however, newer platforms can be similarly integrated with little additional effort. Second, we provide a wireless calibration algorithm and toolkit to measure and calibrate for hardware non-idealities for WiFi sensors. The lastly, we open-source state-of-art algorithms to extract physical parameters like angles of arrival or departure of the WiFi signals.  

<a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/wiros.jpg"><center><img class="img-responsive"  src="{{ site.url }}{{ site.baseurl }}/images/pubpic/wiros.jpg" width="100%" style="float:center" ></center> </a>

</div>
</div>

---
<h3 id="demo">Demo Video of WiROS in action</h3>

<br>
<p align="justify"> 
  The following video provides a  visualization of WiROS in action and a simple case-study of a robot deployed with WiROS sensor discovering and localizing IoT devices in an environment.  
</p>
<br>

<iframe width="100%" height="640" src="https://www.youtube.com/embed/zYAshWFn75k" title="IPSN 2023 Demo: Accessible WiFi sensing leveraging Robot Operating System" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---

<h3 id="working">WiROS Process Block Diagram</h3>

<br>
<p align="justify"> 
The following figure showcases the two main blocks - CSI Node and Feature-extraction Node to extract raw WiFi measurements and to calibrate and process these measurements. The blue text indicates the control plane parameters, whereas the red text indicates the exposed measurements. WiROS extends the functionality of the underlying black box `CSI Extraction Toolkit.</p>
<br>

<a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/wiros-block.png"><center><img class="img-responsive"  src="{{ site.url }}{{ site.baseurl }}/images/pubpic/wiros-block.png" width="100%" style="float:center" ></center> </a>

---

<br>
<h3 id="cite">Citation</h3>
If you found our work useful, please cite the project as :

TBA

