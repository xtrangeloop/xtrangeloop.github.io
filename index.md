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

  <p style="padding-left:35px;"> {{ post.description }}</p> 
{% endfor %}
--->

### Recent Posts

{% for post in site.posts %}
* {{ post.date  | date: "%Y-%m-%d" }} - [{{ post.title }}]({{post.url | prepend: site.baseurl }}) - {{ post.description }}
{% endfor %}
