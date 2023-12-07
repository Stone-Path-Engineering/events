---

layout: homepage
title: Home

---

## Upcoming Event

<h3 class="category-head">{{ next }}</h3>
<a name="{{ crochet | slugize }}"></a>
{% for post in site.categories["next"] %}
  <article class="archive-item">
    <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    {{ post.excerpt }}
  </article>
{% endfor %}

## Past Events

<h3 class="category-head">{{ past }}</h3>
<a name="{{ crochet | slugize }}"></a>
{% for post in site.categories["past"] %}
  <article class="archive-item">
    <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
  </article>
{% endfor %}
