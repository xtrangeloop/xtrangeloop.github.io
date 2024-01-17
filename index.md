---
title: "Home"
---

# Welcome to my {{ site.description }}.

<!---
{% for post in site.posts %}
  <h1 class="w3-text-pink"><a href="{{post.url | prepend: site.baseurl }}">{{ post.title }}</a></h1>
  <h4 class="w3-text-gray">{{ post.date  | date: "%Y-%m-%d" }}</h4>
  <h5>{{ post.description }}</h5>
{% endfor %}
--->

<h2>Recent Posts</h2>

{% for post in site.posts %}
### [{{ post.title }}]({{post.url | prepend: site.baseurl }})
<p style="padding-left:35px;">{{ post.date  | date: "%Y-%m-%d" }} - {{ post.description }}</p> 
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
