---
layout: page
title: All Posts
permalink: /all-posts/
description: Every update, oldest to newest
---

Start at the beginning and read the whole story in order.

<ul class="all-posts-list">
{% assign chronological = site.posts | reverse %}
{% for post in chronological %}
  <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> &middot; {{ post.date | date: "%B %-d, %Y" }}</li>
{% endfor %}
</ul>
