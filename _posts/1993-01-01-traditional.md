---
layout: home
permalink: /tradicional/
category: pa
title: Tradicional
logo: /assets/images/projects/wonderwoman.jpg
---
<ul class="projects-list">
	{% for item in site.categories.traditional %}
		<li>
			<a href="{{ item.url | prepend: site.baseurl }}">
				<div class="img-wrapper">
					<img class="index-img" src="{{ item.project.logo | prepend: site.baseurl }}" alt="{{ item.project.title }}" />
				</div>
				<span class="h2">{{ item.project.type }}</span>
				<h3>{{ item.project.title }}</h3>
			</a>
		</li>
	{% endfor %}
</ul>
