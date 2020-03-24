---
layout: page
title: Решения
---

<!-- Section -->
{%- for category in site.solutionCategories -%}
<section>
	<header class="major" id="{{category[0]}}">
		<h3>{{category[1].name}}</h3>
		<p>{{category[1].description}}</p>
	</header>
	{% assign solutions = site.solutions | where: "category", category[0] %}
	{%- for solution in solutions -%}
	<div class="row">
		<div class="2u">
			<span class="image fit"><img src="{{ solution.images[0] }}" alt="" /></span>
		</div>
		<div class="10u">
			<h4>{{ solution.title }}</h4>
			<p>{{ solution.brief }}&nbsp;<span><a href="{{site.baseurl}}/{{solution.url}}">Подробно</a></span></p>
		</div>
	</div>
	{%- endfor -%}
</section>
{%- endfor -%}