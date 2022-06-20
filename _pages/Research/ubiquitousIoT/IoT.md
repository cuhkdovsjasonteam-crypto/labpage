---
title: "WCSNG - Research"
layout: gridlay
excerpt: "WCSNG -- UbiquitousIoT"
sitemap: false
permalink: /ubiquitousIoT/
---

# Hitchhike : Enabling Low Power IoT on WiFi networks  
---

## Backscatter communication
<div class="row">
<div class="col-sm-4 clearfix">
<br>
<p align="justify"> RF signal generation is expensive and takes a lot of power. Hitchhike tackles this problem by recycling the ambient RF signals to embed the data from an IoT device. </p>
</div>

<div class="col-sm-8 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/hitchhike.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/hitchhike.png" width="70%" style="float: center" > </a>
</div>
</div>

---
### Codeword translation

<div class="row">

<div class="col-sm-5 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/codewordtranslation.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/codewordtranslation.png" width="90%" style="float: center" > </a>
Hitchhike enables co-existence of IoT devices along with the user traffic on a Wifi network. It uses a novel technique called "Codeword translation" to embed data onto an existing wifi packet. 
</div>

### Prototype hardware and applications
<div class="col-sm-7 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/Hitchhike_prototype.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/Hitchhike_prototype.png" width="90%" style="float: center" > </a>
Hitchhike's hardware prototype consumes ~30uW of power. At this level of power consumption makes, an AA battery can last upto 15 years. The large shelf life of the tag makes it ideal for vast deployment of sensors in agricultural fields for moisture and temperature monitoring.   
</div>
</div>
<br>

---
## Hierarchical Wake-up receiver
<div class="row">
<div class="col-sm-6 clearfix">
<br>
<p align="justify"> We have developed a novel hierarchical wake-up receiver for backscatter tags to synchronize with incident signals. Traditional backscatter tags suffer from loss of synchronization resulting in lot of bit errors and limit the tag placement close to the transmitter. Here we demonstrate a wake-up receiver to enable synchronization at the tag at a very low power and increase the tag's working range. </p>
</div>

<div class="col-sm-6 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/syncscatter.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/syncscatter.png" width="100%" style="float: center" > </a>
</div>
</div>
---
## Publications

<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="{{ site.url }}{{ site.baseurl }}/files/WiFi_BLE_combo_ISSCC2022.pdf">A WiFi and Bluetooth Backscattering Combo Chip Featuring Beam Steering via a Fully-Reflective Phased-Controlled Multi-Antenna Termination Technique Enabling Operation Over 56 Meters</a> <a style="background-color: white; color: blue;" href="{{ site.url }}{{ site.baseurl }}/files/ISSCC2022_slides.pdf">[Slides]</a><br>
    Shihkai Kuo, Manideep Dunna, Patrick Mercier, Dinesh Bharadia<br>
    ISSCC 2022 
</div>
</div>

<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="{{ site.url }}{{ site.baseurl }}/files/syncscatter.pdf">SyncScatter: Enabling WiFi like synchronization and range for WiFi backscatter Communication</a> <a style="background-color: white; color: blue;" href="{{ site.url }}{{ site.baseurl }}/files/nsdi21_slides_dunna.pdf">[Slides]</a><br>
    Manideep Dunna, Miao Meng, Pohan Peter Wang, Chi Zhang, Patrick Mercier, Dinesh Bharadia<br>
    NSDI 2021 
</div>
</div>

<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="{{ site.url }}{{ site.baseurl }}/files/ISSCC_2021.pdf">Improving the Range of WiFi Backscatter Via a Passive Retro-Reflective Single-Side-Band-Modulating MIMO Array and Non-Absorbing Termination</a> <a style="background-color: white; color: blue;" href="{{ site.url }}{{ site.baseurl }}/files/Meng_Backscatter_ISSCC2021.pdf">[Slides]</a><br>
    Miao Meng, Manideep Dunna, Hans Yu, Shikhai Kuo, Pohan Peter Wang, Dinesh Bharadia, Patrick Mercier<br>
    ISSCC 2021 
</div>
</div>

