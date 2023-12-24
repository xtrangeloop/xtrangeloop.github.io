---
title: "Home"
---

{% for post in site.posts %}
  <h1 class="w3-text-pink"><a href="{{post.url | prepend: site.baseurl }}">{{ post.title }}</a></h1>
  <h4>{{ post.date  | date: "%Y-%m-%d" }}</h4>
  <p>{{ post.description }}</p>
{% endfor %}
