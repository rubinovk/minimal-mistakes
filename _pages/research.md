---
layout: archive
title: "Research" 
permalink: /research/
header:
  image: header-code.jpg
  caption: "Photo credit: [Designed by Freepik](http://www.freepik.com)"
---

{% include base_path %}

<h3 class="archive__subtitle">Recent work</h3>

{% include group-by-array collection=site.posts field="categories" %}

<div class="grid__wrapper">

{% for category in group_names %}
  <!-- all except research -->
  {% if category contains site.research %}
    {% assign posts = group_items[forloop.index0] %}
    {% for post in posts %}
    {% include archive-single.html type="grid" %}
    {% endfor %}
  {% endif %}
{% endfor %}

</div>
