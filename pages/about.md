---
layout: page
title: About
description: 代码改变世界
keywords: MSZ开发者社区,开发者社区,闵行区实验高级中学,闵行实高,MSZDG,mszdg
comments: true
menu: 关于
permalink: /about/
---

当你试图解决一个你不理解的问题时,复杂化就产成了。

生命太短暂,不要去做一些根本没有人想要的东西。

坚信熟能生巧，努力改变人生。

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mazhuang.org' %}
{% endif %}
</ul>


## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