<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="{{ site.url }}{{ site.baseurl }}/files/JSSC_2020.pdf">A Low-Power Backscatter Modulation System Communicating Across Tens of Meters With Standards-Compliant Wi-Fi Transceivers</a>
<br>Po-Han Peter Wang, Chi Zhang, Hongsen Yang, Manideep Dunna, Dinesh Bharadia, Patrick Mercier<br>
    JSSC 2020 
</div>
</div>

<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="{{ site.url }}{{ site.baseurl }}/files/ISSCC_paper.pdf">A 28µW IoT Tag That Can Communicate with Commodity WiFi Transceivers via a Single-Side-Band QPSK Backscatter Communication Technique</a> <a style="background-color: white; color: blue;" href="{{ site.url }}{{ site.baseurl }}/files/ISSCC-talk.pdf">[Slides]</a><br>
    Po-Han Peter Wang, Chi Zhang, Hongsen Yang, Dinesh Bharadia, Patrick Mercier<br>
    ISSCC 2020<br>
    <font color="red">Press cover:</font> 
    <a style="display: inline-block;" href="https://ucsdnews.ucsd.edu/pressrelease/new-chip-brings-ultra-low-power-wi-fi-connectivity-to-iot-devices">UCSD News</a>, 
    <a style="display: inline-block;" href="https://www.techexplorist.com/ultra-low-power-wi-fi-chip-iot-devices-5000-times-less-power/30328/">Tech Explorist</a>,
    <a style="display: : inline-block;" href = "https://cacm.acm.org/news/243008-chip-brings-ultra-low-power-wi-fi-to-iot-devices/fulltext">ACM News</a>,
    <a style="display: : inline-block;" href="https://news.ycombinator.com/item?id=22427511">Hacker News</a>  
</div>
</div>

<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="{{ site.url }}{{ site.baseurl }}/ffiles/freerider.pdf">FreeRider: Backscatter Communication Using Commodity Radios</a> <a style="background-color: white; color: blue;" href="{{ site.url }}{{ site.baseurl }}/files/FreeRiderSlides.pdf">[Slides]</a><br>
    Pengyu Zhang, Colleen Josephson, Dinesh Bharadia, Sachin Katti<br>
    CoNEXT 2017
</div>
</div>

<div class="row">
<div class="container">
<a href="{{ site.url }}{{ site.baseurl }}/files/sensys16_back_comm.pdf" style="background-color: white; color: orange;">HitchHike: Practical Backscatter using Commodity WiFi</a> <a href = "https://www.youtube.com/watch?v=4tmatoD0I1o" style="background-color: white; color: blue;">[Talk]</a><br>
Pengyu Zhang (Co-primary), Dinesh Bharadia (Co-primary), Kiran Joshi, Sachin Katti<br>SenSys 2016<br> 
    <font color="red">Best Paper Award Nominee</font><br>
    <font color="red">Press cover:</font> 
    <a style="display: inline-block;" href="http://news.stanford.edu/2016/11/16/miniature-wifi-device-developed-supplies-missing-link-internet-things/">Stanford News</a>, 
    <a style="display: inline-block;" href="http://cacm.acm.org/news/210000-miniature-wi-fi-device-supplies-missing-link-for-the-internet-of-things/fulltext">ACM TechNews</a>,
    <a style="display: inline-block;" href="https://www.ecnmag.com/news/2016/11/miniature-wifi-device-developed-stanford-engineers-supplies-missing-link-internet-things">ECN</a>,
    <a style="display: inline-block;" href="https://scienceblog.com/490143/miniature-wifi-device-supplies-missing-link-internet-things/">Science Blog</a>,
    <a style="display: inline-block;" href="https://pacetoday.com.au/wifi-device-supplies-missing-link-iot/">Pace Today</a>,
    <a style="display: inline-block;" href="http://northdallasgazette.com/2016/11/19/postage-size-wifi-might-make-internet-things-reality/">North Dallas Gazette</a>, 
    <a style="display: inline-block;" href="http://www.newelectronics.co.uk/electronics-news/low-power-wifi-device-to-translate-radio-waves/148386/">New Electronics</a>, 
    <a style="display: inline-block;" href="http://www.rfidjournal.com/articles/view?15280">RFID Journal</a>, 
    <a style="display: inline-block;" href="http://www.nfcworld.com/2016/11/24/348685/us-researchers-claim-discovery-missing-link-internet-things/">NFC World</a>, 
    etc.
</div>
</div>


