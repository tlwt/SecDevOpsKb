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

Nav
{% for entry in site.pages.standards %}
  <h2>entry {{ entry.title }} - {{ staff_member.datasource }}</h2>
{% endfor %}
