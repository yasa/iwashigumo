---
title: Könyvarchívum
layout: base
---
<div class="archives">
  <div class="index">
    <h2><em>Könyvarchívum</em></h2>
    <ul>
      {% for post in site.posts %}
        <li>
          <a href="{{ post.url }}" title="{{ post.title }}">
            <span class="date">
              <span class="year">{{ post.date | date: '%Y' }}. </span>
              <span class="month">{{ post.date | date: '%m' }}. </span>
              <span class="day">{{ post.date | date: '%d' }}.</span>
            </span>
            <span class="title">{{ post.title }}</span>
          </a>
        </li>
      {% endfor %}
    </ul>
  </div> <!-- /.index -->
</div>
