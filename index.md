---
layout: page
---
{% include JB/setup %}


<ul class="unstyled posts">
  {% for post in site.posts %}
  	{% if post.categories contains 'pages' %}
  	<li>
  		<div class="row">
  			<div class="page-header">
  				<h1>{{ post.title }} <small>{{ post.date | date_to_string }}</small></h1>
  			</div>
  			<div class="span2">
  				<a href="{{ BASE_PATH }}{{ post.url }}" class="thumbnail">
  					<img src="{{ site.url }}/blog/assets/img/postList/{{ post.img }}" alt="" />
  				</a>
  			</div>
  			<div class="span4">
  				{{ post.summary }}
  			</div>
  		</div>
  	</li>
    {% endif %}
  {% endfor %}
</ul>

