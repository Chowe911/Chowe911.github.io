---
layout: base
title: Home
---



{% for post in site.posts %} 
* [{{ post.title }}]({{ post.url }}) 
{% endfor %}