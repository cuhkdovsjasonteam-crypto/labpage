---
title: "YamLab - Home"
layout: homelay
excerpt: "Yam at CUHK."
sitemap: false
permalink: /
---

### About

Prof Jason Yam is Professor & Undergraduate Division Head at Department of Ophthalmology and Visual Sciences of CUHK, Dean of General Education at Chung Chi College, CUHK, Head of Pediatric Ophthalmology and Strabismus service at Hong Kong Eye Hospital, and Head of Ophthalmology Service at Hong Kong Children′s Hospital. He is also Director of CUHK Jockey Club Myopia Prevention Programme. Prof Jason Yam graduated as Bachelor of Medicine and Bachelor of Surgery from the University of Hong Kong in 2005, and received his Doctor of Medicine with Merit from the Chinese University of Hong Kong in 2023. He received overseas training on Pediatric Ophthalmology and Strabismus in Great Ormond Street Hospital (2011); with Dr David Guyton of Johns Hopkins Hospital (2011); and with Dr Kenneth Wright in Los Angeles (2012); ocular genetics with Dr Janey Wiggs of Harvard Medical School (2016); with Dr Alex Levin of Wills Eye Hospital (2017); and Baylor College of Medicine at Texas Children Hospital (2017); ocular oncology and retinoblastoma with Dr Jerry Shields and Dr Carol Shields of Wills Eye Hospital (2017).

<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="5000" data-pause="hover" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        <li data-target="#carousel" data-slide-to="0" class="active"></li>
        <li data-target="#carousel" data-slide-to="1"></li>
        <li data-target="#carousel" data-slide-to="2"></li>
        <li data-target="#carousel" data-slide-to="3"></li>
        <li data-target="#carousel" data-slide-to="4"></li>
        <li data-target="#carousel" data-slide-to="5"></li>
    </ol>

    <!-- Items -->
    <div class="carousel-inner" markdown="0">

        <div class="item active">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/low-power-WiFi-chip-4.jpg" alt="Slide 1" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/beargroup.jpg" alt="Slide 2" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/dineshmani.jpg" alt="Slide 3" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/birthday.jpg" alt="Slide 4" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/groupevent.jpg" alt="Slide 5" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/dinner1.jpg" alt="Slide 6" />
        </div>
    </div>
  <a class="left carousel-control" href="#carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>

# Research


{% assign number_printed = 0 %}
{% for publi in site.data.research_list %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit> <font size="+2">{{ publi.title }}</font></pubtit>
  <meta name="publi.keywords.name" content="{{ publi.keywords.content }}">
  <img src="{{ site.url }}{{ site.baseurl }}/images/respic/{{ publi.image }}" class="img-responsive" width="50%" style="float: right; margin-right: 5px; margin-left: 10px " />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ site.url }}{{ site.baseurl }}{{ publi.link.url }}.html">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
  <p><strong><a href="{{ site.url }}{{ site.baseurl }}/{{ publi.website.url }}">{{ publi.website.display }}</a></strong></p>
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

 **We are  looking for passionate new PhD students, Postdocs, and Master's students to join the team** [(more info)]({{ site.url }}{{ site.baseurl }}/vacancies.html) **!**


<!--We are grateful for funding from Leiden University, [NWO](www.nwo.nl) ([Vidi talent scheme](http://www.nwo.nl/en/research-and-results/programmes/Talent+Scheme) and the [Frontiers in Nanoscience program](https://www.universiteitleiden.nl/en/research/research-projects/science/frontiers-of-nanoscience-nanofront)), and from an [ERC starting grant](https://erc.europa.eu/funding/starting-grants).

<figure class="fourth">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_Leiden.jpg" style="width: 210px">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_Nanofront.jpg" style="width: 110px">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_NWO.jpg" style="width: 120px">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_ERC.jpg" style="width: 110px">
</figure>-->
