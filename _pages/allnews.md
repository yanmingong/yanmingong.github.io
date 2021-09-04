---
title: "News"
layout: textlay
excerpt: "TINS Lab at San Antonio."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
{{ article.headline }}</p>
{% endfor %}
