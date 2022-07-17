---
layout: page
title: Blog
---

Welcome to my blog! I write about things that I might find interesting. Have a look at some of my recent posts:

{% for post in site.posts reversed %}

<div markdown="1">

## [{{ post.title }}]({{ post.url }})
{{ post.content | strip_html | truncatewords: 50 }}

</div>

{% endfor %}
