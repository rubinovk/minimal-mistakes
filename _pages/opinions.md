---
layout: archive
title: "Opinions"
permalink: /opinions/
header:
  image: header-code.jpg
  caption: "Photo credit: [Designed by Freepik](http://www.freepik.com)"
---

{% include base_path %}


<div class="page__inner-wrap">
<section class="page__content" itemprop="text">

<h3 class="archive__subtitle">Work in progress</h3>
<h2 class="archive__item-title" itemprop="headline">
<a href="{{ base_path }}/library/">Personal Library -></a>
</h2>

<small>Sharing my notes on books and reading</small>

</section>
</div>


<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

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
