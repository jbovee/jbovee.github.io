---
layout: default
title: Archive
---

<div id="blog-archives">

	{% assign projects = site.projects | sort: 'order' %}
	{% for project in projects reversed %}

		<article class="project archive">

			<h1>
				<a href="{{ project.url }}">{{ project.title }}</a>
			</h1>

		</article>

	{% endfor %}

</div>
