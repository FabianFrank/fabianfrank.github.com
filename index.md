---
layout: default
title: Fabian's Blog
tagline: What doesn't fit in a tweet
---
{% include JB/setup %}



{% for post in site.posts %}
  {% assign content = post.content %}
  <div class="row-fluid post-full">
    <h1 class="entry-title">
    <a href="{{ root_url }}{{ post.url }}">{{ post.title }}</a>
    </h1>
    <div class="date">
      <span><a href="https://plus.google.com/+FabianFrank?rel=author" rel="author">Fabian Frank</a> on {{ post.date | date_to_long_string }}</span>
    </div>
    <div class="entry-content">{{ content }}</div>
  </div>
  {% if forloop.last == false %}
  <hr>
  {% endif %}
{% endfor %}

