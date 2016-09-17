---
layout: default
permalink: /calender/
title: Calender
---

<ul class="post-list">
  {% for post in site.posts reversed %}
    {% if post.categories contains "calender" %}
    <li>
      <div class="col-md-4 col-sm-4 col-xs-4">
      <div class="calender">
        <h2 class="calender__date">{{ post.date | date: "%Y" }}</h2>
          <div class="calender__item">
            {{ post.content }}
          </div>
        </div>
    </div>
      </li>
      {% endif %}
  {% endfor %}
</ul>
