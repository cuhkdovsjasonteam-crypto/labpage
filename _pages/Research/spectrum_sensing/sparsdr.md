---
title: "WCSNG - Research"
layout: gridlay
excerpt: "SparSDR"
sitemap: false
permalink: /sparsdr/
---

# SparSDR: Sparsity-proportional Backhaul and Compute for SDRs
---
### Mobisys'19
```
Authors: Moein Khazraee, Yeswanth Guddeti, Sam Crow, Alex C. Snoeren, Kirill Levchenko, Dinesh Bharadia, Aaron Schulman
```


#### <a href="http://people.csail.mit.edu/moein/papers/sparsdr-mobisys19.pdf" style="background-color: white; color: #BA4A00;">[Paper]</a> <a href="https://youtu.be/019AI3Q0s4g" style="background-color: white; color: blue;">[Video]</a> <a href="https://github.com/ucsdsysnet/sparsdr" style="background-color: white; color: blue;">[Repository]</a>

<iframe width="560" height="315" src="https://www.youtube.com/embed/019AI3Q0s4g" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Summary

We present SparSDR, a resource-efficient architecture for softwaredefined radios whose backhaul bandwidth and compute power requirements scale in inverse proportion to the sparsity (in time and frequency) of the signals received. SparSDR requires dramatically fewer resources than existing approaches to process many popular protocols while retaining both flexibility and fidelity. We demonstrate that our approach has negligible impact on signal quality, receiver sensitivity, and processing latency. The SparSDR architecture makes it possible to capture signals across bandwidths far wider than the capacity of a radio's backhaul through the addition of lightweight frontend processing and corresponding backend reconstruction to restore the signals to their original sample rate. We employ SparSDR to develop two wideband applications running on a USRP N210 and a Raspberry Pi 3+: an IoT sniffer that scans 100 MHz of bandwidth and decodes received BLE packets, and a wideband Cloud SDR receiver that requires only residential-class Internet uplink capacity. We show that our SparSDR implementation fits in the constrained resources of popular low-cost SDR platforms, such as the AD Pluto.


<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/sparSDR.png.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/sparSDR.png" width="80%" style="float: center" > </a>
</div>
<br>


 SparSDR’s goal is to make SDRs capture primary transmissions rather than entire channels. While a Full-capture SDR always backhauls data at a fixed rate, SparSDR takes advantage of frequency-time signal sparsity to scale the backhaul rate linearly with the actual occupancy of the channels observed. This allows SparSDR to backhaul more than 100 MHz of bandwidth over a backhaul where a Full-capture SDR could do less than 25 MHz.

<br>
<br>
<br>
<br>
<br>
<br>

<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/sparsdr_result.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/sparsdr_result.png" width="80%" style="float: center" > </a>
</div>

We show that the backhaul data rate and CPU usage on a Raspberry PI 3 scales linearly with the rate of BLE advertisement packets within the entire 2.4 GHz ISM band. The rate of advertisement packets directly corresponds to spectrum utilization in this experiment. Such a linear scaling of processing allows for low-power, low-cost hardware to be deployed at the edge of networks in order to agreggate sparse wideband traffic or for spectrum sensing.

<br>
<br>
<br>
<br>

***


#### See similar papers: <a href="https://github.com/ucsdsysnet/SweepSense" style="background-color: white; color: blue;">SweepSense: Sensing 5 GHz in 5 ms with Low-cost Radios</a>
