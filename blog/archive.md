---
title: Archive
layout: blog
---

# Archive

<ul id="listing-archive">
	{% for post in site.posts %}
		{% if post.hidden != true %}
			<li>
				<time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date_to_string }}</time> - 
				<a href="{{ post.url }}">{{ post.title }}</a>
			</li>
		{% endif %}
	{% endfor %}
</ul>
