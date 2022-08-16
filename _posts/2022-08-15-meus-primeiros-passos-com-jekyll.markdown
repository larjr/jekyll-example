---
layout: post
title:  "Meus primeiros passos com Jekyll"
date:   2022-08-15 17:00:00 -0300
categories: jekyll tutorial
---
Ola pessoas!

Aqui é o Luís!

Simplesmente estou fazendo o meu **primeiro post** no Blog **{{ site.title }}**. Dessa forma quero testar algumas coisas que o **Jekyll** consegue nos ajudar nessa jornada.

{% highlight java %}
String saudacao = "Ola Mundo!";
System.out.println(saudacao);
{% endhighlight %}

{{ site.title }}, {{ site.email }}


----


{{ author_luisangelorjr.name }} and {{ author_luisangelorjr.age }} and too {{ author_luisangelorjr }}

## Adicionais

### Emojis

Adicionando a seguinte gem:

{% highlight bash %}
bundle add jemoji
{% endhighlight %}

E adicionar a seguinte linha ao seu ```_config.yml```:

{% highlight yaml %}
plugins:
  - jemoji
{% endhighlight %}

Para ter um sorisso :smile:

```
:smile:
```

Para ter um joinha :+1:

```
:+1:
```