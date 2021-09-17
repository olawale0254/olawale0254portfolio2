---
title: "Deep Generative Modeling in Engineering"
layout: single-portfolio
image: '/images/research/ffdgan.png'
collection: research
order_number: 30
header: 
  og_image: "research/ffdgan.png"
abstract: "Deep generative models (e.g., VAEs, GANs, and invertible NNs) are successfully applied in the domain of computer vision. This success is owing to their ability to learn complex, high-dimensional data distributions, and hence generate new data by sampling from that distribution. We can also make these generative models to learn the distribution of engineering designs and generate new ones. This will help in various tasks such as data augmentation for surrogate modeling, design representation learning, design optimization, inverse design, and uncertainty quantification. Different from the image generation problem commonly seen in computer vision, engineering design generation is usually subject to strict constraints. For example, aerodynamic or hydrodynamic designs require smooth surfaces. In addition, engineering designs are normally associated with performance metrics (e.g., lift and drag). In this line of work, I develop new deep generative models to account for these two factors. This brings the benefits of deep generative modeling into the engineering domain."
---

{{ page.abstract }}

## Related Papers

{% for post in site.publications reversed %}
  {% if post.topic.generative_modeling %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
