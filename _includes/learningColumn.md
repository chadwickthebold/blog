<h3>Today I Learned...</h3>

<ul>
	{% for post in site.posts %}
  	{% if post.categories contains 'learns' %}
   	<li><span>{{ post.date | date_to_string }}</span><br>
   	<span>{{ post.content }}</span></li>
   	{% endif %}
  {% endfor %}
</ul>