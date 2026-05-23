---
title: 首页
layout: default
---

# {{ site.title }}

{{ site.tagline }}

<div class="article-cards">

{% for topic in site.data.topics %}
<div class="article-card">
  <h2><a href="{{ site.baseurl }}/{{ topic.slug }}">{{ topic.title }}</a></h2>
  <div class="card-date">{{ topic.date_str }}</div>
  <div class="card-excerpt">{{ topic.excerpt }}</div>
</div>
{% endfor %}

</div>
