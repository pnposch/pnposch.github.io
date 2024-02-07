---
layout: gpx
title: GPX
---



{% for ride in site.rides %}
  <a href="{{ ride.url | prepend: site.baseurl }}">
    <div>
      <time datetime="{{ ride.date }}">{{ ride.date | date: "%B %d, %Y" }}</time>
      <h2>{{ ride.title }}</h2>
    </div>
  </a>
{% endfor %}