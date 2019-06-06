---
layout: archive
title: "Talks and presentations"
permalink: /talks/
author_profile: true
---

<!-- <p style="text-decoration:underline;"><a href="/talkmap.html">See a map of all the places I've given a talk!</a></p> -->

{% include base_path %}

<ul>
{% for post in site.talks reversed %}
  <li>{% include archive-single-talk.html %}
<ul>{% endfor %}
