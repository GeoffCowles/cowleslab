---
title: "News"
layout: textlay
excerpt: "Cowles Lab at UMass Dartmouth."
sitemap: false
permalink: /allnews/
---

# News

{% for article in site.data.news %}
<div class="well">
<div class="row">
<div class="col-sm-12">
<p>{{ article.date }} <br><em>{{ article.headline }}</em></p>
{% if article.image_cnt == 1 %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/newspic/{{ article.image }}" class="img-responsive" width="25%" style="float: left" >
{% endif %}
</div>
</div>
</div>
{% endfor %}


