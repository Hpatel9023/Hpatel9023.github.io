---
layout: page
permalink: /publications/
title: Fun Facts
description: I will be giving a few fun facts about me.
nav: true
---

<div class="">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
