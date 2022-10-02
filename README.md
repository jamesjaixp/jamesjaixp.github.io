---
layout: default
title: Home
---

<div class="row">
  <div class="section-one" style="background-image:url({{ site.github.url }}/images/fire.jpg)">
    <h2><span><a href="#">People Around Lit Fire</a></span></h2>
  </div>
</div>
{% for post in paginator.posts %}
  <a href="{{ site.github.url }}{{ post.url }}">
    <div class="featured-posts" {% if post.image.feature %}style="background-image:url({{ site.github.url }}/images/{{ post.image.feature }})"{% endif %}>
      <h2><span>{{ post.title }}</span></h2>

<div class="row">
  <div class="section-two col-2" style="background-image:url({{ site.github.url }}/images/tools.jpg)">
    <h2><span>Some Cool Tools</span></h2>
  </div>
  <div class="section-three col-2" style="background-image:url({{ site.github.url }}/images/forest.jpg)">
    <h2><span>Rain Drop Drop Top</span></h2>
  </div>
</div>
    <!--{% if post.image.teaser %}
      <a href="{{ site.github.url }}{{ post.url }}"><img src="{{ site.github.url }}/images/{{ post.image.teaser }}"></a>
    {% endif %}
    <h1>
      <a href="{{ site.github.url }}{{ post.url }}">{{ post.title }}</a>
    </h1>-->

<div class="row">
  <div class="section-four col-3" style="background-image:url({{ site.github.url }}/images/room.jpg)">
    <h2><span>Check Out This Room</span></h2>
  </div>
  <div class="section-five col-3" style="background-image:url({{ site.github.url }}/images/spools.jpg)">
    <h2><span>Some Cool Spools</span></h2>
  </div>
  <div class="section-six col-3" style="background-image:url({{ site.github.url }}/images/cards.jpg)">
    <h2><span>Don't Forget This</span></h2>
  </div>
</div>
    </div>
  </a>

  <!--<div class="featured-posts">
    <a href="{{ site.github.url }}{{ post.url }}"><img src="{{ site.github.url }}/images/{{ post.image.teaser }}" alt="" /><h2><span>{{ post.title }}</span></h2></a>
  </div>-->

{% endfor %}

<!-- Pagination links -->
<div class="pagination">
  {% if paginator.next_page %}
    <a class="pagination-button pagination-active" href="{{ site.github.url }}{{ paginator.next_page_path }}" class="next">Older</a>
  {% else %}
    <span class="pagination-button">Older</span>
  {% endif %}

<div class="row">
  <div class="section-six col-23" style="background-image:url({{ site.github.url }}/images/bag.jpg)">
    <h2><span>Thirst Angle</span></h2>
  </div>
  <div class="section-five col-3" style="background-image:url({{ site.github.url }}/images/sewing.jpg)">
    <h2><span>Cool Spool Fool</span></h2>
  </div>
  {% if paginator.previous_page %}
    <a class="pagination-button pagination-active" href="{{ site.baseurl }}{{ paginator.previous_page_path }}">Newer</a>
    {% else %}
      <span class="pagination-button">Newer</span>
  {% endif %}
</div>
