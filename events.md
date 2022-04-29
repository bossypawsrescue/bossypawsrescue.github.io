---
title: "Events"
permalink: /events
---

# {{ page.title }}

<section id="events">
{% for event in site.events %}
<section class="event">
  <h2 class="event-date">{{ event.date | date: "%m/%d/%Y" }}</h2>
  <strong class="event-title">{{ event.title }}</strong>
  <span class="event-time">{{ event.time }}</span>
  <a class="event-location" href="https://www.google.com/maps/search/?api=1&query={{ event.place | url_encode }}">{{ event.place }}</a>
  <span class="event-description">{{ event.description }}</span>
</section>
{% endfor %}
</section>
