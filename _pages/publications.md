---
title: "Yanmin Gong - Publications"
layout: gridlay
excerpt: "Yanmin Gong -- Publications."
sitemap: false
permalink: /publications/
---


<!-- ### Publications -->
### Publications by Area (quick view)

- **AI for Health:** CHASE’25 (MOUD dropout), JMIR’23 (mHealth), JHIR’24 (Fairness in FL for healthcare)
- **Federated & Distributed Learning:** ICLR’22 (Spotlight), ICCV’23 (Workie-Talkie/FedCR), TVT’25 (Edge FL scheduling), INFOCOM’25 (Fed-tuning LLMs)
- **Trustworthy AI:** TIFS’19 (DP-ADMM), TDSC’23 (Intrinsic privacy in wireless FL), ICC’25 (PFedSAM)
- **Edge/Networking/Systems:** TMC’22 (Cooperative edge FL), TVT’24 (Multi-UAV MEC), TWC’23 (FD-DSA)
- **Generative & FMs:** ICLR’24 (LyCORIS), INFOCOM’25 (Hetero-quantized + LoRA Fed-tuning)

### Selected Publications

(For a full list see [below](#full-list) or go to [Google Scholar](https://scholar.google.com/citations?user=o3BGIEMAAAAJ&hl=en))

{% assign number_printed = 0 %}
{% for publi in site.data.publistj %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.link.display }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong>{{ publi.title }}</strong></p>
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

{% for publi in site.data.publistc %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.link.display }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong>{{ publi.title }}</strong></p>
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

{% for publi in site.data.publistw %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.link.display }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong>{{ publi.title }}</strong></p>
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


### Full List
#### Peer-Reviewed Journal Articles

{% for publi in site.data.publistj %}

1. {{ publi.link.display }} <br />
  <em>{{ publi.authors }} </em><br />{{ publi.title }}

{% endfor %}

#### Conference Papers

{% for publi in site.data.publistc %}

1. {{ publi.link.display }} <br />
  <em>{{ publi.authors }} </em><br />{{ publi.title }}

{% endfor %}

<!--
#### Workshop Papers and Posters

{% for publi in site.data.publistw %}

1. {{ publi.link.display }} <br />
  <em>{{ publi.authors }} </em><br />{{ publi.title }}

{% endfor %}
-->

#### Preprints

{% for publi in site.data.publistw %}

1. {{ publi.link.display }} <br />
  <em>{{ publi.authors }} </em><br />{{ publi.title }}

{% endfor %}
