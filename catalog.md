---
layout: page
title: Catalog
---

<!-- Posts Title List-->
<ul>

	{% for post in site.posts %}

	<li>
   <a href="{% if site.baseurl == '/' %}{{ post.url }}{% else %}{{ post.url | prepend: site.baseurl }}{% endif %}">{{ post.title }}</a>
	</li>

	{% endfor %}

</ul>

<br>