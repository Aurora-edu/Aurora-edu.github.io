---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


I'm a third-year undergraduate student majoring in Mathematics and Physics at Tsinghua University. My research interests lies in  ML/CV, including generative models, VLMs, Video Gen/World Model and training dynamics, ICL. I prefer the principles for understanding neural networks and building next-generation AI. 

Now I'm looking forward to 27fall phd positions.

<div class="publication-section-heading">
  <span class="publication-heading">Recent Selected Publications [<a style="font-size:20px;" href="{{ "/publications/" | relative_url }}"> Full List </a>]</span>
  <p>(*Equal Contribution, #Corresponding Author)</p>
</div>

{% assign selected_publications = site.publications | sort: "featured_order" %}
<table class="publication-list"><tbody>
{% for post in selected_publications limit: 2 %}
  {% include publication-card.html pub=post %}
{% endfor %}
</tbody></table>
