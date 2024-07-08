<div class="educations">
<ol class="afflication">

{% for link in include.dataset %}

<li>
<div class="edu-row">
  <div class="col-sm-3" style="position: relative;padding-left: 5px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" width="50px">
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title">{{ link.title }}</div>
      <div class="details">{{ link.position }} in {{ link.field }} <t style="float:right">{{link.start}} - {{ link.end }}</t></div>
      <div class="advisor">Advisor: {{ link.advisor }}</div>
  </div>

</div>
</li>

<br>

{% endfor %}

</ol>
</div>
