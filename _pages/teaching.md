---
title: "Cowles Lab - Teaching"
layout: gridlay
excerpt: "Cowles Lab: Teaching"
sitemap: false
permalink: /teaching/
---

# Teaching 

## Current Courses


{% for member in site.data.teaching %}
<div class="row">
<div class="col-sm-12">
 <div class="well">
  <h3><b>{{ member.number }}&nbsp;-&nbsp;{{member.name}}</b></h3>
  <it>Offered: {{ member.offered }}</it>
  <h4>{{ member.synopsis }}</h4>
  <a href="{{ site.url }}{{ site.baseurl }}/docs/syllabus/{{ member.syllabus }}" target="_blank"> {{member.syllabus}} </a>
</div>
</div>
</div>
{% endfor %}

<p> &nbsp; </p>

## Past Offerings

{% for member in site.data.priorteaching %}
<div class="row">
<div class="col-sm-12">
 <div class="well">
  <h3><b>{{ member.number }}&nbsp;-&nbsp;{{member.name}}</b></h3>
  <it>Offered: {{ member.offered }}</it>
  <h4>{{ member.synopsis }}</h4>
  <a href="{{ site.url }}{{ site.baseurl }}/docs/syllabus/{{ member.syllabus }}" target="_blank"> {{member.syllabus}} </a>
</div>
</div>
</div>
{% endfor %}

