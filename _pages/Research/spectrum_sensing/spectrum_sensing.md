---
title: "WCSNG - Research"
layout: research
excerpt: "WCSNG -- Research"
sitemap: false
permalink: spectrum_sensing.html
---
<!-- <a href="{{ site.url }}{{ site.baseurl }}/research"><img src="{{ site.url }}{{ site.baseurl }}/images/back.png" class="img-responsive" width="4%" /> </a> -->

# Spectrum Sensing
<!-- ####  This page contains papers related to `Spectrum Sensing`. 
#### Go back to other <a href="{{ site.url }}{{ site.baseurl }}/research"> <b>Research</b></a> categories or see full list of <a href="{{ site.url }}{{ site.baseurl }}/publications"> <b>Publications</b></a>. -->

Spectrum usage has evolved over many decades, shaped by both state-of-the art technological progress and the intended use cases. Over the last few years, usage of wireless spectum has become increasingly fragmented and congested. The rapid adoption of new and complex protocols such as LTE and 5G-NR with along with existing legacy systems like FM Radio and Defense wireless deployments have uncovered challenges in spectrum allocation, regulation and monitoring. Adoption of spectrum sharing standards such as CBRS signal a future where
the usage of wireless spectrum needs to be strictly monitored and regulated to maximize utilization while being secure and tolerant to faults. To this end, there is a need of a sensing entity to extract valuable information from the wireless spectrum for a variety of use cases. 

An ideal spectrum sensing entity would have an oracular view of spectrum usage. However, implementing such a system is challenging due to the highly dynamic nature of spectrum usage. These dynamics present themselves in the time domain, as fleeting signals of the order of ms, and in the frequency domain where a multitude of signals and protocols are
crammed into ever-more-congested bandwidth. Added to this, the nature of usage varies from place to place, depending on density of users, terrain and even weather. Our current thrust in this direction is in **designing and building novel spectrum sensing architectures that can scale to next-generation wireless networks** and their requirements. 

Our architecture **SweepSense**, combines sweep-frequency downconversion with simultaneous sampling and achieves **large bandwidth, high-time resolution** sensing. Through our work, we show that **SweepSense** can be implemented on existing radios with minimal cost overheads, and provides promising performance over state-of-art.

<div>
  <a><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/spectrum_sensing/sweepsense_spectrogram.png" width="75%" style="float: center" ></a>
  <br>
  <a href="https://github.com/ucsdsysnet/SweepSense/tree/master"> SweepSense spectrogram of the 2.4 GHz ISM band showing WiFi and Bluetooth transmissions. 100 MHz bandwidth available with only a 25 MSps radio. </a>
</div>

We also investigate orchestration, networking and data management of spectrum sensor deployments. A sensor that can observe large amounts of spectrum will also generate large amounts of data that comes with the cost of backhaul and storage capacity. We show that **powerful spectrum sensors can be deployed on low bandwidth backhaul by
exploiting the sparsity in the spectrum to compress the information captured**. Our algorithm, **SparSDR**, uses **Overlapped Fourier Transform based compression to allow sparsity proportional scaling of backhaul bandwidth**. 


## Publications


<p> &nbsp; </p>
{% assign number_printed = 0 %}
{% for publi in site.data.publist %}
{% if publi.tag1=='spectrum_sensing' or publi.tag2=='spectrum_sensing'  %}

{% assign even_odd = number_printed | modulo: 2 %}


{% if even_odd == 0 %}
<div class="row">
{% endif %}


<div class="col-sm-13 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }} <a href="{{ publi.link.url }}"><span style="color:tomato;">{{ publi.link.display }}</span></a></pubtit>
  <p><strong>
  <a href="{{ publi.website.url }}">{{ publi.website.display }}</a>
  <a href="{{ publi.paper.url }}"><span style="color:#D35400;">{{ publi.paper.display }}</span></a>
  <a href="{{ site.url }}{{ site.baseurl }}/{{ publi.presentation.url }}"><span style="color:#7D3C98;">{{ publi.presentation.display }}</span></a> 
  </strong></p>
  <meta name="publi.keywords.name" content="{{ publi.keywords.content }}">
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="50%" style="float: left" hspace="20" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>


{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}


{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>
