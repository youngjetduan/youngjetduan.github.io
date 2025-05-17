---
layout: homepage
---

<h2 style="margin: -10px 0px 5px;">About Me</h2>
{% include_relative _includes/aboutme.md %}

<h2 style="margin: -10px 0px 5px;">Educations</h2>
{% include_relative _includes/educations.md dataset=site.data.educations.main %}

<h2 style="margin: -10px 0px 5px;">News</h2>
<div style="height: 200px; overflow: auto; margin-bottom: 20px;">
<ul>
{% include_relative _includes/news.md dataset=site.data.news.main %}
</ul>
</div>

<details>
<summary style="cursor: pointer; display: flex; align-items: center; list-style: none;">
<h2 style="margin: -10px 0px 5px; flex-grow: 1;">Preprints</h2>
<span class="toggle-icon"></span>
</summary>
{% include_relative _includes/publications.md dataset=site.data.preprints.main %}
</details>

<details>
<summary style="cursor: pointer; display: flex; align-items: center; list-style: none;">
<h2 style="margin: 0px 0px 5px; flex-grow: 1;">Publications</h2>
<span class="toggle-icon"></span>
</summary>
{% include_relative _includes/publications.md dataset=site.data.publications.main %}
</details>

<h2 style="margin: 0px 0px 5px;">Services</h2>
{% include_relative _includes/services.md %}

<h2 style="margin: -10px 0px 5px;">Awards and Honors</h2>
{% include_relative _includes/awards.md dataset=site.data.awards.main %}
