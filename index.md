---
layout: default
--- 

{% for post in site.posts %}
<p><h2><a href="{{ post.url }}">{{ post.date | date: "%-d %B %Y" }} - {{ post.title }}</a></h2></p>
{{ post.description }}
<a href="{{ post.image }}"><img src="{{ post.image | prepend: site.baseurl }}" alt="{{ post.title }}" title="{{ post.title }}"></a>
{% endfor %}