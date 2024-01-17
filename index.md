---
title: "Home"
---

<h1>Welcome to my {{ site.description }}.</h1>

<!---
{% for post in site.posts %}
  <h1 class="w3-text-pink"><a href="{{post.url | prepend: site.baseurl }}">{{ post.title }}</a></h1>
  <h4 class="w3-text-gray">{{ post.date  | date: "%Y-%m-%d" }}</h4>
  <h5>{{ post.description }}</h5>
{% endfor %}
--->

<H4>Recent Posts</H4>

<DL>
  {% for post in site.posts %}
  <DT> <h1><a href="{{post.url | prepend: site.baseurl }}">{{ post.title }}</a></h1> <h5>{{ post.date  | date: "%Y-%m-%d" }}</h5> </DT>
  <DD> <h4>{{ post.description }}</h4> </DD>
  {% endfor %}
</DL>

<!---
<OL>
<LI>Main Heading
<UL>
<LI>List item 1
<LI>List item 2
</UL>
<LI>Secondary Heading
<UL>
<LI>List item 1
<LI>List item 2
</UL>
</OL>
--->
