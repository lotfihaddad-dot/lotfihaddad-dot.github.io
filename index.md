# Problèmes MP

{% for file in site.static_files %}
  {% if file.path contains '/MP/problèmes/' and file.extname == '.pdf' %}
- [{{ file.name }}]({{ file.path | relative_url }})
  {% endif %}
{% endfor %}
