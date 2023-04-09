---
title: "WCSNG - Research"
layout: dlocnewslay
excerpt: "DLoc"
sitemap: false
permalink: /dloc/
---

# Indoor Navigation using Deep Learning
---
### Mobicom 2020
```
Authors: Roshan Ayyalasomayajula, Aditya Arun, Chenfeng Wu, Sanatan Sharma, Abhishek Sethi, Deepak Vasisht, Dinesh Bharadia
```
#### <a href="{{ site.url }}{{ site.baseurl }}/files/dloc.pdf" style="background-color: white; color: #BA4A00;">[Paper]</a> <a href="{{ site.url }}{{ site.baseurl }}/files/DLoc-ppt.pdf" style="background-color: white; color: purple;">[Slides]</a> <a href="https://youtu.be/b19C7U9jNFs">[Video]</a> <a href= "https://wcsng.ucsd.edu/wild" style="color:green">[Datasets]</a> <a href= "https://github.com/ucsdwcsng/DLoc_pt_code" style="color:blue">[Code]</a><a href="https://www.kaggle.com/competitions/wildv2/data"> [Kaggle Competition] </a>

<div class="well">
<h4> WiFi Datasets: </h4>
<h5> 06/20/2020: We released the largest location labelled WiFi CSI dataset, that can be accessed at <a href= "https://wcsng.ucsd.edu/wild">WILD</a> webpage.</h5>
</div>

<iframe width="560" height="315" src="https://www.youtube.com/embed/b19C7U9jNFs" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Motivation
Location services, fundamentally, rely on two components: a mapping system and a positioning system. The mapping system provides the physical map of the space, and the positioning system identifies the position within the map. Outdoor location services have
thrived over the last couple of decades because of well-established
platforms for both these components (e.g. Google Maps for mapping, and GPS for positioning). In contrast, indoor location services
haven’t caught up because of the lack of reliable mapping and positioning frameworks, as GPS is known not to work indoors. Wi-Fi
positioning lacks maps and is also prone to environmental errors.


### Overview 
_**DLoc**_ is a Deep Learning based wireless
localization algorithm that can overcome traditional limitations of
RF-based localization approaches (like multipath, occlusions, etc.).
DLoc uses data from the mapping platform we developed, **_MapFind_**,
that can construct location-tagged maps of the environment. Together, they allow off-the-shelf Wi-Fi devices like smartphones to
access a map of the environment and to estimate their position with
respect to that map. During our evaluation, MapFind has collected
location estimates of over 150 thousand points under 10 different
scenarios across two different spaces covering 2000 sq. Ft. DLoc
outperforms state-of-the-art methods in Wi-Fi-based localization
by 80% (median & 90th percentile) across the 2000 sq. ft. spanning
two different spaces.
<br>
<br>

<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/respic/dloc.png"><img src="{{ site.url }}{{ site.baseurl }}/images/respic/dloc.png" width="90%" style="float: center" > </a>
</div>
<br>


MapFind (left) is an autonomous platform
that maps an indoor environment while collecting wireless channel
data. The platform generates a detailed map of the environment
and collects training data for DLoc. DLoc uses the training data to
learn a model to accurately localize users in the generated map.

<br>
<br>
<br>



***
### DLoc deployment
<div class="row">
<div class="col-sm-3 clearfix">
<p align="left">Once DLoc has been trained using the data collected from MapFind. Any new user entering the environment can use their smartphone to estimate their location with the help of the trained network.</p>
</div>

<div class="col-sm-9 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/user_example.gif"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/user_example_extended.gif" width="70%" style="float: center" > </a>
</div>

---
### MapFind to train DLoc

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/bot_data_collection_medium_slow.gif"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/bot_data_collection_medium_slow.gif" width="100%" style="float: center" > </a>
After the map is generated, MapFind goes around the mapped space in an optimal path pre-determined by our path-planning algorithm so as to cover sufficient space in the provided map as shown above.
</div>

<div class="col-sm-6 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/network_trainig_medium_slow.gif"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/network_trainig_medium_slow.gif" width="100%" style="float: center" > </a>

Simultaneously the server on board the bot collects the CSI information and converts them into the Input heatmaps as shown above. These Input images are then used to train the DLoc network shown above using both L<sub>Location</sub> and L<sub>Consistency</sub> losses. These losses back propogate as shown by the red dotted lines to train DLoc.
</div>

---


## DLoc code and data
While being the first in in Deep Learning based Indoor Navigation with WiFi data, we want to build WiFi CSI dataset on par with [ImageNet](http://www.image-net.org/) to assist further research in WiFi based indoor localization and their applications.

#### Download the <a href= "https://wcsng.ucsd.edu/wild">[Datasets]</a> and the PyTorh implementation of DLoc <a href="https://github.com/ucsdwcsng/DLoc_pt_code">[Codes]</a>




