---
title: "WCSNG - Research"
layout: gridlay
excerpt: "P2SLAM dataset"
sitemap: true
permalink: /viwid/
---

### ViWiD: Leveraging WiFi for Robust and Resource-Efficient SLAM
```
Authors: Aditya Arun, William Hunter, Roshan Ayyalasomayajula, Dinesh Bharadia
```


<div class="well">
 <center>
 <h4><A href="#env"> New Environment Added!</A>&emsp;<A href="#result">In-depth Results</A>&emsp;<A href="#cite">Citation</A> &emsp;<a href="{{ site.url }}{{ site.baseurl }}/files/viwid.pdf" target="_blank"> Paper download [PDF] </a> </h4>
 </center>
</div>

---

<div class="row">
<div class="col-sm-5 clearfix">
<br>
<div class="well">
<h3 id="abstract">Abstract</h3>
<p align="justify">
Recent interest towards autonomous navigation and exploration robots for indoor applications has spurred research into indoor Simultaneous Localization and Mapping (SLAM) robot systems. While most of these SLAM systems use Visual and LiDAR sensors in tandem with an odometry sensor, these odometry sensors drift over time. To combat this drift, Visual SLAM systems deploy compute and memory intensive search algorithms to detect `Loop Closures', which make the trajectory estimate globally consistent. To circumvent these resource (compute and memory) intensive algorithms, we present ViWiD, which integrates WiFi and Visual sensors in a dual-layered system. This dual-layered approach separates the tasks of local and global trajectory estimation making ViWiD resource efficient while achieving on-par or better performance to state-of-the-art Visual SLAM. We demonstrate ViWiD's performance on four datasets, covering over 1500 m of traversed path and show 4.3x and 4x reduction in compute and memory consumption respectively compared to state-of-the-art Visual and Lidar SLAM systems with on par SLAM performance. 
</p>
</div>
<br>
</div>

<div class="col-sm-7 clearfix">
<h3 id="idea">High-level idea</h3>

The core idea of ViWiD is to consider WiFi access points, deployed in the envrionment, as unique landmarks which can be leveraged to correct for drifts in the robot's trajectory. A visualization of new AP's discovered and added in an envrionment and appropriate corrections made to the trajectory, is provided under [Quick Results](#result). However, fusing new sensors in an existing SLAM system can be challenging, hence we provide a dual graph approach, where the inputs from any SLAM algorithm can be provided to the ViWiD ROS node for trajectory corrections. Consequently, ViWiD stands for Visual-WiFi dual graph and the above figure showcases a this process block diagram.

<a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/viwid.png"><center><img class="img-responsive"  src="{{ site.url }}{{ site.baseurl }}/images/pubpic/viwid.png" width="100%" style="float:center" ></center> </a>

</div>
</div>

---
<h3 id="env">New Envrionment Added to [P2SLAM]({{ site.url }}{{ site.baseurl }}/p2slam/#env) datasets!</h3>

<br>
<p align="justify"> 
  In addition to the environment described in P2SLAM, we have collected a new dataset in an office envrionment, with stereo camera data, IMU, Lidar, Wheel odometry and WiFi measurements. The purple box and orange boxes indicate the robot and the AP's placed in the environment respectively. The colored boxes in the map correspond to the view points of the 3 images of the environment shown, color-matched to the edges of the respective images. The bag file for this dataset can be downloaded [here](TODO). 
  <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/viwid-env.png"><center><img class="hiddenImage" src="{{ site.url }}{{ site.baseurl }}/images/pubpic/viwid-env.png" width="100%" style="float:center" ></center> </a> <br>

</p>
<br>

---
<h3 id="result">Quick Results</h3>
<div class="row">
  <div class="col-sm-6 clearfix">
  <h4>Real-time operation</h4>
  The following videos provide high level results of running ViWiD on the P2SLAM datasets and the above new dataset (ViWiD dataset). 

  <iframe width="100%" height="267" src="https://www.youtube.com/embed/xL3AP-ne_NQ" title="Viwid: Leveraging WiFi for Robust and Resource-Efficient SLAM - Part 1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
  <iframe width="100%" height="267" src="https://www.youtube.com/embed/M6ZDygSaq5M" title="ViWiD: Leveraging WiFi for Robust and Resource-Efficient SLAM - Part 2" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
  </div>

  <div class="col-sm-6 clearfix">
  <h4>Memory and compute efficiency</h4>

  The primary deliverable of ViWiD is to reduce the memory and compute consumption of SLAM algorithms. By leveraging WiFi landmarks, we observe that we can remove the need for a loop-closure module. This provides over 3x improvement in memory and 1.5x improvement in compute when relying on Visual SLAM systems. More details are available in the paper, however, the key memory and compute improvement result is showcased below. 
  <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/viwid-mem-cpu .png"><center><img class="hiddenImage" src="{{ site.url }}{{ site.baseurl }}/images/pubpic/viwid-mem-cpu.png" width="100%" style="float:center" ></center> </a> <br>
  Timeseries of memory (left) and CPU consumption (right) of VIO, Kimera and ViWiD + VIO are shown. The resource consumption of the ViWiD’s WiFi graph is also analysed (Wifi only) 
  


  </div>
</div>

<!-- Results table -->

---

<br>
<h3 id="cite">Citation</h3>
If you found our work useful, please cite the project as :

@article{arun2022viwid, <br>
  title={ViWiD: Leveraging WiFi for Robust and Resource-Efficient SLAM}, <br>
  author={Arun, Aditya and Hunter, William and Ayyalasomayajula, Roshan and Bharadia, Dinesh}, <br>
  journal={arXiv preprint arXiv:2209.08091}, <br>
  year={2022} <br>
}
