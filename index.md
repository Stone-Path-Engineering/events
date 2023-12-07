---

layout: homepage
title: Home

---

## Upcoming Event

### **To be announced soon!**

## Past Events

{% for tag in site.tags %}
  {% if tag[0] == "past" %}
    {% for post in tag[1] %}
      <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
      </li>
    {% endfor %}
  {% endif %}
{% endfor %}
