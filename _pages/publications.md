---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
entries_layout: grid
g1:
  - image_path: 500x300.png
g2:
  - image_path: foo-bar-identity.jpg
  - image_path: foo-bar-identity.jpg
  - image_path: foo-bar-identity.jpg
g3:
  - image_path: 500x300.png
  - image_path: 500x300.png
g4:
  - image_path: foo-bar-identity.jpg
  - image_path: 500x300.png
  - image_path: 500x300.png
---

## Peers Review

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
  {% if post.galid %}
	{% include gallery id=post.galid %}
  {% endif %}
{% endfor %}

## Others

{% for post in site.nonpubs reversed %}
  {% include archive-single.html %}
  {% if post.galid %}
	{% include gallery id=post.galid %}
  {% endif %}
{% endfor %}