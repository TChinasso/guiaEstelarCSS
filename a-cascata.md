# A cascata (cascading) C do CSS

A escolha do browser de qual regra aplicar, caso haja muitas regras para o mesmo elemento

* Seu estido e lido de cima para baixo

e levado em consideracoes 3 fatores

1 origem do estilo
2 especificidade
3 importancia

### origem do estilo

Inline > tag style > tag link

HTML
<style>  TERCEIRO MAIS FORTE
  h1 {
    color:grey;
  }
</style>
<link name="stylesheet" href=""> SEGUNDO MAIS FORTE

<h1 style="color: green">TITULO</h1>   <- MAIS FORTE
<p>paragrafo</p>

CSS

h1 {            QUARTO MAIS FORTE
  color: red;
}

h1 {
  color: blue;
}

### especificidade 

e um calculo matematico, onde, cada tipo de seletor e origem do estilo, possuem valores a serem considerados

0 universal selector, combinators e nagation pseudo-class (:not())
1 element type selector e pseudo-elements (::before, ::after)
10 classes e attribute selector ([type="radio"])
100 id selector
1000 InLine

HTML
<h1 class="tittle" id="my-tittle">TITULO
<strong>STYLE</strong>
</h1>
<p>paragrafo</p>

CSS
#my-tittle, #my-tittle strong {
  color: gray;
}
.tittle {
  color: red;
}

h1 {
  color: blue;
}

* {
  color:green;
}

### a regra !important


Ultima tentativa para sobreescrever um estilo usando biblioteca externas

ex

h1 {
    color: blue !important;
}