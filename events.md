---
title: "Events"
---

{% for event in site.events %}
  <ul>
  <li>{{ event.date }}</li>
  <li>{{ event.title }}</li>
  <li>{{ event.description }}</li>
  <li>{{ event.time }}</li>
  <li>{{ event.place }}</li>
  </ul>
{% endfor %}
