---
layout: default
title: Resources
weight: 5
---

# Community Resources

These are a long list of community resources available for workers in the paleo-bio-geo-sciences.

{% for resources in site.resources %}
  <div class="col-lg-3 col-md-6 text-center">
    <div class="resource-box">
      <big>{{ resources.title }}</big> &#8226; <small>{{ resources.concept }} [<a href="{{resources.url}}">Link</a>]</small><br><p></p>
    </div>
  </div>
{% endfor %}
