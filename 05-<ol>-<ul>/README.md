## 📋 O que são `<ul>` e `<ol>`

Ambos `<ul>` e `<ol>` são elementos de lista em HTML, usados para agrupar itens listados. Eles diferem basicamente no fato de que:

* `<ul>` (lista **não ordenada**) exibe itens com marcadores (bolinhas, quadrados etc.), sem ênfase em ordem.
* `<ol>` (lista **ordenada**) exibe itens numerados ou com outro tipo de contagem, enfatizando uma sequência/ordem entre os itens.

Ou seja: se a ordem dos itens importa (ex: etapas de um processo), use `<ol>`; se não importa (ex: lista de ingredientes, tópicos), use `<ul>`.

---

## Estrutura básica

Ambos os elementos compartilham uma estrutura muito similar:

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

<ol>
  <li>Primeiro passo</li>
  <li>Segundo passo</li>
  <li>Terceiro passo</li>
</ol>
```

* Em ambos os casos, os elementos internos devem ser `<li>` (item de lista).
* As tags de abertura e fechamento (`<ul> … </ul>`, `<ol> … </ol>`) são obrigatórias.
* As listas podem ser **aninhadas** (listas dentro de listas), combinando `<ul>` dentro de `<ol>` ou vice-versa, sem limite de profundidade.

Exemplo de aninhamento misto:

```html
<ul>
  <li>Frutas
    <ol>
      <li>Maçã</li>
      <li>Banana</li>
    </ol>
  </li>
  <li>Legumes</li>
</ul>
```
