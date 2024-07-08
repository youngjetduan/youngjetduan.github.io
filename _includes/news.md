{% for item in include.dataset %}

  {% if item.type == "paper" %}
    <li> 
      <strong>[{{ item.date }}]</strong> 1 paper on {{ item.title }}
      {% if item.status == "submitted" %}submitted to{% else %}accepted by{% endif %}
      <a href="{{ item.url }}" target="_blank">{{ item.venue }}</a>{% if item.role %} as {{ item.role }}!{% else %}!{% endif %}
      {% if item.award %}<i style="color:#e74d3c"><b>{{ item.award }}</b></i>{% endif %}
    </li>
  {% elsif item.type == "joined" %}
    <li>
      <strong>[{{ item.date }}]</strong> Joined <a href="{{ item.url }}" target="_blank">{{ item.org }}</a> as {{ item.role }}.
    </li>
  {% endif %}

{% endfor %}
