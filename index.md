---
title: "Home"
---

{% for post in site.posts %}
  <h1><a href="{{post.url | prepend: site.baseurl }}">{{ post.title }}</a></h1>
  <div>{{ post.date  | date: "%Y-%m-%d" }}</div>
  <p>{{ post.excerpt }}</p>
{% endfor %}
