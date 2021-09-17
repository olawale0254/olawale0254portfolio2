---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

My research explores how artificial intelligence (machine learning in particular) can assist humans in solving engineering design problems. Particularly, I'm interested in developing tools using deep learning, reinforcement learning, active learning, statistical modeling, and engineering optimization to realize performance and efficiency that is unachievable by traditional methods in tasks such as design synthesis, design space exploration, design optimization, and inverse design.

<nbsp>

{% include base_path %}

{% assign ordered_pages = site.research | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single.html %}
{% endfor %}
