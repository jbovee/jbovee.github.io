---
layout: default
title: Skills
---

<h1>Languages</h1>

<div id="languages" class="skills">

	{% assign languages = site.skills | where:"type", "language" %}
	{% for language in languages %}

		<div class="skill">
			<svg fill="#CDEE69" width="150" height="150">

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
			<svg fill="#CDEE69" width="150" height="150">

				{{ other.content }}

			</svg>
		</div>

	{% endfor %}

</div>