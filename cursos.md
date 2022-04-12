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
	{% if post.title != 404 and post.category == "curso	" %}
		<header class="major">
		<h1>{{ post.title }}</h1>
		</header>
		{% if post.image %}
			<span class="image main"><img src="{{ site.baseurl }}/{{ post.image }}" alt="" /></span>
		{% endif %}
		{% if post.date %}
			<p>{{ post.date }}</p>
		{% endif %}
		<p>{{ post.content }}</p>
	{% endif %}
{% endfor %}


<h2 id="content"></h2>
<div class="row">
</div>

<hr class="major" />
</div>
