---
title: "WCSNG - Research"
layout: gridlay
excerpt: "mMobile"
sitemap: false
permalink: /mmobile/
---

# mMobile: Building a mmWave Testbed to Evaluate and Address Mobility Effects
---
### mmNets 2020 Workshop (with Mobicom)
```
Authors: Ish Kumar Jain, Raghav Subbaraman, Tejas Harekrishna Sadarahalli, Xiangwei Shao, Hou-Wei Lin, Dinesh Bharadia
```
#### <a href="{{ site.url }}{{ site.baseurl }}/files/mmobile.pdf" style="background-color: white; color: #BA4A00;">[Paper]</a> <a href="{{ site.url }}{{ site.baseurl }}/files/mMobile_slides.pdf" style=" color: purple;">[Slides]</a> <a href="https://youtu.be/5vfE90wR03Q">[Video]</a> <a href="https://github.com/ucsdwcsng/mMobile" style="background-color: white; color: green;">[Datasets]</a>

<iframe width="560" height="315" src="https://www.youtube.com/embed/5vfE90wR03Q" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<div class="well">
<h3> 5G user mobility Datasets News: </h3>
<h5> Sept 2020: We release channel (CSI) measurements data collected from our mMobile testbed to encourage development and verification of novel mobility management algorithms for 5G New radio <a href="https://github.com/ucsdwcsng/mMobile" style="background-color: white; color: green;">[Datasets]</a></h5>
</div>


### Abstract
Beamforming methods need to be critically evaluated and improved to achieve the promised performance of millimeter wave (mmWave) 5G NR in high mobility applications like Vehicle-to-Everything (V2X) communication. Conventional beam management methods developed for higher frequency applications do not directly carry over to the 28 GHz mmWave regime, where propagation and reflection characteristics are vastly different. Further, real system deployments and tests are required to verify these methods in a practical setting. In this work, we develop mMobile, a custom 5G NR compliant mmWave testbed to evaluate beam management algorithms. We describe the architecture and challenges in building such a testbed. We then create a novel, low-complexity beam tracking algorithm by exploiting the 5G NR waveform structure and evaluate its performance on the testbed. The algorithm can sustain almost twice the average throughput compared to the baseline.


<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/5G/mMobile_testbed.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/5G/mMobile_testbed.png" width="90%" style="float: center" > </a>
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
### Testbed Architecture
We show that mMobile is well designed and can support 5G NR specifications. We established a link with 240 kHz subcarrier spacing with a bandwidth of 50 MHz. The radiated transmit power is fixed to an EIRP of 30 dBm. We demonstrate that \name can support a high throughput link with up to 256-QAM constellation with the bit error rate as low as 0.0022 without channel coding. We have also verified that our FPGA baseband platform can be used as gNB with high bandwidth of 400 MHz required for 5G NR. Finally, we show that our phased array module can produce the desired beam patterns when measured in an anechoic chamber.


<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/5G/mMobile_256qam_beampatterns.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/5G/mMobile_256qam_beampatterns.png" width="70%" style="float: center" > </a>
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



## mMobile 5G user mobility dataset
### Motivation
The access to such a testbed is generally out-of-reach to a large research community. To allow the large research community to test and verify novel algorithms for 5G NR mobility management, we release one-of-its-kind mobility dataset. We build the dataset of channel measurements with two important goals. First, it should allow the testing of algorithms based on 5G-NR specific features such as the SSB and CSI-RS. Second, it should easily allow other testbeds to collect and publish similar measurements. We envision this dataset will be useful for testing any new algorithm for mmWave user tracking and mobility management. The dataset is catered to meet these requirements. We plan to continuously add more experiments. 


### Description of the dataset
We relese 28 GHz full channel (CSI) measurements for a mobile user. The CSI data is tagged with each user location and for each beam index. The CSI consists of 256 subcarriers with a sub-carrier spacing of 240 kHz requisite by 5G NR standards. There are four datasets for various indoor and outdoor environments.

#### <a href="https://github.com/ucsdwcsng/mMobile" style="background-color: white;"> Download the datasets and code</a>


|` Setting`   | `Link-Length` | `Moving-Direction` | `Resolution` | `#points` | `Blockage `     |
|:---------:|:-----:|:---------:|:-------:|:-------:|:------------:|
| Indoor  | 2\.5m   | 90 degree    | 0\.1m   | 21      | No |
| Indoor  | 4\.2m   | 90 degree   | 0\.1m   | 32      | No |
| Outdoor | 10m     | 90 degree   | 0\.2m   | 31      | No |
| Outdoor | 30m     | 120 degree   | 0\.6m   | 45      | Yes |

<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/5G/mMobile_results.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/5G/mMobile_results.png" width="70%" style="float: center" > </a>
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


### Cite the dataset
Ish Kumar Jain, Raghav Subbaraman, Tejas Harekrishna Sadarahalli, Xiangwei Shao, Hou-Wei Lin, Dinesh Bharadia. 2020. mMobile: Building a
mmWave Testbed to Evaluate and Address Mobility Effects. In 4th ACM
Workshop on Millimeter-Wave Networks and Sensing Systems (mmNets’20),
September 25, 2020, London, United Kingdom. ACM, New York, NY, USA,
6 pages. https://doi.org/10.1145/3412060.3418433





