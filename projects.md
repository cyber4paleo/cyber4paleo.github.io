---
layout: default
title: Projects
weight: 5
---

# Project Ideas

There are many project topics or ideas that can be addressed in this meeting.  This page is intended to be the location for team or group summary pages.  Once you've met and started working on an idea, please add a Markdown or HTML page to the `_projects` folder in the [cyber4paleo.github.io](https://github.com/cyber4paleo/cyber4paleo.github.io) GitHub repository.

{% for projects in site.projects %}
  <div class="col-lg-3 col-md-6 text-center">
    <div class="resource-box">
      <big>{{ projects.title }}</big> &#8226; <small>{{ projects.concept }} [<a href="{{projects.url}}">Link</a>]</small><br><p></p>
    </div>
  </div>
{% endfor %}

The [YAML](http://www.yaml.org/start.html) header for your Markdown document should match those of other pages.  In particular the header should include: `layout: page`, some `title:` and a `concept` heading, which is a brief summary of your team purpose.  You can look at the **Team Awesome** page for an example.