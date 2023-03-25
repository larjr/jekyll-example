---
layout: post
title:  "Diário: Voltando"
date:   2023-03-24 21:27:00 -0300
categories: Diário
tags: [OQueÉ Writing]
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

##  "Voltando"?

Bom, nesse momento estou tentando reiniciar meu hábito de escrita.
O principal motivo, simplesmente foi porque senti que é um grande passo para que eu aprenda concretamente um conteúdo (e aqui nasce a idéia de escrever outro post sobre "Aprender")

Nao me estenderei muito.
Esse post fica somente como um marco de retorno

**Até a próxima :smile:!**

{{ site.author_luisangelorjr.name }} - [{{site.twitter_username}}](https://twitter.com/{{site.twitter_username}})
