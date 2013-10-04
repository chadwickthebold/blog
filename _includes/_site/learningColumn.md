<ul>
	{% for post in site.posts %}
  	{% if post.categories contains 'learns' %}
   	<li><span>{{ post }}</a></li>
    {% endif %}
  {% endfor %}
</ul>