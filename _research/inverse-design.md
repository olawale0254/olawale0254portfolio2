---
title: "Data-Driven Inverse Design"
layout: single-portfolio
image: "/images/research/inverse_design.png"
collection: research
order_number: 20
header: 
  og_image: "research/inverse_design.png"
abstract: "A typical inverse design problem can be solved by optimization, where we optimize design parameters such that the design’s performance satisfies certain targets. Unfortunately, gradient-based optimization (e.g., topology optimization or adjoint-based shape optimization) is restricted to limited design representations and solver types. On the other hand, in gradient-free optimization (e.g., genetic algorithm or Bayesian optimization), as the number of design variables increases, the computational cost quickly becomes prohibitive due to the curse of dimensionality. The goal for this line of work is to solve the inverse design problem without the need of an iterative optimization process. We achieve this goal by learning a one-to-many (target to design) mapping from the data. These new inverse design approaches eliminate the computational time of the iterative optimization, and are particularly useful in large-scale inverse design problems, such as heterogeneous materials design using metamaterials."
---

{{ page.abstract }}

## Related Papers

{% for post in site.publications reversed %}
  {% if post.topic.inverse_design %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}


