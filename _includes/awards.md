{% for item in include.dataset %}

  <li> {{ item.year }} {{ item.title }}, {{ item.affiliation }} </li>

{% endfor %}
