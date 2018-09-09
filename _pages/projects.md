---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

<!-- {% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %} -->

{% include base_path %}

<ul>
{% for post in site.projects reversed %}
  <li>{% include archive-single.html %}</li>
{% endfor %}
</ul>
