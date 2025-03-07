---
layout: home
title: Welcome to My Site
---

Welcome to my website! Here you'll find helpful articles and reviews about various products.

## Latest Articles

{% for post in site.posts limit:5 %}
* [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
