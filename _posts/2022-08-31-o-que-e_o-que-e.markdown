---
layout: post
title:  "OQueÉ: OQueÉ"
date:   2022-08-31 12:00:00 -0300
categories: OQueÉ
tags: [OQueÉ]
---

<div class="post-categories">
categorias: 
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


> Sim, voce entrou num loop recursivo sim, voce entrou num loop recursivo sim, voce...
>> **Uma piada recursivamente encontrada em grupos de devs**

Ola, eu sou o {{site.author_luisangelorjr.name}}, mas geralmente vcs irao me achar na internet como {{site.author_luisangelorjr.nickname}}


## O que eh "OQueÉ"

A minha ideia ao criar a categoria do "**OQueÉ**"" 'e tentar responder quest'oes r'apidas de quem procurou algo no Google  e s'o precisa de um tira-d'uvidas sucinto sem muitos detalhes complexos, mas j'a conseguindo reconhecer o prop'osito inicial do termo buscado, bem como uma superficial vis'ao de como us'a-lo.

Com isso, tive que bolar um nome que nao ficasse ruim e facil de lembrar...logo surgiu o **OQueÉ**

![Uma captura de tela mostrando a disposicao da url, t'itulo e categoria do **OQueÉ**]({{site.baseurl}}/assets/img/captura-de-tela-exemplo-oquee.jpg)


Como podemos ver no print acima, tanto a url, t'itulo e categoria est'ao aceit'aveis

### Por que essa categoria nasceu?

Percebi que eu posso ser muito prolixo (falo/escrevo demais as vezes hasudhasudhu).

Com isso, tendo alguns limites, consigo focar e deixar o post com uma melhor qualidade e sem ser um eterno trabalho n'ao publicado.

:smile:

## FIM

'E isso!

Para ter acesso a outros posts sobre **OQueÉ** acesse: <a href="{{site.baseurl}}/categorias/#OQueÉ">OQueÉ</a>


