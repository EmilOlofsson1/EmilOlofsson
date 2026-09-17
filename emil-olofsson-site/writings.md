---
layout: default
title: Other Writings
permalink: /writings/
---
{% if site.posts.size > 0 %}
<ul class="post-list">
{% for post in site.posts %}
  <li class="post-list-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="post-list-date">{{ post.date | date: '%B %-d, %Y' }}</span>
  </li>
{% endfor %}
</ul>
{% else %}
<p class="empty-note">No writings published yet.</p>
{% endif %}
