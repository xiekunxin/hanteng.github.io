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
<img src="https://xiekunxin.github.io/images/jie.png" alt="teaser" itemprop="image">

<div class="tiles">
{% for post in site.categories.infovis %}
  {% include post-grid.html %}
{% endfor %}
<<<<<<< HEAD
</div><!-- /.tiles 把所有categories 有 infovis 的列出來-->

