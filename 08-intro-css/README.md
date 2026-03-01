# Introdução ao CSS

CSS (Cascading Style Sheets) é a linguagem usada para definir a aparência e o layout de páginas web. Enquanto o HTML estrutura o conteúdo (como títulos, parágrafos, imagens e formulários), o CSS é responsável por controlar cores, fontes, espaçamentos, tamanhos, posicionamento e até animações dos elementos na tela.

Ele funciona aplicando **regras de estilo** a elementos selecionados do HTML, permitindo separar o conteúdo da apresentação. Isso torna o código mais organizado, reutilizável e fácil de manter.

Além disso, o CSS possibilita a criação de **layouts responsivos**, adaptando o design para diferentes dispositivos, como celulares, tablets e computadores.

---

# Seletores CSS

Seletores são **padrões que determinam a quais elementos HTML um conjunto de regras CSS deve ser aplicado**. Ou seja, eles “selecionam” os elementos que você quer estilizar.

---

## Seletores Básicos

* **Seletor por tag:** seleciona pelo nome da tag HTML
  Exemplo: `div`, `p`, `h1`

* **Seletor por classe:** seleciona elementos com determinada classe (começa com `.`)
  Exemplo: `.container`

* **Seletor por ID:** seleciona um elemento específico (começa com `#`)
  Exemplo: `#menu`

* **Seletor universal:** seleciona *todos* os elementos
  Exemplo: `*`

* **Seletores por atributo:** selecionam com base em atributos
  Exemplos:
  `[required]`
  `[type="text"]`

---

## Combinadores

Permitem selecionar elementos com base na **relação entre eles**, como:

* Elementos dentro de outros
* Filhos diretos
* Irmãos imediatos
* Irmãos em geral

Eles ajudam a criar seleções mais específicas dentro da estrutura do HTML.

---

## Pseudo-classes

Selecionam elementos com base em **estado ou interação**:

* `:hover` → quando o mouse está sobre o elemento
* `:visited` → link já visitado
* `:focus` → elemento em foco

---

## Pseudo-elementos

Representam **partes específicas de um elemento**:

* `::first-line` → primeira linha
* `::before` → conteúdo antes do elemento
* `::after` → conteúdo depois do elemento

---

# O que são Classes em HTML e CSS

## Classes no HTML

No HTML, o atributo `class` é usado para **marcar elementos com um ou mais nomes de classe**, separados por espaço.

Isso permite identificar e categorizar elementos para estilização com CSS ou manipulação com JavaScript.

Exemplo:

```html
<div class="menu principal"></div>
```

Um mesmo elemento pode ter **várias classes ao mesmo tempo**.

---

## Classe como seletor no CSS

Em CSS, a classe funciona como um **seletor** que aponta para todos os elementos que tenham aquele nome de classe.

A sintaxe é simples:

```css
.nomeDaClasse {
  propriedade: valor;
}
```

Exemplo:

```css
.menu {
  color: blue;
}

.principal {
  font-weight: bold;
}
```

Nesse caso, o `<div class="menu principal">` receberá **os dois estilos**, porque possui as duas classes.

---

## Múltiplas classes no mesmo elemento

Você também pode criar seletores mais específicos combinando classes:

```css
li.espaçoso.elegante {
  margin: 20px;
}
```

Esse estilo será aplicado apenas a elementos `li` que possuam **as duas classes ao mesmo tempo**.

Outro exemplo prático:

```html
<p class="vermelho amarelo-bg"></p>
```

```css
.vermelho {
  color: red;
}

.amarelo-bg {
  background: yellow;
}
```

O parágrafo terá texto vermelho e fundo amarelo.

---

# Agrupando Seletores em CSS

## Por que agrupar?

Quando **vários seletores compartilham o mesmo conjunto de regras**, você pode agrupá-los para deixar o CSS mais limpo, curto e fácil de manter.

---

## Como funciona

Você separa os seletores com **vírgulas**:

```css
h1, h2, p, .box {
  color: green;
  font-size: 16px;
}
```

Todos os `h1`, `h2`, `p` e qualquer elemento com a classe `box` receberão os mesmos estilos.
