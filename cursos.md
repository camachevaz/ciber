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
<div class="row">
	{% if post.title != 404 and post.category == "curso" %}
		<a href="{{ post.url | absolute_url }}">
			<div class="8u 8u$(medium)">
				<p class="image left"><img src="{{ site.baseurl }}/{{ post.image }}" alt="" /></p>
				<h2>{{ post.title }}</h2>
				<p>{{ post.description }}</p>
			</div>
		</a>
	{% endif %}
</div>
{% endfor %}

</div>
