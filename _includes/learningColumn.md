<ul>
	{% for post in site.posts %}
  	{% if post.categories contains 'learns' %}
   	<li><span>{{ post.date | date_to_string }}</span><span>{{ post.content }}</span></li>
    {% endif %}
  {% endfor %}
</ul>