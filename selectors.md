# Selector

conecta um elemento HTML com o css

## Tipos

* Global selector '*'
* Element/Type selector 'h1, h2, p, div'
* ID Selector '#box, #container'
* Class selector '.red, .m-4'
* Atribute selector, Pseudo-class, Pseudo-element e outros


HTML


<div id="container" class="m-4">
  <h1>Titulo da pagina</h1>
  <h2>Subtitulo</h2>
</div


CSS

* {
  margin: 0;
}

#container {
  width: 30%
}

.m-4 {
  margin: 40px;
}

h1, h2 {
  color: red;
  font-size: 60px;
  background: gray;
  text-align:center;
}