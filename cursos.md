---
layout: page
title: Cursos
description: Conoce la oferta educativa completa.
image: assets/images/cursos.jpg
nav-menu: true
permalink: /cursos/
---

<!-- Main -->
<div id="main" class="alt">

<!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h1>Cursos disponibles</h1>
		</header>

<!-- Content -->
{% for post in site.posts %}
	{% if post.title != 404 and post.category == "curso" %}
		<div class="12u 12u$(medium)">
			<h3>{{ post.title }}</h3>
			<p>
			{% if post.image %}
				<span class="image left"><img src="{{ site.baseurl }}/{{ post.image }}" alt="" /></span>
			{% endif %}
			{{ post.description }}</p>
		</div>
	{% endif %}
{% endfor %}

</div>
