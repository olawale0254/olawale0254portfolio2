---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

## Journal
---

{% for post in site.publications reversed %}
  {% if post.category == 'journal' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Conference
---

{% for post in site.publications reversed %}
  {% if post.category == 'conference' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Preprint
---

{% for post in site.publications reversed %}
  {% if post.category == 'preprint' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
