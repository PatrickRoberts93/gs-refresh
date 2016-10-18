---
layout: default
permalink: /calender/
title: Calender
---

<ul class="post-list">
  {% for post in site.posts reversed %}
    {% if post.categories contains "calender" %}
    <li>
      <div class="calender__item">
        <h2 class="calender__date">{{ post.date | date: "%Y" }}</h2>
          <div class="calender__content">
            {{ post.content }}
          </div>
    </div>
      </li>
      {% endif %}
  {% endfor %}
</ul>
