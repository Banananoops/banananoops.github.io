---
title: investment
subtitle: Personal is the perfect theme for developers, designers and other creatives.
description: Personal is the perfect theme for developers, designers and other creatives.
featured_image: /images/demo/about.jpg
---

## Features



<section class="listing">

	<div class="wrap">

		{% for project in site.projects %}

		<article class="post">

			<div class="post__image-wrap">
				<div class="post__image" style="background-image: url({{ project.featured_image | relative_url }})"></div>
			</div>

			<div class="post__content-wrap">
				<div class="post__content">
					<h2 class="post__title"><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
					<p class="post__subtitle">{{ project.subtitle }}</p>
					<p class="post__description">{{ project.description }}</p>
				</div>
			</div>

		</article>

		{% endfor %}

	</div>

</section>

