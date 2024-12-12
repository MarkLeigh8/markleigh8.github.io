---
layout: page
title: "档案"
description: "Mark Leigh Trading 教育博客"
hide-in-nav: true
lang: zh-cn
permalink: /zh-cn/archive/
---
<!-- Chinese content here -->
<div class="archive-section">
  <h2>每日评论</h2>
  <ul>
    {% assign report1_files = site.static_files | where_exp: "file", "file.path contains 'mark-report/daily1'" %}
    {% assign sorted_report1 = report1_files | sort: 'modified_time' %}
    {% for file in sorted_report1 %}
      <li><a href="{{ file.path }}" target="_blank">{{ file.name }}</a></li>
    {% endfor %}
  </ul>
</div>
