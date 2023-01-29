---
title: "Wireless Sensing"
layout: research-new
excerpt: "Wireless Sensing"
sitemap: false
permalink: wireless-sensing.html
---
<!-- <a href="{{ site.url }}{{ site.baseurl }}/research"><img src="{{ site.url }}{{ site.baseurl }}/images/back.png" class="img-responsive" width="4%" /> </a> -->
<div class="col-sm-24 clearfix">
<div class="well">
   <center>
     <h4><a href="#proj">Projects</a>&emsp;<a href="#open">Open-Sourcing</a>&emsp;<a href="#pubs">Publications</a>&emsp;<a href="#demos">Demos and Posters</a>&emsp;<a href="#team">Team</a></h4>
   </center>
</div>
</div>



# Wireless Sensing
<!-- ####  This page contains papers related to `Wireless Sensing and Localization`. 
#### Go back to other <a href="{{ site.url }}{{ site.baseurl }}/research"> <b>Research</b></a> categories or see full list of <a href="{{ site.url }}{{ site.baseurl }}/publications"> <b>Publications</b></a>. -->
<div id="top">
<div class="col-sm-24 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/wireless_sensing.svg" class="img-responsive" width="100%" style="float: center"/>
  <p>We at the Wireless Sensing group of <a href="{{ site.url }}{{ site.baseurl }}">WCSNG</a>, focus on designing, researching, developing, and deploying wireless localization and sensing systems for a wide range of applications, including Extended Reality, Indoor Robotics, Navigation, Warehouse management and Industrial IoT 4.0, with the goal of providing accurate and reliable location and sensing estimates for humans, devices, and robots.</p>

### Latest News & Updates

<ul>

 <li> <b>January 2023</b> A 2nd iteration of <a href= "https://wcsng.ucsd.edu/wild/" style="color:green">[WILD]</a> has been released for a <a href="https://www.kaggle.com/competitions/wildv2/data">Kaggle competition</a>. More details can be found at <a href= "https://wcsng.ucsd.edu/waip" style="color:blue">[WAIP]</a>.</li>
 <li> <b>May 2022:</b> Wide press coverage about our work in P2SLAM, Using everyday WiFi to help robots see and navigate better indoors.  <a href="https://today.ucsd.edu/story/using-everyday-wifi-to-help-robots-see-and-navigate-better-indoors">UCSD Press Coverage.</a>, <a href="https://www.eurekalert.org/news-releases/953372">eurekalert.</a>, <a href="https://www.azosensors.com/news.aspx?newsID=15051">Azosensors.</a></li>
 <li> <b>April 2022:</b> The 1st international workshop for Wireless AI perception is happening at CVPR 2022. More details can be found at <a href= "https://wcsng.ucsd.edu/waip/" style="color:blue">[WAIP]</a>.</li>
 <li> <b>September 2021</b>UCSD News article on ULoc. <a href="https://today.ucsd.edu/story/new-upgrades-to-old-wireless-tech-could-enable-real-time-3d-motion-capture">New Upgrades to Old Wireless Tech Could Enable Real-Time 3D Motion Capture</a></li>
 <li> <b>April 2020:</b> WCSNG group inspired from the need of contact tracing and proximity sensing, has developed a BLE based proximity sensing called <a href = "https://wcsng.ucsd.edu/bluble/">BluBLE</a> to tackle with the COVID-19 pandemic.</li>
 <li> <b>Feb 2019:</b> BLoc published in Dec 2018 has prposed the idea of long sequences of 1's and 0's along with multiple antenna BLE master to enable AoA esitmation along with relative ToF esimation. Later in January 2019, <a href = "">BLE 5.1</a> has propsoed CTE (series of un-whitened 1's) based protocol for AoA esitmation.</li>

</ul>

</div>

</div>

<hr>


<div id="proj">

## Projects

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% if publi.tag1=='wireless-sensing' or publi.tag2=='wireless-sensing'  %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}


