---
title: "News"
layout: textlay
excerpt: "Allan Lab at Leiden University."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<div class="row">
<div class="col-sm-12">
 <div class="well">
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
</div>
</div>
</div>
{% endfor %}


