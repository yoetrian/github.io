---
layout: default
--- 

{% for post in site.posts %}
<p><h1>{{ post.title }}</h1></p>
<img src="{{ post.image | prepend: site.baseurl }}" alt="{{ post.title }}" title="{{ post.title }}">
{% endfor %}