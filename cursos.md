---
layout: page
title: Servicios
description: Conoce la oferta educativa completa.
image: assets/images/cursos.jpg
nav-menu: true
permalink: /servicios/
---
{% comment %}
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
			<div class="12u 12u$(medium)">
				<p class="image left"><img src="{{ site.baseurl }}/{{ post.image }}" alt="" /></p>
				<h2>{{ post.title }}</h2>
				<p>{{ post.description }}</p>
			</div>
		</a>
	{% endif %}
</div>
{% endfor %}

</div>
{% endcomment %}


<!-- Main -->
<div id="main">

<!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h2>Nuestros servicios</h2>
		</header>
		<p>Capacitación para todo tipo de usuarios. Desde nivel organizacional para las empresas, hasta las necesidades particulares de emprendedores, estudiantes, o simplemente mejorar los hábitos personales.</p>
	</div>
</section>

<!-- Two -->
<section id="two" class="spotlights">
	<section>
		<a href="generic.html" class="image">
			<img src="{% link assets/images/cursos/ciberseguridad-principiantes.jpg %}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Ciberseguridad para principiantes</h3>
				</header>
				<p>Da los primeros pasos ser un ciudadano digital precavido.</p>
				<ul class="actions">
					<li><a href="/cursos/ciberseguridad-principiantes/" class="button">Ver más</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section>
		<a href="generic.html" class="image">
			<img src="{% link assets/images/cursos/conferencia.jpg %}" alt="" data-position="top center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Conferencia sobre ciberseguridad</h3>
				</header>
				<p>Plática concisa y amena con el objetivo de sensibilizar a los asistentes sobre la importancia de establecer medidas de protección activas en temas de ciberseguridad.</p>
				<ul class="actions">
					<li><a href="/cursos/conferencia/" class="button">Ver más</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section>
		<a href="generic.html" class="image">
			<img src="{% link assets/images/cursos/ninja-ciberseguridad.jpg %}" alt="" data-position="25% 25%" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Ninja de la seguridad</h3>
				</header>
				<p>De cero a Ninja. Curso intensivo para conocer herramientas, hábitos y aplicaciones para convertirse en un experto en protección de datos personales y confidenciales.</p>
				<ul class="actions">
					<li><a href="/cursos/ninja-seguridad/" class="button">Ver más</a></li>
				</ul>
			</div>
		</div>
	</section>
</section>

{% comment %}
<!-- Three -->
<section id="three">
	<div class="inner">
		<header class="major">
			<h2>Massa libero</h2>
		</header>
		<p>Nullam et orci eu lorem consequat tincidunt vivamus et sagittis libero. Mauris aliquet magna magna sed nunc rhoncus pharetra. Pellentesque condimentum sem. In efficitur ligula tate urna. Maecenas laoreet massa vel lacinia pellentesque lorem ipsum dolor. Nullam et orci eu lorem consequat tincidunt. Vivamus et sagittis libero. Mauris aliquet magna magna sed nunc rhoncus amet pharetra et feugiat tempus.</p>
		<ul class="actions">
			<li><a href="generic.html" class="button next">Get Started</a></li>
		</ul>
	</div>
</section>
{% endcomment %}

</div>
