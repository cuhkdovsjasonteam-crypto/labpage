---
title: "WCSNG - Research"
layout: gridlay
excerpt: "P2SLAM dataset"
sitemap: true
permalink: /p2slam/
---

# P2SLAM datasets
```
Authors: Aditya Arun, Roshan Ayyalasomayajula, William Hunter, Dinesh Bharadia
```

---

<div class="well">
 <center>
 <h4><A href="#env">Environment Description</A>&emsp;<A href="#result">In-depth Results</A>&emsp;<A href="#swapc">SWaP-C Analysis</A>&emsp;<A href="#usage"> Dataset Usage </A>&emsp;<a href="https://ucsdcloud-my.sharepoint.com/:u:/g/personal/aarun_ucsd_edu/ERBGyYIWBTtBhT_phoQzWf4BBoWPPAbpQN36DHhzCWy10Q?e=KMY3lO"> Download (size: 28GB) </a></h4>
 </center>
</div>


---

<h3 id="env">Envrionment Description</h3>

Here we describe the environments and the datasets collected in these environments. We further showcase P2SLAM results as compared to camera-based baseline RTABMap. We find that in all datasets inclusion of WiFi-based sensing for localization performs on par with RTABMap and makes a strong case for the inclusion of these simple sensors within SLAM systems. 

1.  <b> Env-1: Atkinson Hall 4th Floor </b> -- 20 x 30 m (65 x 100 feet) standard office environment with complex mulitpath and mulitple Non-line of sight conditions. A total of 5 AP's were deployed in this environment and two paths (<i> Dataset 1 </i> and <i> Dataset 2 </i>) were taken as described below.
<a href="{{ site.url }}{{ site.baseurl }}/images/respic/env1.jpg"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/env1.jpg" width="100%" style="float: center" > </a>

2. <b> Env-2: Atkinson Hall Ground Floor </b> -- 50 x 40 m large environment covering mulitple corridors and large lobbies and auditorium spaces. <i> Dataset 3 </i> was collected in this environment.
<a href="{{ site.url }}{{ site.baseurl }}/images/respic/env2.jpg"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/env2.jpg" width="95%" style="float: center" > </a>

<p> First, we summarize all our results in the following table. We show the median and 90th percentile translation and orientation errors in centimeters and degrees respectively. We show across three sensing modalities -- using odometry only, using odometry + Camera (RTABMap) and using odometry + WiFi (P2SLAM): </p>
<a href="{{ site.url }}{{ site.baseurl }}/images/respic/p2slam_results_table.jpg"> <center> <img src="{{ site.url }}{{ site.baseurl }}/images/respic/p2slam_results_table.jpg" width="70%" style="float: center" > </center> </a>

---


<h3 id="result">In-depth Results</h3>