<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }} <a href="{{ publi.link.url }}"><span style="color:tomato;">{{ publi.link.display }}</span></a></pubtit>
  <p><strong>
  <a href="{{ publi.website.url }}">{{ publi.website.display }}</a>
  <a href="{{ site.url }}{{ site.baseurl }}/{{ publi.paper.url }}"><span style="color:#D35400;">{{ publi.paper.display }}</span></a>
  <a href="{{ site.url }}{{ site.baseurl }}/{{ publi.presentation.url }}"><span style="color:#7D3C98;">{{ publi.presentation.display }}</span></a> 
  </strong></p>
  <p><em>{{ publi.authors }}</em></p>
  
  <meta name="publi.keywords.name" content="{{ publi.keywords.content }}">
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="100%" style="float: center" />
  <p>{{ publi.short-desc }}</p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
</div>


<hr>
<!-- <p> &nbsp; </p> -->

<div id="open">
## Open-Source

<p>At WCSNG we develop systems that are deployable and reproducable, So, we open-sourced our <a href="#code"><b>Codes</b></a>, <a href="#data"><b>Datasets</b></a>, and <a href="#platform"><b>Platform Designs</b></a> to ensure reproducability and aid also to aid the wireless sensing research in the community.</p>

#### Source-code
<div class="col-sm-12 clearfix" id="code">
 <div class="well">
{% for publi in site.data.opensrc_list %}
{% if publi.tag1=='wireless-sensing' or publi.tag2=='wireless-sensing'  %}

{% if publi.type=='code' %}
<li>
  <pubtit>{{ publi.title }} <a href="{{ publi.link.url }}"><span style="color:tomato;">{{ publi.link.display }}</span></a>
  <a href="{{ publi.website.url }}">{{ publi.website.display }}</a>
  <a href="{{ site.url }}{{ site.baseurl }}/{{ publi.paper.url }}"><span style="color:#D35400;">{{ publi.paper.display }}</span></a>
  <a href="{{ site.url }}{{ site.baseurl }}/{{ publi.presentation.url }}"><span style="color:#7D3C98;">{{ publi.presentation.display }}</span></a> 
  </pubtit>
  <p><em>{{ publi.authors }}</em></p>
  <meta name="publi.keywords.name" content="{{ publi.keywords.content }}">
  <!-- <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="100%" style="float: center" /> -->
  <p>{{ publi.short-desc }}</p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
</li>
{% endif %}
{% endif %}
{% endfor %}
 </div>
</div>

#### Datasets
<div id="data">
{% for publi in site.data.opensrc_list %}
{% if publi.tag1=='wireless-sensing' or publi.tag2=='wireless-sensing'  %}
{% if publi.type=='data' %}

{% assign number_printed = 0 %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }} <a href="{{ publi.link.url }}"><span style="color:tomato;">{{ publi.link.display }}</span></a></pubtit>
  <p><strong>
  <a href="{{ publi.website.url }}">{{ publi.website.display }}</a>
  <a href="{{ site.url }}{{ site.baseurl }}/{{ publi.paper.url }}"><span style="color:#D35400;">{{ publi.paper.display }}</span></a>
  <a href="{{ site.url }}{{ site.baseurl }}/{{ publi.presentation.url }}"><span style="color:#7D3C98;">{{ publi.presentation.display }}</span></a> 
  </strong></p>
  <p><em>{{ publi.authors }}</em></p>
  
  <meta name="publi.keywords.name" content="{{ publi.keywords.content }}">
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="100%" style="float: center" />
  <p>{{ publi.description }}</p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% assign even_odd = number_printed | modulo: 3 %}

{% endif %}

{% endif %}
{% endfor %}

{% if even_odd == 2 or even_odd == 1 %}
</div>
{% endif %}

</div>

#### Platforms
<div id="platform">
{% for publi in site.data.opensrc_list %}
{% if publi.tag1=='wireless-sensing' or publi.tag2=='wireless-sensing'  %}
{% if publi.type=='platform' %}

