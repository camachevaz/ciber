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

{% assign vez = 0 %}
{% for post in site.posts %}
	{% increment vez %}
	{% if vez | modulo: 2 == 1 %}
		<p>Modulus: {{ vez }}</p>
		<div class="row">
	{% endif %}
	
	{% if post.title != 404 and post.category == "curso" %}
		<div class="6u 12u$(small)">
			<h3>{{ post.title }}</h3>
			{% if post.image %}
				<p><span class="image main"><img src="{{ site.baseurl }}/{{ post.image }}" alt="" /></span></p>
			{% endif %}
			<p>{{ post.description }}</p>
		</div>
	{% endif %}

	{% if vez | modulo: 2 == 0 %}
		<p>Modulus: {{ vez }}</p>
		</div>
	{% endif %}
{% endfor %}

</div>
