---
layout: default
title: "Home"
active: "active"
permalink: /
---

<div class="row">
	<div class="col-md-12">
		<h2>Home page</h2>
	</div>
</div>

<div class="row">
	<div class="col-md-12">
		<h4>Posts</h4>
		<ul style="list-style-type: none;">
			{% for post in site.posts %}
				<li>
					<span>{{ post.date | date: "%b %d, %Y"  }}</span>
					<a href="{{ post.url }}">{{ post.title }}</a>
				</li>
			{% endfor %}
		</ul>
	</div>
</div>
