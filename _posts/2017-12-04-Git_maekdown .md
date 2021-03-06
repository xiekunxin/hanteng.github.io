---
layout: article
title:  "Markdown语法说明"
date:   2017-12-29 21:45:50 +0800
categories: portfolio
image:
  teaser: float.jpg 
  feature: float.jpg
---
Aaron Swatz 就是一个盗火的普罗米修斯，为这个世界带来了Markdown

{% include toc.html %}

## 关于Markdown的概述

Markdown 的目标是实现「易读易写」。

不过最需要强调的便是它的可读性。一份使用 Markdown 格式撰写的文档应该可以直接以纯文本发布，并且看起来不会像是由许多标签或是格式指令所构成。
Markdown 语法受到一些既有 text-to-HTML 格式的影响，包括 Setext、atx、Textile、reStructuredText、Grutatext 和 EtText，然而最大灵感来源其实是纯文本的电子邮件格式。

因此 Markdown 的语法全由标点符号所组成，并经过严谨慎选，是为了让它们看起来就像所要表达的意思。
像是在文字两旁加上星号，看起来就像*强调*。Markdown 的列表看起来，嗯，就是列表。假如你用过电子邮件，区块引言看起来就真的像是引用一段文字。


## 行内 HTML
Markdown 的语法有个主要的目的：用来作为一种网络内容的写作用语言。

Markdown 不是要来取代 HTML，甚至也没有要和它相似，它的语法种类不多，只和 HTML 的一部分有关系，重点不是要创造一种更容易写作 HTML 文档的语法，Markdown 的重点在于，它能让文档更容易阅读、编写。
HTML 是一种发布的格式，Markdown 是一种编写的格式，因此，Markdown 的格式语法只涵盖纯文本可以涵盖的范围。

不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。不需要额外标注这是 HTML 或是 Markdown；只要直接加标签就可以了。

只有区块元素──比如 <div>、<table>、<pre>、<p> 等标签，必需在前后加上空白，以利与内容区隔。而且这些（元素）的开始与结尾标签，不可以用 tab 或是空白来缩排。
Markdown 的产生器有智能判断，可以避免在区块标签前后加上没有必要的 <p> 标签。
请注意，Markdown 语法在 HTML 区块标签中将不会被进行处理。例如，无法在 HTML 区块内使用 Markdown 形式的*强调*。

HTML 的区段标签如 <span>、<cite>、<del> 则不受限制，可以在 Markdown 的段落、列表或是标题里任意使用。
依照个人习惯，甚至可以不用Markdown 格式，而采用 HTML 标签来格式化。
举例说明：如果比较喜欢 HTML 的 <a> 或 <img> 标签，可以直接使用这些标签，而不用 Markdown 提供的链接或是图片标示语法。
HTML 区段标签和区块标签不同，在区段标签的范围内， Markdown 的语法是有效的。

## 特殊字符自动转换
在 HTML 文档中，有两个字符需要特殊处理： < 和 & 。 < 符号用于起始标签，& 符号则用于标记 HTML 实体，如果只是想要使用这些符号，必须要使用实体的形式，像是 &lt; 和 &amp;。

& 符号其实很让写作网络文档的人很困扰，如果要输入「AT&T」 ，必须要写成「AT&amp;T」 ，还得转换网址内的 & 符号。
不过需要注意的是，code 范围内，不论是行内还是区块， < 和 & 两个符号都一定会被转换成 HTML 实体，这项特性让你可以很容易地用 Markdown 写 HTML code （和 HTML 相对而言， HTML 语法中，要把所有的 < 和 & 都转换为 HTML 实体，才能在 HTML 文档里面写出 HTML code。）

