---
layout: home
---
<ul class="projects-list">
	{% for item in site.categories.pa %}
		<li>
			<a href="{{ item.url | prepend: site.baseurl }}">
				<div class="img-wrapper">
					<img class="index-img" src="{{ item.logo | prepend: site.baseurl }}" alt="{{ item.project.title }}" />
				</div>
				<span class="h2">{{ item.title }}</span>
				<h3>{{ item.title }}</h3>
			</a>
		</li>
	{% endfor %}
</ul>
