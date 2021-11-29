---
title: "WCSNG - Research"
layout: gridlay
excerpt: "P2SLAM dataset"
sitemap: true
permalink: /p2slam-datasets/
---

# P2SLAM datasets
```
Authors: Aditya Arun, Roshan Ayyalasomayajula, William Hunter, Dinesh Bharadia
```

---

<div class="well">
 <center>
 <h4><A href="#Envrionment and Results">Environment and Results</A>&emsp;&emsp;<A href="#downloads">Downloads</A>&emsp;&emsp;</h4>
 </center>
</div>


---

## Envrionment and Results ##

### Two Different Environments

Here we describe the environments and the datasets collected in these environments. We further showcase P2SLAM results as compared to camera-based baseline RTABMap. We find that in all datasets inclusion of WiFi-based sensing for localization performs on par with RTABMap and makes a strong case for the inclusion of these simple sensors within SLAM systems. 

<h4> 1.  <b> Env-1: Atkinson Hall 4th Floor </b> -- 20 x 30 m (65 x 100 feet) standard office environment with complex mulitpath and mulitple Non-line of sight conditions. A total of 5 AP's were deployed in this environment.  </h4>
<a href="{{ site.url }}{{ site.baseurl }}/images/respic/env1.jpg"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/env1.jpg" width="100%" style="float: center" > </a>
<p>**channels_atk_ds1** (easy): Simple robot movement where we traverse all the corridors, for a total path length of 330 m (approx) at 18 cm/s. AP's are placed in the locations marked by circles in the above figure. </p>
<a href="{{ site.url }}{{ site.baseurl }}/images/respic/results_ds1.jpg"> <center> <img src="{{ site.url }}{{ site.baseurl }}/images/respic/results_ds1.jpg" width="50%" style="float: center" > </center> </a>
<p>**channels_atk_ds2** (hard): Complex robot movement where the robot traverses different nooks in the environment. This path closely replicate one taken by a vacuume cleaner or package delivery robot. Total path-length travelled is 495 m (approx) at 28 cm/s. AP's are placed in the locations marked by cross in the above figure.</p>
<a href="{{ site.url }}{{ site.baseurl }}/images/respic/results_ds2.jpg"> <center> <img src="{{ site.url }}{{ site.baseurl }}/images/respic/results_ds2.jpg" width="50%" style="float: center" > </center> </a>


<h4> 2. <b> Env-2: Atkinson Hall Ground Floor </b> -- 50 x 40 m large environment covering mulitple corridors and large lobbies and auditorium spaces. </h4>
<a href="{{ site.url }}{{ site.baseurl }}/images/respic/env2.jpg"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/env2.jpg" width="95%" style="float: center" > </a>
<p>**channels_atk_ds3**: Simple robot movement where mulitple corridors are traversed at 28 cm/s for a total path length of 400 m (approx) </p>
<a href="{{ site.url }}{{ site.baseurl }}/images/respic/results_ds3.jpg"> <center> <img src="{{ site.url }}{{ site.baseurl }}/images/respic/results_ds3.jpg" width="50%" style="float: center" > </center> </a>

<p> Finally, we summarize all our results in the following table. We show the median and 90th percentile translation and orientation errors in centimeters and degrees respectively. We show across three sensing modalities -- using odometry only, using odometry + Camera (RTABMap) and using odometry + WiFi (P2SLAM): </p>
<a href="{{ site.url }}{{ site.baseurl }}/images/respic/p2slam_results_table.jpg"> <center> <img src="{{ site.url }}{{ site.baseurl }}/images/respic/p2slam_results_table.jpg" width="70%" style="float: center" > </center> </a>

---

We provide both the CSI data for all the above setups. **All the corresponding links can be found below.**

### Channels

The CSI data is named as **DATASET_NAME.mat** as given above. These MATLAB files are stored using **HDF5** file structure and contain the following variables:

- **channels_cli**: *[ n_datapoints x n_frequency x n_ap x n_rx_ant X n_tx_ant]* 5D complex channel matrix recieved at the WiFi access points deployed in the environment.
- **channels_ap**: *[ n_datapoints x n_frequency x num_aps x n_rx_ant X n_tx_ant]* 5D complex channel matrix recieved at the WiFi access point present on the robot.
- **cli_rssi_synced**: *[ n_datapoints x n_rx_ant x n_ap ]* 2D recieved signal strength matrix at the environments' WiFi access point.
- **ap_rssi_synced**: *[ n_datapoints x n_rx_ant x n_ap ]* 2D recieved signal strength matrix at the robot's WiFi access point.
- **ap**: *[1 x n_ap]* cell matrix. Each element corresponding to *[ n_rx_ant x 2]* antenna positions in th global coordinates.  
- **labels**: *[ n_datapoints x 3 ]* 2D best-estimate ground truth XY labels + heading of the robot -- computed using Cartographer using onboard Lidar and internal odometry.
- **labels_noise**: *[ n_datapoints x 3 ]* 2D XY labels + heading of the robot computed using only robot's wheel encoder (highly erroneous measurements)
- **labels_imu**: *[ n_datapoints x 3 ]* 2D  XY labels + heading of the robot computed using the robot's wheel encoder and internal gyroscope (less erroneous than only using wheel encoders)
- **labels_vel**: *[ n_datapoints x 1 ]* Velocity of the robot in m/s.

---

## Downloads ##

RAL Reviewers, please use the password given in the review-responses document to access these files. The datasets will be open-sourced upon paper's acceptance. 

### Channel Downloads:

Cumulative Downloads: [All channels](https://ucsdcloud-my.sharepoint.com/:f:/g/personal/aarun_ucsd_edu/Ehi2q7tR3ZlHhCamVxFX510ByrEl6aT7aA8n_61d9ToPWQ?e=1RRHLI)

Individual Downloads:
- [channels_atk_ds1](https://ucsdcloud-my.sharepoint.com/:u:/g/personal/aarun_ucsd_edu/EZBHoXwnUGBBgx1X-2G0g-YBpJCzFOyaEhYuwL5SShRNJA?e=3oiN1A)
- [channels_atk_ds2](https://ucsdcloud-my.sharepoint.com/:u:/g/personal/aarun_ucsd_edu/Ef1ETWRODuxEj4RSAV-wlK4BfirvThNOviIqoYJxQalmyg?e=PBCH50)
- [channels_atk_ds3](https://ucsdcloud-my.sharepoint.com/:u:/g/personal/aarun_ucsd_edu/EVPUpb8DFuRBoKW8r7yS7nkBRWXWP9Z03eQcX7O4XydnEg?e=9j93j4)


<!-- #### All the dataset downloads are **PASSWORD** protected. To get the password, please read and agree to the [terms and conditions](https://forms.gle/WWGymUFxhPWRc4zu7). You can then proceed to download datasets from the links above. -->

---
<!-- 
## CITATION ##

- TBA -->

  
