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

<script charset="utf-8" type="text/javascript" src="//js.hsforms.net/forms/embed/v2.js"></script>
<script>
  hbspt.forms.create({
    portalId: "48052701",
    formId: "8d1eced9-d6fc-4e06-95f4-f76f736ed257",
    region: "na1"
  });
</script>

<br />
<br />

## Past Events

<h3 class="category-head">{{ past }}</h3>
<a name="{{ past | slugize }}"></a>
{% assign posts = site.posts | sort: 'date' | reverse %}
{% for post in site.categories["past"] limit: 10 %}
  <article class="archive-item">
    <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
  </article>
{% endfor %}
