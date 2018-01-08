---
layout: archive
title: "可视化作品集"
date: 2017-12-30T11:40:45-04:00
categories.infovis
modified:
excerpt: 好的丶可改进的及有趣的"
tags: []
image: 
  feature: Portfolio.svg
  teaser:
---
- <a href="https://public.tableau.com/views/5_393/2_2?:embed=y&:display_count=yes&publish=yes" target="_blank">![conferm.png](https://i.loli.net/2018/01/08/5a52fe08133b7.png)</a>

<div class="tiles">
{% for post in site.categories.infovis %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles 把所有categories 有 infovis 的列出來-->

