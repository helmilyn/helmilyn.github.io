---
layout: gallery
permalink: /
title: UI/UX design
---
{% for item in site.ui-ux-design %}

<div class="h-64 relative">
	<a href="{{ item.url }}">
		<div class="absolute inset-0 z-0 bg-cover bg-center" style="background-image: url('{{ item.thumbnail_url }}')"></div>
		<div class="absolute inset-0 z-10 opacity-0 hover:opacity-100 duration-300 flex justify-center items-center text-2xl text-white bg-gray-800/75">
			{{ item.title }}
		</div>
	</a>
</div>

{% endfor %}
