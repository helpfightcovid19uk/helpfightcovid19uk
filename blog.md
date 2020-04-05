---
layout: default
title: Blog
---

<h1>Latest Posts</h1>

{% for post in site.posts %}
<div class="card">
	<div class="card-body">
		<h5 class="card-title">{{ post.title }}</h5>
		<p class="card-text">{{ post.excerpt }}</p>
		<a href="{{ post.url }}" class="stretched-link"></a>
	</div>
	<div class="card-footer text-muted">
		Posted by {{ post.author }} on {{ post.date | date_to_string }}
	</div>
</div>
{% endfor %}


