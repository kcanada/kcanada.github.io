---
layout: page
permalink: /publications/
title: publications
description:
years: [2017, 2018, 2019, 2020, 2021]
nav: true
---
<span style="font-size: 1.2em">You can find my full CV listing manuscripts under review or in preparation [here](https://kcanada.github.io/assets/pdf/Canada_Kelsey_CV_21.pdf){:target="\_blank"}.</span>

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
