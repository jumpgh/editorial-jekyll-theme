---
layout: page
title: Оборудование
---

<!-- Section -->
{%- for category in site.productCategories -%}
<section>
	<header class="major" id="{{category[0]}}">
		<h3>{{category[1].name}}</h3>
		<p>{{category[1].description}}</p>
	</header>
	<div class="posts">
		{% assign products = site.products | where: "category", category[0] %}
		{%- for product in products -%}
		<article>
			<a href="#" class="image"><img src="{{ product.images[0] }}" alt="" /></a>
			<h3>{{ product.model }}</h3>
			<p>{{ product.brief }}</p>
			<ul class="actions">
				<li><a href="{{site.baseurl}}/{{ product.url }}" class="button">подробнее</a></li>
			</ul>
		</article>
		{%- endfor -%}
	</div>
</section>
{%- endfor -%}