{% assign number_printed = 0 %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }} <a href="{{ publi.link.url }}"><span style="color:tomato;">{{ publi.link.display }}</span></a></pubtit>
  <p><strong>
  <a href="{{ publi.website.url }}">{{ publi.website.display }}</a>
  <a href="{{ site.url }}{{ site.baseurl }}/{{ publi.paper.url }}"><span style="color:#D35400;">{{ publi.paper.display }}</span></a>
  <a href="{{ site.url }}{{ site.baseurl }}/{{ publi.presentation.url }}"><span style="color:#7D3C98;">{{ publi.presentation.display }}</span></a> 
  </strong></p>
  <p><em>{{ publi.authors }}</em></p>
  
  <meta name="publi.keywords.name" content="{{ publi.keywords.content }}">
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="100%" style="float: center" />
  <p>{{ publi.description }}</p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% assign even_odd = number_printed | modulo: 3 %}

{% endif %}

{% endif %}
{% endfor %}

{% if even_odd == 2 or even_odd == 1 %}
</div>
{% endif %}

</div>
<!-- <p> &nbsp; </p> -->


<hr>

## Posters and Demos
<div id="demos">
{% assign number_printed = 0 %}
{% for publi in site.data.demopost-list %}

{% if publi.tag1=='wireless-sensing' or publi.tag2=='wireless-sensing'  %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}


<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }} </pubtit>
  <p><strong>
  <a href="{{ publi.link.url }}"><span style="color:tomato;">{{ publi.link.display }}</span></a>
  <a href="{{ publi.website.url }}">{{ publi.website.display }}</a>
  <a href="{{ site.url }}{{ site.baseurl }}/{{ publi.paper.url }}"><span style="color:#D35400;">{{ publi.paper.display }}</span></a>
  <a href="{{ site.url }}{{ site.baseurl }}/{{ publi.presentation.url }}"><span style="color:#7D3C98;">{{ publi.presentation.display }}</span></a> 
  </strong></p>
  <p><em>{{ publi.authors }}</em></p>
  
  <a href="{{ site.url }}{{ site.baseurl }}/{{ publi.paper.url }}"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/posters/{{ publi.image }}" class="img-responsive" width="100%" style="float: center" /></a>
  <p>{{ publi.short-desc }}</p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
<!-- <p> &nbsp; </p> -->

<hr>

</div>
<div id="pubs">
## Full List of Publications

{% for publi in site.data.publist %}
{% if publi.tag1=='wireless-sensing' or publi.tag2=='wireless-sensing'  %}
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}
{% endfor %}
</div>

<hr>

<!-- <p> &nbsp; </p> -->
<div id="team">

## Team

> “The strength of the team is each individual member. The strength of each member is the team.” –Phil Jackson

### Advisor
<div class="row">
<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/dinesh.jpg" class="img-responsive" width="30%" style="float: left" hspace="20" />
  <!-- <div class="col-sm-7 clearfix"> -->
  <h3>Dinesh Bharadia</h3>
  Principal Investigator, WCSNG<br>
  Associate Professor<br>
  Department of Electrical and Computer Engineering <br>
  University of California, San Diego
<ul style="margin: 0; padding: 0; list-style-type:none; overflow: hidden">
<li>Email: <b>dineshb [at] eng.ucsd.edu</b></li>
<li>Office: FAH 2303, Franklin Antonio Hall</li>
<li><a href="https://web.eng.ucsd.edu/~dineshb/"> Personal Website </a> | <a href="https://scholar.google.com/citations?user=5SjaXJsAAAAJ&hl=en"> Google Scholar </a></li>
</ul>

</div>
</div>



### Ph.D. Mentors
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}
{% if member.research1=='wireless-sensing' or member.research2=='wireless-sensing'  %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="30%" style="float: left" hspace="20" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i><br>{{ member.email }}
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 3 %}
{% if even_odd == 2 or even_odd == 1 %}
</div>
{% endif %}



