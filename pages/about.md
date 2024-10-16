---
layout: page
title: About
description: 打码改变世界
keywords: yang.hong
comments: true
menu: 关于
permalink: /about/
---

我是洪洋

追求「极致代码的匠心」。


## 联系

<ul>
<li>email：<a href="mailto:yang.hong@expiol.com">yang.hong@expiol.com</a></li>
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
