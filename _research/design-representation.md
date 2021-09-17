---
title: "Machine Learning-Based Design Representation"
layout: single-portfolio
image: '/images/research/airfoil_hull.gif'
collection: research
order_number: 10
header: 
  og_image: "research/airfoil_hull.gif"
abstract: "Design representation is at the foundation of many design problems. It decides how difficult one can create a new design, and affects the efficiency of design space exploration and optimization. Geometric design representations controlled by hand-crafted parametric models either require unnecessarily many design parameters, contain invalid solutions, or have limited representation capacity. These flaws can negatively impact the performance of design space exploration and optimization. In this line of work, I develop machine learning models to learn new design parameterizations and hence avoid human biases introduced by hand-crafted models. Our past experiments have shown that the learned parameterizations can form compact, ordered representations, and achieve an order of magnitude speedup in design optimization tasks compared to other state-of-the-art parameterizations."
---

{{ page.abstract }}

## Related Papers

{% for post in site.publications reversed %}
  {% if post.topic.design_representation %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