Next, we present in-depth analysis for the above three datasets. These datasets can be downloaded [here (size: 28GB)](https://ucsdcloud-my.sharepoint.com/:u:/g/personal/aarun_ucsd_edu/ERBGyYIWBTtBhT_phoQzWf4BBoWPPAbpQN36DHhzCWy10Q?e=KMY3lO)
<!-- These datasets can be downloaded [here](https://ucsdcloud-my.sharepoint.com/:f:/g/personal/aarun_ucsd_edu/Ehi2q7tR3ZlHhCamVxFX510ByrEl6aT7aA8n_61d9ToPWQ?e=1RRHLI).  -->
Further details to use this dataset is given below. 

<b> NOTE: RAL Reviewers, please use the password given in the review-responses document to access these files. The datasets will be open-sourced upon paper's acceptance. </b>


1. <b> Env 1 - Dataset 1 </b> (easy): Simple robot movement where we traverse all the corridors, for a total path length of 330 m (approx) at 18 cm/s. AP's are placed in the locations marked by circles in the above figure. 
<!-- Download the dataset .mat file [here](https://ucsdcloud-my.sharepoint.com/:u:/g/personal/aarun_ucsd_edu/EZBHoXwnUGBBgx1X-2G0g-YBpJCzFOyaEhYuwL5SShRNJA?e=3oiN1A). -->
<a href="{{ site.url }}{{ site.baseurl }}/images/respic/results_ds1.jpg"> <center> <img src="{{ site.url }}{{ site.baseurl }}/images/respic/results_ds1.jpg" width="50%" style="float: center" > </center> </a>

2. <b> Env 1 - Dataset 2 </b> (hard): Complex robot movement where the robot traverses different nooks in the environment. This path closely replicate one taken by a vacuume cleaner or package delivery robot. Total path-length travelled is 495 m (approx) at 28 cm/s. AP's are placed in the locations marked by cross in the above figure. 
<!-- Download the dataset .mat file [here](https://ucsdcloud-my.sharepoint.com/:u:/g/personal/aarun_ucsd_edu/Ef1ETWRODuxEj4RSAV-wlK4BfirvThNOviIqoYJxQalmyg?e=PBCH50). -->
<a href="{{ site.url }}{{ site.baseurl }}/images/respic/results_ds2.jpg"> <center> <img src="{{ site.url }}{{ site.baseurl }}/images/respic/results_ds2.jpg" width="50%" style="float: center" > </center> </a>

3. <b> Env 2 - Dataset 3 </b>: Simple robot movement where mulitple corridors are traversed at 28 cm/s for a total path length of 400 m (approx). 
<!-- Download the dataset .mat file [here](https://ucsdcloud-my.sharepoint.com/:u:/g/personal/aarun_ucsd_edu/EVPUpb8DFuRBoKW8r7yS7nkBRWXWP9Z03eQcX7O4XydnEg?e=9j93j4). -->
<a href="{{ site.url }}{{ site.baseurl }}/images/respic/results_ds3.jpg"> <center> <img src="{{ site.url }}{{ site.baseurl }}/images/respic/results_ds3.jpg" width="50%" style="float: center" > </center> </a>

---

<h3 id="swapc">SWaP-C Analysis</h3>

SWaP-C is a common industry acronym for Size, Weight, Power and Cost. In P2SLAM, we show the efficacy of WiFi-based sensing for robotic localization and navigation. Furthermore, we claim that the SWaP-C metrics for WiFi radios is 10 times better than LiDAR's. Here we further justify this claim. 

<h4> Size </h4>

The smallest surround LIDAR, [Puck Lite](https://www.mapix.com/wp-content/uploads/2018/07/63-9286_Rev-H_Puck-LITE_Datasheet_Web.pdf) by Velodyne Lidar, has a very small form factor with a 3.5" diameter and height of 2.82". 

Developing a WiFi sensor using the [ESP8266 NodeMCU](https://www.nodemcu.com/index_en.html) with multi-antenna capability will have dimensions of (2" x 1" x 0.5"), with the size of an 4-element linear antenna array at 9.8" or a square antenna array at 6.25". 

<h4> Weight </h4>

The Puck Lite weighs at 590 g. An ESP8266-based design would weight a meagre 9 g. 

<h4> Power </h4>

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-ce78{background-color:#c0c0c0;border-color:inherit;font-size:100%;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-f35e{background-color:#c0c0c0;border-color:inherit;font-size:100%;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-7btt{border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-fymr{border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-ce78">Device</th>
    <th class="tg-ce78">Power Consumption</th>
    <th class="tg-f35e">Notes</th>
    <th class="tg-f35e">Sources</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow">Hokoyo Lidar</td>
    <td class="tg-c3ow">8.4 W</td>
    <td class="tg-0pky">Single channel</td>
    <td class="tg-0pky"><a href="https://autonomoustuff.com/-/media/Images/Hexagon/Hexagon%20Core/autonomousstuff/pdf/hokuyo-utm-30lx-datasheet.ashx?la=en&hash=E1F8A1F837A229BD9EB3FEC17DD3488F" target="_blank" rel="noopener noreferrer">Datasheet</a></td>
  </tr>
  <tr>
    <td class="tg-7btt">Velodyne Puck</td>
    <td class="tg-7btt">8 W</td>
    <td class="tg-fymr">16 channel</td>
    <td class="tg-fymr"><a href="https://www.mapix.com/wp-content/uploads/2018/07/63-9286_Rev-H_Puck-LITE_Datasheet_Web.pdf" target="_blank" rel="noopener noreferrer">Datasheet</a></td>
  </tr>
  <tr>
    <td class="tg-c3ow">ASUS RT-AC86U</td>
    <td class="tg-c3ow">Measured @ 6.5 W in lab</td>
    <td class="tg-0pky">802.11AC, 5 Ghz, 20/40/80 MHz, 4x4</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-c3ow">Quantenna </td>
    <td class="tg-c3ow">Measured @ 3.2 W in lab</td>
    <td class="tg-0pky">802.11AC, 5 Ghz, 20/40/80 MHz,  4x4</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-c3ow">Intel 5300</td>
    <td class="tg-c3ow">1.6 W Rx, 2.1 W Tx</td>
    <td class="tg-0pky">802.11n, 2.4 Ghz, 20 and 40 MHz, <br>3x3</td>
    <td class="tg-0pky"><a href="https://www.usenix.org/legacy/events/hotpower/tech/full_papers/Halperin.pdf" target="_blank" rel="noopener noreferrer">Power measurements by Halperin et al.</a></td>
  </tr>
  <tr>
    <td class="tg-c3ow">TP-Link TL-WDR4300<br>(Atheros CSI tool)</td>
    <td class="tg-c3ow">4.6 W</td>
    <td class="tg-0pky">IEEE 802.11n, 2.4 GHz, 20/40 MHz, 3x3 </td>
    <td class="tg-0pky">Power consumption database</td>
  </tr>
  <tr>
    <td class="tg-7btt">ESP 32, NodeMCU</td>
    <td class="tg-7btt">240 mW x 4 ~ 1 W</td>
    <td class="tg-fymr">802.11 b/g/n, 2.4 GHz, 20 MHz</td>
    <td class="tg-fymr">Measurement by JeeLabs</td>
  </tr>
</tbody>
</table>

From the above table, we can see that taking a conservative power estimate of the NodeMCU, we find the power consumption to be close to 1 W, which is about 8 times lower than the Velodyne Puck Lite. 

<h4> Cost </h4>

Publicly available information about the Velodyne Puck prices the it at $8000. A simple NodeMCU WiFi sensor would cost less than $20. 

---

<h3 id="usage">Dataset Usage</h3>


The CSI data is named as **channels.mat** and the rosbag is named as **data.bag** in the resepctive dataset folders. All the datasets can be downloaded [here (size: 28GB)](https://ucsdcloud-my.sharepoint.com/:u:/g/personal/aarun_ucsd_edu/ERBGyYIWBTtBhT_phoQzWf4BBoWPPAbpQN36DHhzCWy10Q?e=KMY3lO):

The MATLAB files are stored using **HDF5** file structure and contain the following variables:
- **channels_cli**: *[ n_datapoints x n_frequency x n_ap x n_rx_ant X n_tx_ant]* 5D complex channel matrix recieved at the WiFi access points deployed in the environment.
- **channels_ap**: *[ n_datapoints x n_frequency x num_aps x n_rx_ant X n_tx_ant]* 5D complex channel matrix recieved at the WiFi access point present on the robot.
- **cli_rssi_synced**: *[ n_datapoints x n_rx_ant x n_ap ]* Recieved signal strength matrix at the environments' WiFi access point.
- **ap_rssi_synced**: *[ n_datapoints x n_rx_ant x n_ap ]* Recieved signal strength matrix at the robot's WiFi access point.
- **cli_hw_noise_synced**: *[ n_datapoints x n_ap ]* Hardware noise floor measured at the Environment's AP's when signal is received from the robot.
- **ap_hw_noise_synced**: *[ n_datapoints x n_ap ]* Hardware noise floor measured at robot' WiFi AP with signal received from each of the environment's AP's.
- **ap**: *[1 x n_ap]* cell matrix. Each element corresponding to *[ n_rx_ant x 2]* antenna positions in th global coordinates.  
- **labels**: *[ n_datapoints x 3 ]* 2D best-estimate ground truth XY labels + heading of the robot -- computed using Cartographer using onboard Lidar and internal odometry.
- **labels_noise**: *[ n_datapoints x 3 ]* 2D XY labels + heading of the robot computed using only robot's wheel encoder (highly erroneous measurements)
- **labels_imu**: *[ n_datapoints x 3 ]* 2D  XY labels + heading of the robot computed using the robot's wheel encoder and internal gyroscope (less erroneous than only using wheel encoders)
- **labels_vel**: *[ n_datapoints x 1 ]* Velocity of the robot in m/s.

The rosbags contain the following topics:

1. Camera Information from Intel Realsense D415:
- /camera/rgb/camera_info
- /camera/depth_registered/image_raw/compressedDepth
- /camera/rgb/image_rect_color/compressed

2. Odometry Information from Turtlebot base:
- /mobile_base/sensors/core
- /mobile_base/sensors/imu_data
- /mobile_base/sensors/imu_data_raw
- /odom
/tf

3. Hokuoyo Lidar scan information:
- /scan





<!-- ## Downloads ##
 -->

<!-- ### Channel Downloads:


Individual Downloads:
- [channels_atk_ds1](https://ucsdcloud-my.sharepoint.com/:u:/g/personal/aarun_ucsd_edu/EZBHoXwnUGBBgx1X-2G0g-YBpJCzFOyaEhYuwL5SShRNJA?e=3oiN1A)
- [channels_atk_ds2](https://ucsdcloud-my.sharepoint.com/:u:/g/personal/aarun_ucsd_edu/Ef1ETWRODuxEj4RSAV-wlK4BfirvThNOviIqoYJxQalmyg?e=PBCH50)
- [channels_atk_ds3](https://ucsdcloud-my.sharepoint.com/:u:/g/personal/aarun_ucsd_edu/EVPUpb8DFuRBoKW8r7yS7nkBRWXWP9Z03eQcX7O4XydnEg?e=9j93j4)
 -->

<!-- #### All the dataset downloads are **PASSWORD** protected. To get the password, please read and agree to the [terms and conditions](https://forms.gle/WWGymUFxhPWRc4zu7). You can then proceed to download datasets from the links above. -->

<!-- 
## CITATION ##

- TBA -->

  
