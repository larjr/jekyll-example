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

String saudacao = "Ola Mundo!";
System.out.println(saudacao);

{{ site.title }}, {{ site.email }}


----

# Título <h1> (como podemos ver...ele nao recebe o tamanho correto em relacao ao h2)
## Título <h2>
### Título <h3>
#### Título <h4>
##### Título <h5>
###### Título <h6>

{% highlight markdown %}
# Título <h1> (como podemos ver...ele nao recebe o tamanho correto em relacao ao h2)
## Título <h2>
### Título <h3>
#### Título <h4>
##### Título <h5>
###### Título <h6>
{% endhighlight %}

```markdown
# Título <h1> (como podemos ver...ele nao recebe o tamanho correto em relacao ao h2)
## Título <h2>
### Título <h3>
#### Título <h4>
##### Título <h5>
###### Título <h6>
```

{{ site.author_luisangelorjr.name }} and {{ site.author_luisangelorjr.age }} and too {{ site.author_luisangelorjr }}

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
Teste de um gist
<script src="https://gist.github.com/luisangelorjr/d31ed68f221f4b60588a4fe12fb73e1b.js"></script>

----

Teste usando Carbon

![teste](blob:https://carbon.now.sh/99ed7b44-02a1-45d2-8b46-07fa651da836)


![carbon plain url](https://carbon.now.sh/?bg=rgba%28248%2C231%2C28%2C1%29&t=3024-night&wt=none&l=auto&width=680&ds=true&dsyoff=20px&dsblur=68px&wc=true&wa=true&pv=56px&ph=56px&ln=true&fl=1&fm=Fira+Code&fs=14px&lh=152%25&si=false&es=2x&wm=false&code=class%2520Main%2520%257B%250A%2520%2520public%2520static%2520void%2520main%28String%255B%255D%2520args%29%2520%257B%250A%2520%2520%2520%2520%2520%2520%2520%2520int%2520NumInt%253B%250A%2520%2520%2520%2520%2520%2520%2520%2520double%2520NumReal%252C%2520soma%253B%250A%2520%2520%2520%2520%2520%2520%2520%2520char%2520Caracter%253B%250A%2520%2520%2520%2520%2520%2520%2520%2520String%255B%255D%2520entrada%2520%253D%2520new%2520String%255B%255D%257B%25221%2522%252C%2520%25222.5%2522%252C%2520%2522L%2522%257D%253B%250A%2520%2520%2520%2520%250A%2520%2520%2520%2520%2520%2520%2520%2520%252F%252Fentrada%2520de%2520dados%250A%2520%2520%2520%2520%2520%2520%2520%2520NumInt%2520%253D%2520Integer.parseInt%28entrada%255B0%255D%29%253B%2520%250A%2520%2520%2520%2520%2520%2520%2520%2520NumReal%2520%253D%2520Double.parseDouble%28entrada%255B1%255D%29%253B%250A%2520%2520%2520%2520%2520%2520%2520%2520Caracter%2520%253D%2520%28entrada%255B2%255D%29.charAt%280%29%253B%2520%252F%252F%2520converte%2520o%2520terceiro%2520digito%2520em%2520caracter%250A%2520%2520%2520%2520%2520%2520%2520%250A%2520%2520%2520%2520%2520%2520%2520%2520soma%2520%253D%2520%28double%29NumInt%2520%252B%2520NumReal%253B%250A%2520%2520%2520%2520%2520%2520%2520%2520%250A%2520%2520%2520%2520%2520%2520%2520%2520System.out.println%28%28double%29NumInt%2520%252B%2520%2522%2520%252B%2520%2522%2520%252B%2520NumReal%2520%252B%2520%2522%2520%253D%2520%2522%2520%252B%2520soma%2520%252B%2520%2522%2520sinal%2520%2522%2520%252B%2520Caracter%29%253B%250A%2520%2520%2520%2520%2520%2520%2520%2520System.exit%280%29%253B%250A%2520%2520%257D%250A%257D)

<iframe
  src="https://carbon.now.sh/embed?bg=rgba%28248%2C231%2C28%2C1%29&t=3024-night&wt=none&l=auto&width=680&ds=true&dsyoff=20px&dsblur=68px&wc=true&wa=true&pv=56px&ph=56px&ln=true&fl=1&fm=Fira+Code&fs=14px&lh=152%25&si=false&es=2x&wm=false&code=class%2520Main%2520%257B%250A%2520%2520public%2520static%2520void%2520main%28String%255B%255D%2520args%29%2520%257B%250A%2520%2520%2520%2520%2520%2520%2520%2520int%2520NumInt%253B%250A%2520%2520%2520%2520%2520%2520%2520%2520double%2520NumReal%252C%2520soma%253B%250A%2520%2520%2520%2520%2520%2520%2520%2520char%2520Caracter%253B%250A%2520%2520%2520%2520%2520%2520%2520%2520String%255B%255D%2520entrada%2520%253D%2520new%2520String%255B%255D%257B%25221%2522%252C%2520%25222.5%2522%252C%2520%2522L%2522%257D%253B%250A%2520%2520%2520%2520%250A%2520%2520%2520%2520%2520%2520%2520%2520%252F%252Fentrada%2520de%2520dados%250A%2520%2520%2520%2520%2520%2520%2520%2520NumInt%2520%253D%2520Integer.parseInt%28entrada%255B0%255D%29%253B%2520%250A%2520%2520%2520%2520%2520%2520%2520%2520NumReal%2520%253D%2520Double.parseDouble%28entrada%255B1%255D%29%253B%250A%2520%2520%2520%2520%2520%2520%2520%2520Caracter%2520%253D%2520%28entrada%255B2%255D%29.charAt%280%29%253B%2520%252F%252F%2520converte%2520o%2520terceiro%2520digito%2520em%2520caracter%250A%2520%2520%2520%2520%2520%2520%2520%250A%2520%2520%2520%2520%2520%2520%2520%2520soma%2520%253D%2520%28double%29NumInt%2520%252B%2520NumReal%253B%250A%2520%2520%2520%2520%2520%2520%2520%2520%250A%2520%2520%2520%2520%2520%2520%2520%2520System.out.println%28%28double%29NumInt%2520%252B%2520%2522%2520%252B%2520%2522%2520%252B%2520NumReal%2520%252B%2520%2522%2520%253D%2520%2522%2520%252B%2520soma%2520%252B%2520%2522%2520sinal%2520%2522%2520%252B%2520Caracter%29%253B%250A%2520%2520%2520%2520%2520%2520%2520%2520System.exit%280%29%253B%250A%2520%2520%257D%250A%257D"
  style="width: 1024px; height: 590px; border:0; transform: scale(1); overflow:hidden;"
  sandbox="allow-scripts allow-same-origin">
</iframe>

---

![imgurl](https://imgur.com/M9RUaqg)

---

![imgrurl .png](https://i.imgur.com/M9RUaqg.png)



----

Essa é uma simples nota de rodapé[^1].

Uma nota de rodapé também pode ter várias linhas[^2].  

Você também pode usar palavras, para se adequar melhor ao seu estilo de escrita[^note].

[^1]: Minha referência.
[^2]: Cada nova linha deve ser precedida de 2 espaços.  
  Isso permite que você tenha uma nota de rodapé com várias linhas.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.  
    Essa nota de rodapé também foi feita com uma sintaxe diferente usando 4 espaços para novas linhas.


----

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

```geojson
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "id": 1,
      "properties": {
        "ID": 0
      },
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
              [-90,35],
              [-90,30],
              [-85,30],
              [-85,35],
              [-90,35]
          ]
        ]
      }
    }
  ]
}
```

```topojson
{
  "type": "Topology",
  "transform": {
    "scale": [0.0005000500050005, 0.00010001000100010001],
    "translate": [100, 0]
  },
  "objects": {
    "example": {
      "type": "GeometryCollection",
      "geometries": [
        {
          "type": "Point",
          "properties": {"prop0": "value0"},
          "coordinates": [4000, 5000]
        },
        {
          "type": "LineString",
          "properties": {"prop0": "value0", "prop1": 0},
          "arcs": [0]
        },
        {
          "type": "Polygon",
          "properties": {"prop0": "value0",
            "prop1": {"this": "that"}
          },
          "arcs": [[1]]
        }
      ]
    }
  },
  "arcs": [[[4000, 0], [1999, 9999], [2000, -9999], [2000, 9999]],[[0, 0], [0, 9999], [2000, 0], [0, -9999], [-2000, 0]]]
}
```




## Configs

{{ site.timezone }}

{{ site.teste }}

---

{{ site.author_luisangelorjr.name }}


https://docs.github.com/pt/get-started/writing-on-github/working-with-advanced-formatting/creating-diagrams