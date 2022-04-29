---
title: "Events"
permalink: /events
---

# {{ page.title }}

{% for event in site.events %}
<section>
  <h2>{{ event.date | date: "%m/%d/%Y" }}</h2>
  <strong>{{ event.title }}</strong>
  <p>
  <span>{{ event.time }}</span>
  <a href="https://www.google.com/maps/search/?api=1&query={{ event.place | url_encode }}">{{ event.place }}</a>
  </p>
  <p>{{ event.description }}</p>
</section>
{% endfor %}
