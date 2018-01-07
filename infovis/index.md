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
## 中国宗教场所分布情况
####  ==数据来源==：[国家数据](http://data.stats.gov.cn/)
<iframe src="https://public.tableau.com/views/5_393/1_2?:embed=y&:display_count=yes/sheet4?:embed=y&:display_count=yes&publish=yes/Dashboard1?:showVizHome=no&:embed=truehttps://public.tableau.com/shared/DJPSG6CX9?:display_count=yes" width="850px" height="900px" frameborder="0"></iframe>

<div class="tiles">
{% for post in site.categories.infovis %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles 把所有categories 有 的列出來-->
