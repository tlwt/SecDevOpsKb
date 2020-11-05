<ul>
{% for member in site.data.standards %}
  <li>
    {{standard.name}} - {{standard.description}}
  </li>
{% endfor %}
</ul>
