---

layout: homepage
title: Home

---

## Upcoming Event

<a name="{{ next | slugize }}"></a>
{% for post in site.categories["next"] %}
  <article class="archive-item">
    <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    {{ post.excerpt }}
  </article>
  
  <br />
  <a href="{{ site.baseurl }}{{ post.url }}">Learn more and register...</a>

<br />
{% endfor %}

<br />
<br />
<br />
<br />

## Past Events

<h3 class="category-head">{{ past }}</h3>
<a name="{{ past | slugize }}"></a>
{% for post in site.categories["past"] limit: 10 %}
  <article class="archive-item">
    <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
  </article>
{% endfor %}
