---
layout: default
title: Home
datasource: site.data.standards
---

blah

page.Site title: {{ page.sitetitle }}
page.sub title: {{ page.subtitle }}

without page
Site title: {{ sitetitle }}
sub title: {{ subtitle }}

Site URL {{ site.url }}

<table>
  {% for row in {{ datasource }} %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    <tbody id="myTable">
    {% endif %}
  
    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
    </tbody>

</table>
