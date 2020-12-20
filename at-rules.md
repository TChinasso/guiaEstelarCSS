# AT-Rules

* esta relacionado ao comportamento do CSS
* Comeca com o sinal de '@' seguindo do identificador e valor

## Exemplos comuns

-@import       /* incluir um CSS externo */
-@media        /* regras condicionais para dispositivos */
-@font-face    /* fontes externas */
-@keyframes /* animation */

```css
@import url("http://local.com/style.css");

@media (min-width: 500px) {
    /*rules here*/
}

@font-face {
    /* rules here */
}

@keyframes nameOfAnimation {
    /* rules here */
}