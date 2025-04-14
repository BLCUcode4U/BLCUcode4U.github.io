---
layout: page
title: About
description: OTAKU SAVE THE WORLD
keywords: BLCUcode4U
comments: true
menu: 关于
permalink: /about/
---

Looking our eyes, tell us! Tell us why！

## 这里也可以找到我们哟~

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mazhuang.org' %}
<li>
微信公众号：<br />
<img style="height:192px;width:192px;border:1px solid lightgrey;" src="{{ site.url }}/assets/images/qrcode.jpg" alt="BLCUcode4U" />
</li>
{% endif %}
</ul>


## Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
