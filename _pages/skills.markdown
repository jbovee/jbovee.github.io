---
layout: default
title: Skills
---

<h1>Languages</h1>

<div id="languages" class="skills">

	{% assign languages = site.skills | where:"type", "language" | sort: 'proficiency' %}
	{% for language in languages reversed %}

		<div class="skill">
			<svg fill="#CDEE69" width="80" height="80" viewBox="0 0 128 128">

				{{ language.content }}

			</svg>
		</div>

	{% endfor %}

</div>

<h1>Others</h1>

<div id="others" class="skills">

	{% assign others = site.skills | where:"type", "other" %}
	{% for other in others %}

		<div class="skill">
			<svg fill="#CDEE69" width="80" height="80" viewBox="0 0 128 128">

				{{ other.content }}

			</svg>
		</div>

	{% endfor %}

</div>