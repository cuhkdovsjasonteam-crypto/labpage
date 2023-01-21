---
title: "WCSNG - Team"
layout: gridlay
excerpt: "WCSNG: Team members"
sitemap: false
permalink: /team/
---

# Group Members



 **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(See Opportunities)]({{ site.url }}{{ site.baseurl }}/vacancies.html) **!**

Jump to [master's students](#masters-students), [undergrad students](#undergraduate-students) and [alumni](#alumni) members.

<div class="row">
<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/dinesh.jpg" class="img-responsive" width="32%" style="float: left" />
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
<!-- </div> -->

<!-- <div class="row"> -->
<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/fred.jpg" class="img-responsive" width="32%" style="float: left" />
  <!-- <div class="col-sm-7 clearfix"> -->
  <h3>fred harris</h3>
  Honorable member, WCSNG<br>
  Adjunct Professor<br>
  Department of Electrical and Computer Engineering <br>
  University of California, San Diego
<ul style="margin: 0; padding: 0; list-style-type:none; overflow: hidden">
<li>Email: <b>fjharris [at] eng.ucsd.edu</b></li>
<li>Office: Jacobs Hall</li>
<li><a href="https://en.wikipedia.org/wiki/Fredric_J._Harris"> Wiki Page </a> | <a href="https://scholar.google.com/citations?user=6A5XoroAAAAJ&hl=en"> Google Scholar </a></li>
</ul>

</div>
</div>

<!-- <hr/> -->
> "In union there is strength" - Aesop

## PhD Students
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i><br>{{ member.email }}
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}



