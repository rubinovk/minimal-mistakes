---
layout: archive
title: "Opinions"
permalink: /opinions/
header:
  image: header-code.jpg
  caption: "Photo credit: [Designed by Freepik](http://www.freepik.com)"
---

{% include base_path %}

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

TODO: CORRECT GROUPING BY DATE. SHOW TAGS?

{% include group-by-array collection=site.posts field="categories" %}

{% for category in group_names %}
  <!-- all except research -->
  {% unless category contains site.research %}
    {% assign posts = group_items[forloop.index0] %}
    {% for post in posts %}
      {% include archive-single.html %}
    {% endfor %}
  {% endunless %}
{% endfor %}
