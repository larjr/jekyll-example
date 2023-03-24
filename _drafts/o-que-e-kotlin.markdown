---
layout: post
title:  "OQueÉ: Kotlin"
date:   2022-09-01 00:00:00 -0300
categories: OQueÉ Kotlin
tags: [OQueÉ, Kotlin]
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

> N'ao. Kotlin nao 'e o sobrenome de um Sir Charles Kotlin, blessed by god e londrino por natureza.
>> (mas que beleza) - **Jorge Ben Jor**

Ola, eu sou o {{site.author_luisangelorjr.name}}, mas geralmente vcs irao me achar na internet como {{site.author_luisangelorjr.nickname}} :sunglasses:

![Logo Oficial da Linguagem Kotlin]({{site.baseurl}}/assets/img/kotlin/Kotlin%20Full%20Color%20Logo%20on%20White%20RGB.svg)

## "Kotlin"?

>Ok, vamos esquecer o Sir Charles Kotlin...por enquanto...

[Kotlin](https://kotlinlang.org/){:target="_blank" rel="noopener"} 'e uma linguagem de programacao lan'cada oficialmente (primeira vers'ao est'avel, [Kotlin 1.0.0](https://github.com/JetBrains/kotlin/releases/tag/build-1.0.0)) em [2016-02-15](https://blog.jetbrains.com/kotlin/2016/02/kotlin-1-0-released-pragmatic-language-for-jvm-and-android/){:target="_blank" rel="noopener"}, mas tendo seu primeiro an'uncio p'ublico em [2011-07-19](https://blog.jetbrains.com/kotlin/2011/07/hello-world-2/){:target="_blank" rel="noopener"}. Tendo como parte core do time desenvolvedor da linguagen nomes como [Andrey Beslav](https://twitter.com/abreslav){:target="_blank" rel="noopener"} ([como Language Designer e Project Lead](https://github.com/abreslav){:target="_blank" rel="noopener"}), [Roman Belov](https://twitter.com/volebamor){:target="_blank" rel="noopener"}, [Dmitry Jemerov](https://twitter.com/intelliyole){:target="_blank" rel="noopener"}, entre outros

Com seu desenvolvimento encabecado pela [Jetbrains](https://www.jetbrains.com/pt-br/opensource/kotlin/){:target="_blank" rel="noopener"} desde o inc'icio at'e a atual data desse post, na atual vers'ao [Kotlin 1.7.10](https://blog.jetbrains.com/kotlin/2022/06/kotlin-1-7-0-released/){:target="_blank" rel="noopener"} lanc'ada em [2022-07-08](https://github.com/JetBrains/kotlin/releases/tag/v1.7.10){:target="_blank" rel="noopener"} e j'a com boa parte do time de desenvolvedores alterado/ampliado.

E em [2019-05-07](https://techcrunch.com/2019/05/07/kotlin-is-now-googles-preferred-language-for-android-app-development/){:target="_blank" rel="noopener"} 'e anunciada como a linguagem de preferencia para programar nativamente em Android (mesmo que ainda mantenha seu suporte e interoperabilidade com Java)

Apesar disso, Kotlin tamb'em [pode ser usada no backend](https://kotlinlang.org/lp/server-side/){:target="_blank" rel="noopener"}, [frontend](https://kotlinlang.org/docs/js-overview.html){:target="_blank" rel="noopener"}, [multi-plataforma mobile](https://kotlinlang.org/lp/mobile/){:target="_blank" rel="noopener"} (isso quer dizer que al'em do Android, tamb'em rodar'a no iOS), para [ciencia de dados](https://kotlinlang.org/docs/data-science-overview.html){:target="_blank" rel="noopener"}, [programacao competitiva](https://kotlinlang.org/docs/competitive-programming.html){:target="_blank" rel="noopener"} e [NATIVAMENTE!!!](https://kotlinlang.org/docs/native-overview.html){:target="_blank" rel="noopener"} (ou seja, sem precisar da JVM ou correlatas).


> Mas aqui nesse post nao iremos a fundo nesses ou em outros recursos avan'cados da linguagem.
> Deixarei para explorar em posts dedicados.

## Sintaxe b'asica

Bom, toda linguagem de programacao tem sua sintaxe b'asica por onde todo mundo 
come'ca e n'os nao seremos diferentes.

Ah...tbm é importante eu dizer que iremos utilizar a ultima versao estável do 
Kotlin, [v1.17.10](https://github.com/JetBrains/kotlin/releases/tag/v1.7.10) 
para esses exemplos

### Coment'arios

Antes de come'carmos mas j'a come'cando, quero falar sobre como fazer 
coment'arios dentro do Kotlin.

Coment'arios s'ao ignorados pela linguagem e o computador mas podem ser 
importantes para o ser humano que o est'a lendo pois deixa **coment'arios** proximo a trechos importantes e tamb'em pode ser usado para desativar trechos de c'odigo. O conceito de coment'arios 
tamb'em se estende a outras linguagens de forma bem parecida.

Esse recurso ser'a muito importante em todo o post pois quando eu precisar dar 
enfase para alguma parte que seja c'odigo, o usarei

OK! Entao, vamos l'a!
Temos duas formas b'asicas que iremos abordar (tamb'em temos uma terceira forma. Um recurso 
interessante chamado de KDoc que veremos s'o em outro post)

A primeira 'e um coment'ario de linha 'unica:

{% highlight kotlin %}
// Sim...eu sou o coment'ario de linha 'unica.
// Eu sou outro : )
// E eu tbm :D
{% endhighlight %}

Para utilizar ele digitamos // e tudo que estiver a direita e na mesma linha se tornar'a parte do coment'arios'o. Simples. :slightly_smiling_face:

A segunda 'e um coment'ario em bloco:

{% highlight kotlin %}
/*
    Oiiiiii!!! Sim!
    Sou o coment'ario de m'ultiplas linhas.

    Como pode ver, comigo voce consegue escrever bastante
    sem precisar digitar "//" toda linha
*/
{% endhighlight %}

Para utilizar ele comecamos com /* e fechamos com */. Tudo que estiver entre eles, ser'a tratado como coment'ario.

Simples tamb'em :smile:

>"Poh! Ai sim! Gostei desse recurso" - [Walter Casagrande](https://pt.wikipedia.org/wiki/Walter_Casagrande).

>"Eeeeeeuuu taaaaaaambeeem, Tixinha!!!" - [Gustavo Melão](https://twitter.com/melaogustavo).

>"Nao gosto de fofoca, s'o to comentando s'o" - Minha v'o fofocando sobre a
vida das inimiga.

### Funçao main

É aqui que sua aplicaçao dará início.
Ela é declarada dessa forma:

{% highlight kotlin %}
fun main() {
  // É nesse espaço que seu código **Kotlin** 'e implementado
}
{% endhighlight %}

Tamb'em existe essa forma de utilizar a funcao main: passando argumentos na sua inicializacao

{% highlight kotlin %}
fun main(args: Array<String>) {
    /*
        É nesse espaço que seu código **Kotlin** 'e implementado
        e vc poder'a utilizar o conteudo passado como argumento 
        na variavel args para montar sua l'ogica
    */
}
{% endhighlight %}

>Na minha experiencia, passagem de argumentos dessa maneira nao 'e tao usada no dia-a-dia.
>Vi seu uso sendo usado em ferramentas de linha de comando ou em algumas de back especificas

### Printar na tela (imprimir na sa'ida padrao)

>Geralmente as linguagens de programacao sao interfaces de comunicacao entre humanos e maquinas

Tendo isso em mente, no topico anterior vimos uma forma de "falar" com a m'aquina.
Agora iremos utilizar a funcao println() para que nossa aplicacao tenha uma "voz":

{% highlight kotlin %}
fun main() {
    println("Ola Mundo!")
    println(42)
}
{% endhighlight %}

<iframe src="https://pl.kotl.in/iVdIEyBQL?theme=darcula&from=2&to=2"></iframe>

>Tudo o que 'e passado dentro de println() ser'a printado na saida padrao, que no nosso caso 'e o console

### Vari'aveis

Quase 100% das vezes que inicio uma explicacao sobre alguma linguagem de programacao, eu inicio 
demonstrando a atribuicao de alguma variavel. Nesse post por alguns motivos did'aticos decidi seguir por outro caminho.

Para mim faz sentido come'car por vari'aveis pois parto de uma tentativa de mostrar um local, um ponto 
onde podemos sempre olhar (*assim como um cesto que podemos armazenar laranjas
 OU uma seta/ponteiro que podemos usar de referencia*) e ver algo que 
 processamos.

>'E uma tentativa de dar algo mais concreto nesse imenso mundo de abstra'c'oes.

Primeiro vamos ver sobre a declaracao e atribuicao pra tr'es tipos

{% highlight kotlin %}
                // #1
val a: Int = 7  // Atribui'c'ao imediata com a tipagem "Int". Prefira utilizar esse sempre que poss'ivel.

                // #2
val b = 7       // O tipo "Int" foi inferido. A linguagem entende que pela atribui'c'ao ela 'e do tipo "Int"

                // #3
val c: Int      // O tipo "Int" foi declarado mas nenhum valor foi atribuido 'a vari'avel, ou seja, ela nao foi inicializda.
c = 7           // Agora o valor foi atribuido :)
{% endhighlight %}

Como voc'es perceberam, a palavra val 'e uma forma que temos de criar uma variavel.
Criando a variavel com val, a ela ser'a somente leitura.

Mas...ser'a

#### val Versus var

Acabamos de aprender sobre a palavra reservada val para declarar vari'aveis. 
Mas tamb'em temos outra palavra reservada para isso: var

Basicamente, o var consegue ter o valor atribu'ido a ele alterado (recurso muito utilizado dentro de lacos de repeticao).
O mesmo nao ocorre com val, que 'e mais indicado para quando se precisar manter os valores

{% highlight kotlin %}
var x: Int = 5 // Aqui declaramos nossa variavel com var
x += 1 // Aqui conseguimos alterar o valor atribu'ido a varia'avel

// Agora vamos tentar algo parecido com val

val y: Int = 5 // Aqui declaramos nossa variavel com val
y += 1  /* 'Val cannot be reassigned' esse ser'a o erro que tomaremos 
            se tentarmos alterar o valor de uma vari'avel com val */
{% endhighlight %}

Logo abaixo, um exemplo de uso interessante de ambas vari'aveis, onde PI 'e uma constante que n'ao ser'a alterada e x 'e uma variavel que ser'a alterada logo ao chamar incrementarX()

{% highlight kotlin %}
val PI = 3.14
var x = 0

fun incrementarX() { 
    x += 1 
}

fun main() {
    println("x = $x; PI = $PI")
    incrementarX()
    println("incrementarX()")
    println("x = $x; PI = $PI")
}
{% endhighlight %}

>No geral, por seguran'ca e organizacao, indico preferir utilizar o val em detrimento ao var 

#### Data Types (Tipos das vari'aveis)

Quero me aprofundar melhor nos tipos de dados em uma s'erie de Kotlin (e nao essa de OQue'E), mas aqui, para conseguirmos ter alguns elementos minimos, vamos usar cinco tipos de variaveis:

- Boolean
- Char
- String
- Int
- Double

##### Boolean

{% highlight kotlin %}
val meuBooleano: Boolean = true // Boolean
{% endhighlight %}

##### Char

{% highlight kotlin %}
val minhaLetra: Char = 'D' // Char
{% endhighlight %}

##### String

{% highlight kotlin %}
val meuTexto: String = "Hello" // String
{% endhighlight %}

##### Int

{% highlight kotlin %}
val meuNumero: Int = 5 // Int
{% endhighlight %}

##### Double

{% highlight kotlin %}
val meuNumeroDecimal: Double = 5.99 // Double
{% endhighlight %}

### Funcoes

{% highlight kotlin %}
{% endhighlight %}

{% highlight kotlin %}
fun somar(a: Int, b: Int): Int {
    return a + b
}

fun main() {
    print("Soma de 3 e 5 'e: ")
    println(somar(3, 5))
}
{% endhighlight %}

### Condicionais

#### if

{% highlight kotlin %}
fun maiorDe(a: Int, b: Int): Int {
    if (a > b) {
        return a
    } else {
        return b
    }
}

fun main() {
    println("Maior n'umero entre 0 e 42 'e ${maiorDe(0, 42)}")
}
{% endhighlight %}

{% highlight kotlin %}
fun maiorDe(a: Int, b: Int) = if (a > b) a else b

fun main() {
    println("Maior n'umero entre 0 e 42 'e ${maiorDe(0, 42)}")
}
{% endhighlight %}

#### when

{% highlight kotlin %}
fun descrever(obj: Any): String =
    when (obj) {
        1           -> "Um"
        "Oi"        -> "Sauda'c''ao"
        is Long     -> "N'umero do tipo Long"
        !is String  -> "N'ao 'e uma String"
        else        -> "Desconhecido"
    }

fun main() {
    println(descrever(1))
    println(descrever("Oi"))
    println(descrever(1000L))
    println(descrever(2))
    println(descrever("other"))
}
{% endhighlight %}

### La'cos

#### for 

{% highlight kotlin %}
fun main() {
    val items = listOf("ma'ca", "banana", "kiwi")
    for (item in items) {
        println(item)
    }
}
{% endhighlight %}

{% highlight kotlin %}
fun main() {
    val items = listOf("ma'ca", "banana", "kiwi")
    for (index in items.indices) {
        println("item na posicao $index 'e ${items[index]}")
    }
}
{% endhighlight %}

#### while

{% highlight kotlin %}
fun main() {
    val items = listOf("ma'ca", "banana", "kiwi")
    var index = 0
    while (index < items.size) {
        println("item na posicao $index 'e ${items[index]}")
        index++
    }
}
{% endhighlight %}

### Interpola'c'ao (String Templates)

{% highlight kotlin %}
fun main() {
    var a = 1
    // simple name in template:
    val s1 = "a is $a" 

    a = 2
    // arbitrary expression in template:
    val s2 = "${s1.replace("is", "was")}, but now is $a"
    println(s2)
}
{% endhighlight %}

### Classes e suas instancias

{% highlight kotlin %}
class FormaGeometrica
{% endhighlight %}

{% highlight kotlin %}
class Retangulo(var altura: Double, var comprimento: Double) {
    var perimetro = (altura + comprimento) * 2
}
{% endhighlight %}

{% highlight kotlin %}
class Retangulo(var altura: Double, var comprimento: Double) {
    var perimetro = (altura + comprimento) * 2 
}
fun main() {
    val Retangulo = Retangulo(5.0, 2.0)
    println("O perimetro 'e ${Retangulo.perimetro}")
}
{% endhighlight %}

{% highlight kotlin %}
open class FormaGeometrica

class Retangulo(var altura: Double, var comprimento: Double): FormaGeometrica() {
    var perimetro = (altura + comprimento) * 2
}
{% endhighlight %}
{% highlight kotlin %}
{% endhighlight %}
{% highlight kotlin %}
{% endhighlight %}

## Fontes 

1. [Kotlin](https://kotlinlang.org/){:target="_blank" rel="noopener"}
2. <https://blog.jetbrains.com/kotlin/category/releases/>
3. <https://kotlinlang.org/docs/kotlin-brand-assets.html>
4. <https://www.baeldung.com/kotlin/const-var-and-val-keywords>
