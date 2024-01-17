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

<h2>Recent Posts</h2>

{% for post in site.posts %}
    <h3><a href="{{post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
    <p style="padding-left:20px;">{{ post.date  | date: "%Y-%m-%d" }} - {{ post.description }}</p> 
{% endfor %}

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
