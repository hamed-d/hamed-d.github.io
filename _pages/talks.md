---
layout: page
permalink: /talks/
title: talks
description: Invited and conference talks.
nav: true
nav_order: 4
---

<!-- Lists the _talks collection, newest first. Each talk sets year, event, talk_type and description. -->
{% assign talks_by_year = site.talks | sort: 'year' | reverse | group_by: 'year' %}
{% if talks_by_year.size > 0 %}
  {% for year_group in talks_by_year %}
    <h2 class="year">{{ year_group.name }}</h2>
    <ul class="post-list">
      {% for talk in year_group.items %}
        <li>
          <h3><a class="post-title" href="{{ talk.url | relative_url }}">{{ talk.title }}</a></h3>
          <p class="post-meta">{{ talk.talk_type }} &middot; {{ talk.event }}</p>
        </li>
      {% endfor %}
    </ul>
  {% endfor %}
{% else %}
  <p>No talks listed yet.</p>
{% endif %}
