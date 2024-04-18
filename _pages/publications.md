---
layout: archive
title: "DIY Projects"
permalink: /diy projects/
author_profile: true
---

{% if site.author.googlescholar %}

Hi
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% for post in site.self explored knowledge reversed %}
  {% include archive-single.html %}
{% endfor %}
