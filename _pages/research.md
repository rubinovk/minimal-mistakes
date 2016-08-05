---
layout: archive
title: "Research" 
permalink: /research/
header:
  image: header-code.jpg
  caption: "Photo credit: [Designed by Freepik](http://www.freepik.com)"
---

{% include base_path %}


<section class="page__content" itemprop="text" markdown="1">


My research is an interplay between __understanding software__
and using this understanding to impact software processes, software artifacts,
and, ultimately, __software quality__. In particular, in my PhD research I
harnessed the knowledge about software systems incorporated in existing test
cases to drive the __automatic generation__ of new complex test cases at a low
cost. In my post-doctoral research I employ __program analysis__ to gain insights
into program properties to drive software testing for complex real-world
program binaries and __mobile applications__, and to develop systems with __high
quality and security guarantees__.
{: .text-justify}

> "Nothing in life is to be feared, it is only to be understood. Now is the time to understand more, so that we may fear less."

<cite>Madame Marie Curie</cite> (1867-1934) 
{: .small}

</section>


<h3 class="archive__subtitle">Recent work</h3>

{% include group-by-array collection=site.posts field="categories" %}

<div class="cf"> 
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
</div>

<section class="page__content" itemprop="text" markdown="1">

> "Nothing in life is to be feared, it is only to be understood. Now is the time to understand more, so that we may fear less."

<cite>Madame Marie Curie</cite> (1867-1934) 
{: .small}

</section>
