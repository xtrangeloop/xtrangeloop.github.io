---
title: "Home"
---

# Welcome to my {{ site.description }}.

 <p style="padding-left:35px;"> I find that regardless of our differences, unexplainable loops intricately spiral through our world, winding along, connecting us... </p>

## Recent Twisty Passages

<ul class="star">
{% for post in site.posts %}
  <li> <a href="{{post.url | prepend: site.baseurl }}">{{post.title}}</a> &middot; {{ post.date  | date: "%Y-%m-%d" }} &middot; <i>{{ post.description }}</i></li>
{% endfor %}
</ul>
