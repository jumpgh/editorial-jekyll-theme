---
layout: page
category: light
# заголовок страницы
title: Управление освещением
# краткое описание
brief: enean ornare velit lacus, ac varius enim ullamcorper eu. Proin aliquam facilisis ante interdum congue. Integer mollis, nisl amet convallis, porttitor magna ullamcorper, amet egestas mauris. Ut magna finibus nisi nec lacinia. Nam maximus erat id euismod egestas. Pellentesque sapien ac quam. Lorem ipsum dolor sit nullam.
# используемые картинки. Первая в списке используется в качестве иконки
images:
- https://media.istockphoto.com/vectors/bulb-business-develop-idea-innovation-light-management-black-color-vector-id1141073337
- /assets/images/zhang-kaiyv-Ckgyk1iIZx8-unsplash.jpg
---

<!-- Content -->
<section>
	<!-- Elements -->
	<h2 id="elements">{{ page.model }}</h2>
	<div class="row 200%">
		<!-- solution description -->
		<div class="6u 12u$(medium)">
			<h3>enean ornare velit lacus, ac varius enim ullamcorper eu</h3>
			<p>{{ page.brief }}</p>
			<p>{{ page.description }}</p>
		</div>
		<!-- solution image -->
		<div class="6u 12u$(medium)">
			<div class="11u">
				<span class="image fit"><img src="{{ page.images[1] | absolute_url }}" alt="" /></span>
			</div>
		</div>
	</div>
	<hr />
</section>