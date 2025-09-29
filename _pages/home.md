---
title: "YamLab - Home"
layout: homelay
excerpt: "Yam at CUHK."
sitemap: false
permalink: /
---

### About

Yam Lab is dedicated to research on myopia, children eye diseases, and retinoblastoma, involving basic, translational, and clinical research. The primary research objectives include the discovery of disease’s mechanism, development of new treatment/diagnostic methods, and implementation of novel interventions. The motivation of our research is to protect children’s vision, allowing them to see the world clearly and to develop a bright future.

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

        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/图片2.jpg" alt="Slide 2" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/图片3.jpg" alt="Slide 3" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/图片4.jpg" alt="Slide 4" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/图片5.jpg" alt="Slide 5" />
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

