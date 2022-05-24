---
title: "WCSNG - Research"
layout: research
excerpt: "WCSNG -- Research"
sitemap: false
permalink: privacy.html
---
<!-- <a href="{{ site.url }}{{ site.baseurl }}/research"><img src="{{ site.url }}{{ site.baseurl }}/images/back.png" class="img-responsive" width="4%" /> </a> -->

# Privacy
<!-- ####  This page contains papers related to `Privacy`. 
#### Go back to other <a href="{{ site.url }}{{ site.baseurl }}/research"> <b>Research</b></a> categories or see full list of <a href="{{ site.url }}{{ site.baseurl }}/publications"> <b>Publications</b></a>. -->


<p> &nbsp; </p>
{% assign number_printed = 0 %}
{% for publi in site.data.publist %}
{% if publi.tag1=='privacy' or publi.tag2=='privacy'  %}

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
