---
layout: archive
title: ""
permalink: /publications/
author_profile: true
entries_layout: grid
---

# Peer Review

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% if post.pub == true %}
     {% include archive-single.html %}
  {% endif %}
{% endfor %}

# Others
{% for post in site.publications reversed %}
  {% if post.pub == false %}
     {% include archive-single.html %}
  {% endif %}
{% endfor %}