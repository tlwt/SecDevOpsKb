---
layout: default
title: Home
datasource: standards
---

blah

page.Site title: {{ page.sitetitle }}
page.sub title: {{ page.subtitle }}

without page
Site title: {{ sitetitle }}
sub title: {{ subtitle }}

Site URL {{ site.url }}

inspect: {{ site.pages.standards | inspect }}

Nav
{% for entry in site.pages %}
  <h2>entry {{ entry.title }} - {{ entry.name }}</h2>
{% endfor %}
