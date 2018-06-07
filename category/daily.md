---
layout: category
title: daily
permalink: /daily/
---

<h1 class="page-title">{{ page.title | escape }}</h1>

<div class="section">
    <div style="background: #ddd">
        <div class="container last-post">
        <section>
            <h5>일상..</h5>
            {% assign category = page.category | default: page.title %} <!-- 같은 title 찾기 -->
            
            <ul class="collection">
             {% for post in site.categories[category] %}
              <li class="collection-item avatar">
                {% assign date_format = site.minima.date_format | default: "%m/%d" %}
                <div class="date-post">{{ post.date | date: date_format }}</div>
                <span class="title"><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></span>
                <p>
                   {{ post.content | truncatewords: 10 }}
                </p>
                <a href="{{ post.url | relative_url }}" class="secondary-content"><i class="material-icons">navigate_next</i></a>
              </li>
              {% endfor %}
            </ul>
        </section>
     </div>
</div>
