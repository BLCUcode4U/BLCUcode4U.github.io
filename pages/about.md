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

## 这里也可以找到我们~

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

## Photo Wall
<style>
.photo-wall {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  background: lightgray;
  padding: 9px;
  border: 1px solid lightgray;
  gap: 10px;
}

.photo-wall img {
  width: 100%;
  height: auto;
  border: 6px solid white;
  box-shadow:2px 2px 2px 2px gray;
}
</style>
<!-- 在以下的 div 中添加 img 即可在照片墙中添加内容 -->
<div class="photo-wall">
  <img src="../assets/images/our_photos/25317-1.jpg">
  <img src="../assets/images/our_photos/25317-2.jpg">
  <img src="../assets/images/our_photos/25324-1.jpg">
  <img src="../assets/images/our_photos/25324-2.jpg">
  <img src="../assets/images/our_photos/25328-1.jpg">
  <img src="../assets/images/our_photos/25328-2.jpg">
  <img src="../assets/images/our_photos/25328-3.jpg">
  <img src="../assets/images/our_photos/25328-4.jpg">
  <img src="../assets/images/our_photos/25328-6.jpg">
  <img src="../assets/images/our_photos/25328-5.jpg">
  <img src="../assets/images/our_photos/25328-7.jpg">
  <img src="../assets/images/our_photos/25328-8.jpg">
  <img src="../assets/images/our_photos/25328-9.jpg">
  <img src="../assets/images/our_photos/25328-10.jpg">
  <img src="../assets/images/our_photos/25328-11.jpg">
  <img src="../assets/images/our_photos/25412-1.jpg">
  <img src="../assets/images/our_photos/25412-2.jpg">
  <img src="../assets/images/our_photos/25412-3.jpg">
  <img src="../assets/images/our_photos/25412-4.jpg">
</div>

