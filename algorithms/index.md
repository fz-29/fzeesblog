---
layout: page
title: Algorithms
excerpt: "An archive of some good algorithm posts"
search_omit: true
---

<ul class="post-list">
{% for post in site.categories.algorithms %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></article></li>
{% endfor %}
</ul>
