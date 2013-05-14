---
layout: post
title : Como quebrar automaticamente textos longos com css
tags : [css]
---
Esta é uma propriedade **CSS** raramente utilizada pelos desenvolvedores e extremamente útil, o <code>word-wrap</code>. Com ele você pode forçar palavras longas (sem espaços) à quebrar e ir para próxima linha sem fazer uso de nenhum **Script**, basta especificar a propriedade <code>break-word</code> na no <code>style</code> de seu elemento <code>HTML</code>.

Por exemplo, você quer garantir que um texto não se extenda para fora de uma caixa quebrando seu layout. Isso geralmente acontece muito quando você tem uma URL longa na lista dos comentários do seu blog.

A propriedade <code>word-wrap</code> é suportado por praticamente todos os browsers: **IE 5.5+**, **Firefox 3.5+**, e **WebKit** browsers como **Chrome** e **Safari**.

A seguir é dado um exemplo contendo dois <code>divs</code>, um com a propriedade padrão <code>word-wrap: normal</code>, e outro com <code>word-wrap: break-word</code> setado.

{% highlight css %}
.break-word {
  word-wrap: break-word;
}
{% endhighlight %}

<div style="word-wrap:normal; width:150px; margin:1em auto; border:1px solid #ccc;">
***Sem <code>break-word</code>***
http://www.url_longa_que_quebra_o_design
</div>

<div style="word-wrap:break-word; width:150px; margin:1em auto; border:1px solid #ccc;">
***Com <code>break-word</code>***
http://www.url_longa_que_quebra_o_design
</div>

Caso seu navegador exiba os dois textos ultrapassando as bordas dos <code>divs</code>, ele está ultrapassado e não suporta esta propriedade.