---
layout: archive
permalink: / 
header:
  image: header-code.jpg
  caption: "Photo credit: [Designed by Freepik](http://www.freepik.com)"
---

{% include base_path %}

<section class="page__content" itemprop="text" markdown="1">

Hi there, this is __Konstantin__. Here you will find a collection of my [research]({{ base_path }}/research/), opinions and observations
{: .text-justify}

</section>

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

<div class="grid__wrapper">
{% for post in site.posts %}
      {% include archive-single-main.html type="grid" %} 
{% endfor %}
</div>