## Collaborations/ Post Doctoral Researchers
{% assign number_printed = 0 %}
{% for member in site.data.collaborations %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br></i>{{ member.email }}
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<!-- {% assign number_printed = 0 %}
{% for member in site.data.collaborations %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i><br>Project: {{ member.project }}
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %} -->

> “The strength of the team is each individual member. The strength of each member is the team.” –Phil Jackson

## Master's Students


{% assign number_printed = 0 %}
{% for member in site.data.students_masters %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i><br>Project: {{ member.project }}
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Undergraduate Students


{% assign number_printed = 0 %}
{% for member in site.data.students_undergrad %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i><br>Project: {{ member.project }}
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br>{{ member.email }}</i> <br> Role: {{ member.info }}
  <ul style="overflow: hidden">
{% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

### Alumni MS students
#### 2022
* Howard Chi (MS 2022) (Full Duplex)
* Sanjeev Anthia Ganesh (Backscatter)

#### 2021
* Gautham Reddy (MS 2021) (Radar) (Now at Broadcom, SJ)
* Nitish Kulshrestha (MS 2021) (Backscatter) (Now at Qualcomm, SD)
* Navin Adarsh (MS 2021) (Channel Prediction) (Now at Uhnder, Missouri)
* Mila Tan (MS 2021) (Millimeter-wave testbed) (Now at maxlinear, SD)
* Weginbara (Michael) Youpele (MS 2021) (Millimeter-wave testbed) (Now at Naval Surface Warfare Center, CA)
* Xiangwei Shao (MS 2021) (Millimeter-wave testbed) (Co-authored mmNets'20) (Now at Huawei)
* Hou-Wei Lin (MS 2021) (Millimeter-wave testbed) (Co-authored mmNets'20) (Now at Amazon, SJ)
* Yeswanth Guntupalli (MS 2021) (Full Duplex Radios) (Now at Apple, SD)

#### 2020
* Yeswanth Reddy Guddeti (MS 2021) (Spectrum Sensing) 
* Aman Goyal (MS 2020) (OTFS communication) (Now at Apple, SJ)
* Rohit Kumar(MS 2020) (Full Duplex) (Now at Qualcomm, SD)
* Shruti Jain (MS 2020) (Full Duplex) (Now at XCOM Labs, SD)
* Shreya Nayak (MS 2020) (OTFS communication) (Now at Qualcomm, SD)
* Inderjot Singh (MS 2020) (S-cube Net Machine learning) (Highlight: ECCV'20) (Now at Plus.ai, Cupertino)
* Aman Raj (MS 2020) (Signet) (Highlight: CVPR'19) (Now at Apple, SJ)
* Yunchieh (Zena) Chang (MS 2020) (Deep Learning and Indoor Localization)
* Sanatan Sharma (MS 2020) (Machine Learning) (Highlight: Mobicom'20) (Now at TuSimple, SD)
* Shrinidhi Venkatakrishnan (MS 2020) (Virtual Reality) (Now at Qualcomm, SD)
* Tejas Sadarhalli (MS 2020) (5G testbed) (Now at Qualcomm, SD)

#### 2019
* Shrivatsan Rajagopalan (MS 2019) (Localization) (Highlight: NSDI'20) (Now at Qualcomm, SD)
* Aravind Seetharaman (MS 2019) (Localization) (Highlight: NSDI'20) (Now at Qualcomm, SJ)
* Shreya Ganesaraman (MS 2019) (Localization) (Highlight: NSDI'20) (Now at Intel, SD)
* Arunkumar Ravichandran (MS 2019) (Wireless VR) (Now at Cisco)
* Yue Meng (MS 2019) (SigNet) (Highlight: CVPR'19) (Now at Honda Research Institute, SJ)
* Samuel Sunarjo (BS-MS 2019) (SigNet) (Highlight: CVPR'19) (Now at Qualcomm, SD)
* Kavya Potluri (MS 2019) (Now at Qualcomm, SD)
* Vamsidhar Reddy (MS 2019) (Machine Learning) (Now at Cruise Automation, SJ)

#### 2018
* Rohit Kulkarni (MS 2018) (Spectrum Sensing) (Now at Qualcomm, SD)

### Alumni BS students

#### 2022
* Raini Wu (BS'22) (VR, spectrum sensing project) (Now PhD at UCSD)
* Wen Tian (BS'22) (Backscatter) (Now PhD at UMich)
* Joel Bisarra (BS'22) (Robotics) 
* Tyler Chang (BS'22) (Robotics) (Coauthor - ULoc at IMWUT'21) 
* Zijia Guo (BS'22) (PCB design project)

#### 2021
* Keshav Rungta (BS'21, MS'22) (Robotics and radar) (Coauthor Sensys'20) (Now at Apple, Sunnyvale)

#### 2020
* Chenfeng Wu (BS'20, MS'21) (Localization) (Co-authored Mobicom'20, NSDI'20) (Now at Ford, Ann Arbor)
* Scott Zhao (BS 2020) (Localization) (Now M.S. at Columbia, NY) (Lead-author IMWUT'21)
* Siyuan Zhu (BS 2020, MS 2022) (Radar for autonomous vehicles) (Co-authored Sensys'20)


### UC San Diego Summer Research Internship Program (SRIP)
Undergraduate/ Masters students - <a href='https://www.ece.ucsd.edu/undergraduate/SRIP'>apply to SRIP program here</a>.
#### Summer 2020
* Keshav Rungta (BS)
* Minghui (Scott) Zhao (BS)
* Shivani Bhakta (BS)
* Samantha Long (BS)
* Eamon Patamasing (BS)
* Yidong Li (BS)
* Siyuan Zhu (BS)
* Raini Wu (BS)
* Tyler Chang (BS)
* Zijia Guo (BS)
* Gautham Reddy (MS)
* Xiangwei Shao (MS)
* Tian Qiu (MS)

#### Summer 2019
* Chenfeng Wu (BS) (Robotics SLAM)
* Scott Zhao (BS) (VR tracking using Radar)
* Shrinidhi (MS) (Wireless VR)
* Aman Goyal (MS) (OTFS)
* Keshav Rungta (BS) (Radar sensing)
* Keshav Mittal (BS) (Localization)
* Karl Wang (BS) (Backscatter)
* Siyuan Zhu (BS) (Radar sensing)



### International Summer Interns
#### Summer 2019
* Rushang Gupta [IITD] (Bluetooth localization)
* Raunak Shah [IITK] (Machine Learning, Signet) (Highlight: ECCV'20)
* Aman Tiwari [IITD] (Phone SLAM)


#### Summer 2018
* Raghav Sonavane [IITKgp] (In-body communication) (Now at Sprinklr, India)
* Raghav Vaidyanathan Subbaraman [IITM] (spectrum sensing) (Highlight: NSDI 2018) (Now PhD at UCSD)
* Sidharth Kumar [IITD] (Wireless power transfer) (Highlight: Mobisys 2019) (Now PhD at UT Austin)
* Zihan Zhang [BUPT China] (Spectrum sensing) (Now MS at Michigan University)

<!--
<table align="center" style="width:100%">
 <tr>
    <th>Visitors</th>
    <th>Master Students</th>
    <th>Bachelor Students</th>
  </tr>
  <tr>
    <td>Nikolaos Iliopoulos, Spring 2016</td>
    <td>Bert Visscher, Fall 2017</td>
    <td>Vishnu Saj, Spring 2017</td>
  </tr>
  <tr>
    <td>Vitaly Fedoseev, all of 2016</td>
    <td>Ahmad Jamalzada, Fall 2017</td>
    <td>Joey Braspenning, Spring 2017</td>
  </tr>
  <tr>
    <td>Ramakrishna Aluru, Summer 2018</td>
    <td>Tjerk Benschop, Summer 2017</td>
    <td>Margot Leemker, Spring 2017</td>
  </tr>
  <tr>
    <td>Changwei Zou, Spring 2018</td>
    <td>Oliver Ostojic, Spring 2016</td>
    <td>Sietske Lensen, Spring 2017</td>
  </tr>
  <tr>
    <td></td>
    <td>Farshaad Hoeseni, Fall 2015</td>
    <td>Alexander Vanstone, Spring 2016</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td>Tjerk Benschop, Spring 2016</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td>Arjo Andringa, Spring 2016</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td>Daniëlle van Klink, Spring 2016</td>
  </tr>
</table>
-->
<!--
## Administrative Support
<a href="mailto:Rijsewijk@Physics.LeidenUniv.nl">Ellie van Rijsewijk</a> is helping us (and other groups) with administration.
-->









