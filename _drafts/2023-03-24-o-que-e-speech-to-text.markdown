---
layout: post
title:  "OQueÉ: Speech-to-text"
date:   2023-03-24 20:34:00 -0300
categories: OQueÉ AI
tags: [OQueÉ AI speech-to-text APIs]
---
<div class="post-categories">
  {% if post %}
    {% assign categories = post.categories %}
  {% else %}
    {% assign categories = page.categories %}
  {% endif %}
  {% for category in categories %}
  <a href="{{site.baseurl}}/categorias/#{{category|slugize}}">{{category}}</a>
  {% unless forloop.last %}&nbsp;{% endunless %}
  {% endfor %}
</div>

------

## h2
### h3
#### h4
##### h5
###### h6
teste