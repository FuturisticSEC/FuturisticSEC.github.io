{% capture path %}_pages/{{ page.include }}{% endcapture %}
{% for node in site.pages %}
	{% if node.path == path %}
		{{ node.content }}
	{% endif %}
{% endfor %}