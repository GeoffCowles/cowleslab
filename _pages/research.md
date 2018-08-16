---
title: "Allan Lab - Research"
layout: textlay
excerpt: "Allan Lab -- Research"
sitemap: false
permalink: /research/
---

# Research Examples

{% for member in site.data.research %}
<div class="row">
<div class="col-sm-12">
 <div class="well">
  <h3><b>{{ member.topic }}</b></h3>
  <img src="{{ site.url }}{{ site.baseurl }}/images/respic/{{ member.image }}" class="img-responsive" width="50%" style="float: left" />

  {% if member.with_support == 1 %}
  <p><it>Support: {{ member.support }}</it></p>
  {% endif %}

  {% if member.with_collaborators == 1 %}
  <p><it>{{ member.collaborators }}</it></p>
  {% endif %}

  {% if member.with_fullpage == 1 %} 
  <p><a href="{{ site.url }}{{ site.baseurl }}/_staticpages/{{member.fullpage}}">Detailed Info</a></p>
  {% endif %}

  <h4>{{ member.synopsis }}</h4>

  <ul style="overflow: hidden">
  {% if member.number_pub == 1 %}
  <li> {{ member.pub1 }} </li>
  {% endif %}

  {% if member.number_pub == 2 %}
  <li> {{ member.pub1 }} </li>
  <li> {{ member.pub2 }} </li>
  {% endif %}

  {% if member.number_pub == 3 %}
  <li> {{ member.pub1 }} </li>
  <li> {{ member.pub2 }} </li>
  <li> {{ member.pub3 }} </li>
  {% endif %}
  </ul>

  </div>
</div>
</div>
{% endfor %}


