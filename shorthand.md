﻿## Shorthand

* juncao de propriedades
* resumido
* legivel

```css

{
    /* background properties */
    background-color: #000;
    background-image: url(images/bg.gif);
    background-repeat: no repeat;
    background-position: left top;

    /* background shorthand */
    background: #000 url(images/bg.gif) no repeat left top;
}
```
## detalhes

* nao ira considerar propriedades anteriores
* valores nao especificados irao assumir o valor padra
* geralmente, a ordem descrita nao importa, mas, se houver muitas propriedades com valores  semelhantes, podemos encontrar problemas