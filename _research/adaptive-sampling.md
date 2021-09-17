---
title: "Adaptive Sampling and Bayesian Optimization"
layout: single-portfolio
image: '/images/research/aes.gif'
collection: research
order_number: 40
header: 
  og_image: "research/aes.gif"
abstract: "Design space exploration and optimization require expensive performance evaluations (i.e., numerical simulations or physical experiments). Adaptive sampling and Bayesian optimization are techniques that aim to minimize the number of evaluations. In this work, I adjust these frameworks so that they can be better adapted to machine learning-based design representations and facilitate feasible domain identification, design optimization, and novel design discovery. Specifically, my past work looked into the problem of unbounded adaptive sampling and Bayesian optimization, because manually-defined variable bounds may not include all feasible solutions or the global optimum, especially when the learned representation does not have physical meanings. The proposed approaches can start from an initial point in the design space, and gradually expand the region the algorithm has seen."
---

{{ page.abstract }}

## Related Papers

{% for post in site.publications reversed %}
  {% if post.topic.adaptive_sampling %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