### Collaborations and Post Doctoral Researchers
{% assign number_printed = 0 %}
{% for member in site.data.collaborations %}

{% if member.research1=='wireless-sensing' or member.research2=='wireless-sensing'  %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="30%" style="float: left" hspace="20" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br></i>{{ member.email }}
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 3 %}
{% if even_odd == 2 or even_odd == 1 %}
</div>
{% endif %}


#### Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% if member.research1=='wireless-sensing' or member.research2=='wireless-sensing'  %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="30%" style="float: left" hspace="20" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br></i>{{ member.email }}
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 3 %}
{% if even_odd == 2 or even_odd == 1 %}
</div>
{% endif %}

### Master's Students
{% assign number_printed = 0 %}
{% for member in site.data.students_masters %}

{% if member.research1=='wireless-sensing' or member.research2=='wireless-sensing'  %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="30%" style="float: left" hspace="20" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br></i>{{ member.email }}
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 3 %}
{% if even_odd == 2 or even_odd == 1 %}
</div>
{% endif %}
#### Alumni MS students
##### 2020
* Yunchieh (Zena) Chang (MS 2020) (Deep Learning and Indoor Localization)
* Sanatan Sharma (MS 2020) (Machine Learning) (Highlight: Mobicom'20) (Now at TuSimple, SD)

##### 2019
* Shrivatsan Rajagopalan (MS 2019) (Localization) (Highlight: NSDI'20) (Now at Qualcomm, SD)
* Aravind Seetharaman (MS 2019) (Localization) (Highlight: NSDI'20) (Now at Qualcomm, SJ)
* Shreya Ganesaraman (MS 2019) (Localization) (Highlight: NSDI'20) (Now at Intel, SD)


### Bachelors Students
{% assign number_printed = 0 %}
{% for member in site.data.students_undergrad %}

{% if member.research1=='wireless-sensing' or member.research2=='wireless-sensing'  %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="30%" style="float: left" hspace="20" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br></i>{{ member.email }}
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 3 %}
{% if even_odd == 1 or even_odd == 2 %}
</div>
{% endif %}
#### Alumni BS students

##### 2022
* Joel Bisarra (BS'22) (Robotics) 
* Tyler Chang (BS'22) (Robotics) (Coauthor - ULoc at IMWUT'21) 

##### 2020
* Chenfeng Wu (BS'20, MS'21) (Localization) (Co-authored Mobicom'20, NSDI'20) (Now at Ford, Ann Arbor)
* Scott Zhao (BS 2020) (Localization) (Now M.S. at Columbia, NY) (Lead-author IMWUT'21)

##### UC San Diego Summer Research Internship Program (SRIP)
Undergraduate/ Masters students - <a href='https://www.ece.ucsd.edu/undergraduate/SRIP'>apply to SRIP program here</a>.
##### Summer 2020
* Minghui (Scott) Zhao (BS)
* Shivani Bhakta (BS)
* Tyler Chang (BS)

##### Summer 2019
* Chenfeng Wu (BS) (Robotics SLAM)
* Scott Zhao (BS) (VR tracking using Radar)
* Keshav Mittal (BS) (Localization)


##### International Summer Interns
##### Summer 2019
* Rushang Gupta [IITD] (Bluetooth localization)
* Aman Tiwari [IITD] (Phone SLAM)

##### Summer 2018
* Raghav Sonavane [IITKgp] (In-body communication) (Now at Sprinklr, India)

</div>

<p> &nbsp; </p>

<div class="col-sm-24 clearfix">
<div class="well">
   <center>
     <h4><a href="#top">Wireless Sensing Home (Go to top)</a>&emsp;<a href="#proj">Projects</a>&emsp;<a href="#open">Open-Sourcing&emsp;<a href="#pubs">Publications</a></a>&emsp;<a href="#demos">Demos and Posters</a>&emsp;<a href="#team">Team</a></h4>
   </center>
</div>
</div>