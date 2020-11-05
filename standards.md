<ul>
{% for standard in site.data.standards %}
  <li>
    {{ standard.name }} - {{ standard.focus }}
  </li>
{% endfor %}
</ul>
