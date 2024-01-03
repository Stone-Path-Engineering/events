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
  
  --- 
  
  <a href="{{ site.baseurl }}{{ post.url }}">Learn more and register...</h4>

{% endfor %}

## Past Events

<h3 class="category-head">{{ past }}</h3>
<a name="{{ past | slugize }}"></a>
{% for post in site.categories["past"] %}
  <article class="archive-item">
    <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
  </article>
{% endfor %}
