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
  <div class="card-links">
    <a href="{{ site.baseurl }}/{{ topic.slug }}/article_fr">📖 法语文稿</a>
    <a href="{{ site.baseurl }}/{{ topic.slug }}/article_cn">📖 中文文稿</a>
    <a href="{{ site.baseurl }}/{{ topic.slug }}/annotations">📝 注释与学习指南</a>
    <a href="{{ site.baseurl }}/{{ topic.slug }}/glossary">📊 术语表</a>
  </div>
</div>
{% endfor %}

</div>
