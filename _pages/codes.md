---
title: "Cowles Lab - Codes" 
layout: gridlay
excerpt: "Cowles Lab: Codes" 
sitemap: false
permalink: /codes/
---

<!---# Codes --->


{% for member in site.data.codes %}
<div class="row">
<div class="col-sm-12">
<!--- <div class="well">---->
 <div class="panel panel-info">
 <div class="panel-heading"><h3><b>{{member.name}}</b></h3></div>
  <div class="panel-body">
  <it>{{ member.description }}</it>
  <h4>{{ member.source }}</h4>
  {% if member.number_pub > 0 %}
  <it>Related Publications</it> 
  {% endif %}
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

  {% if member.number_pub == 4 %}
  <li> {{ member.pub1 }} </li>
  <li> {{ member.pub2 }} </li>
  <li> {{ member.pub3 }} </li>
  <li> {{ member.pub4 }} </li>
  {% endif %}

  {% if member.number_pub == 5 %}
  <li> {{ member.pub1 }} </li>
  <li> {{ member.pub2 }} </li>
  <li> {{ member.pub3 }} </li>
  <li> {{ member.pub4 }} </li>
  <li> {{ member.pub5 }} </li>
  {% endif %}
  </ul>

 </div>
 </div>
</div>
</div>
{% endfor %}


