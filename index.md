---
title: "Home"
---

# Welcome to my {{ site.description }}.

I find that regardless of our differences, unexplainable loops intricately spiral through our world, winding along, connecting us... 

<!---
{% for post in site.posts %}
  <h1 class="w3-text-pink"><a href="{{post.url | prepend: site.baseurl }}">{{ post.title }}</a></h1>
  <h4 class="w3-text-gray">{{ post.date  | date: "%Y-%m-%d" }}</h4>
  <h5>{{ post.description }}</h5>
{% endfor %}
--->

## Recent Posts

{% for post in site.posts %}
[{{ post.title }}]({{post.url | prepend: site.baseurl }}) - <p font-size:"0.875em"> {{ post.date  | date: "%Y-%m-%d" }} </p>
<p style="padding-left:35px;"> {{ post.description }}</p> 
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
