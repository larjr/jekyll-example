---
layout: post
title:  "Sobre JWT, OAuth 2, Bearer, Cookies..."
date:   2022-08-18 12:00:00 -0300
categories: resumo sec
tags: oauth oauth2 jwt bearer cookies
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

## Por que estao relacionados?

## O que é cada coisa?

### JWT

Texto sobre JWT

### OAuth 2

#### Uma pequena confusao: Protocolo ou Framework?

Nas minhas primeiras pesquisas sobre **OAuth2** houve, a primeiro momento, uma confusao encontrada sobre o termo.
Num dos primeiros [sites que acessei](https://oauth.net/2/){:target="_blank" rel="noopener"}, existe a referencia dele como um protocolo.

> OAuth 2.0 is the industry-standard protocol for authorization...
>> **Numa traduçao livre**: "OAuth é o protocolo padrao da industria para autorizaçao..."

No meu entendimento isso poderia restringir um pouco o que ela é e como poderia ser utilizada[^1]

[^1]: Ainda farei um post sobre possiveis relações e diferenças entre termos da industria como **Protocolo**, **Framework**, **API**, **Biblioteca** e etc. Pela minha experiencia e relatos de experiencias de outros profissionais, termos/nomes por vezes perdem o sentido em outra língua muitas vezes por terem sofrido traduçao.

Maaaaaaasss...indo ao [site referencia](https://www.rfc-editor.org/rfc/rfc6749){:target="_blank" rel="noopener"} podemos ver:

> The OAuth 2.0 Authorization Framework
>> **Numa traduçao livre**: "O Framework de Autorizaçao OAuth 2.0"

E dentro desse ultimo site, ao realizar um Ctrl+F na página

|Termo | Ocorrencias|
|Protocol|26|
|Framework|7|

Com isso a inicio consigo entender um pouco o motivo da confusao rsrsrs

Mas ao ler a ref e acessar o [auth0](https://auth0.com/docs/authenticate/protocols/oauth)

>>The OAuth 2.0 authorization framework is a protocol...
 **Numa traduçao livre**: "O framework de autorizaçao OAuth 2.0 é um protocolo..."

Bom, a partir daqui iremos tratar OAuth 2 como Framework.

Blz? :wink:

#### OAuth 2 - O Framework

- Dono do Recurso (Resource Owner / RO): uma entidade capaz de conceder acesso à um recurso protegido (pode ser o usuário final).
- Servidor do Recurso (Resource Server / RE): o servidor que hospeda os recursos protegidos. O acesso a ele é feito através de tokens.
- Cliente (Client): uma aplicação requisitando recursos protegidos, através da autorização do dono.
- Servidor de Autorização (Authorization Server / AS): servidor que emite tokens de acesso ao cliente, depois de sua autenticação e obtenção de autorização. 

### Bearer

Texto sobre Bearer

### Cookies

Texto sobre Cookies

## Comparacao

### Tabela de comparacao

|   | JWT  |  OAuth |  Bearer |  Cookies  |
|---|---|---|---|---|
|  Aplicabilidade |   |   |   |   |
|  Seguranca |   |   |   |   |
|  Dificuldade |   |   |   |   |


## Fontes 

1. [Segurança - JWT x Cookies x OAuth 2.0 x Bearer](https://www.brunobrito.net.br/jwt-cookies-oauth-bearer/){:target="_blank" rel="noopener"}
2. [OAuth 2.0 - Guia do Iniciante](https://www.brunobrito.net.br/oauth2/){:target="_blank" rel="noopener"}
3. [OAuth 2.0](https://oauth.net/2/){:target="_blank" rel="noopener"}
4. [Como o JWT funciona](https://www.devmedia.com.br/como-o-jwt-funciona/40265){:target="_blank" rel="noopener"}
5. [OAUTH 2.0](https://www.gov.br/ans/pt-br/centrais-de-conteudo/manuais-do-portal-operadoras/area-do-desenvolvedor/oauth-2.0){:target="_blank" rel="noopener"}
6. <https://www.oauth.com/oauth2-servers/differences-between-oauth-1-2/>
7. <https://www.rfc-editor.org>
    1. <https://www.rfc-editor.org/rfc/rfc6749>
    2. <https://www.rfc-editor.org/rfc/rfc6750>
    2. <https://www.rfc-editor.org/rfc/rfc7519>
8. <https://jwt.io/>


## Notas de Rodapé