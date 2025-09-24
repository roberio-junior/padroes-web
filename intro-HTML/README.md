### 🔹 O que é HTML

* HTML (HyperText Markup Language) não é uma linguagem de programação, mas uma **linguagem de marcação** usada para estruturar páginas da web.
* Ele define elementos que contêm ou envolvem partes do conteúdo para indicar como devem ser exibidas ou comportar-se.

---

### 🔹 Anatomia de um elemento HTML

Um elemento HTML geralmente é formado por:

1. **Tag de abertura**

   * Marca o início do elemento.
   * Contém o **nome da tag** (ex.: `p`, `h1`, `div`, `a`, etc.).
   * Pode conter **atributos** que fornecem informações extras.
   * Exemplos:

     ```html
     <p>
     <a href="https://example.com">
     ```

2. **Tag de fechamento**

   * Marca o fim do elemento.
   * Sempre começa com `/` seguido do nome da tag.
   * Exemplos:

     ```html
     </p>
     </a>
     ```

3. **Conteúdo**

   * O que está entre a **tag de abertura** e a **tag de fechamento**.
   * Pode ser texto, outros elementos HTML ou ambos.
   * Exemplo:

     ```html
     Este é um parágrafo.
     ```

4. **Elemento** 
    * É o conjunto: abertura + conteúdo + fechamento.

---

### 🔹 Exemplo completo

```html
<a href="https://example.com" target="_blank">Exemplo Completo</a>
```

* **Tag de abertura**: `<a href="https://example.com" target="_blank">`
* **Atributos**:

  * `href="https://example.com"` → define o link.
  * `target="_blank"` → abre em nova aba.
* **Conteúdo**: `Exemplo Completo`
* **Tag de fechamento**: `</a>`

---

### 🔹 Elementos aninhados

Elementos podem ser **aninhados**, ou seja, um elemento dentro de outro, mas os elementos devem abrir e fechar corretamente para que eles fiquem claramente dentro ou fora do outro.

Exemplo **correto**:

```html
<p>Um parágrafo com <strong>texto em negrito</strong>.</p>
```

Exemplo **errado** (a ordem de fechamento não foi respeitada):

```html
<p>Um parágrafo com <strong>texto em negrito.</p></strong>
```

---

### 🔹 Elementos Vazios (self-closing)

Alguns elementos **não têm conteúdo** e não precisam de tag de fechamento.
Exemplo:

```html
<img src="foto.jpg" alt="Descrição da imagem">
<br>
<hr>
```
---

### 🔹 Categorias de Elementos HTML

* Existem duas categorias no HTML: **block** (bloco) e **inline**.

* **Block (bloco)**

  * Ocupam toda a largura disponível e começam em uma nova linha.
  * Exemplo: `<div>`, `<p>`, `<h1>`, `<section>`.

* **Inline (em linha)**

  * Não quebram a linha, ficam “dentro” do fluxo do texto.
  * Exemplo: `<a>`, `<span>`, `<em>`, `<strong>`.

Exemplo prático:

```html
<p>Isso é um <em>texto em itálico</em> dentro de um parágrafo em uma linha.</p>
```

```html
<p>Esse é um parágrafo em outro bloco.<p>
```

---

### 🔹 Atributos

* Elementos podem ter **atributos** que fornecem informações adicionais, como `class`, `id`, `href`, `title` etc. ([MDN Web Docs][1])
* Atributos têm nome, sinal de igual, valor entre aspas. ([MDN Web Docs][1])
* **Atributos booleanos**: alguns atributos funcionam como “liga/desliga” — ex: `disabled`. Quando presentes, já ativam o efeito desejado. ([MDN Web Docs][1])
* Aspas simples ou duplas para os valores são permitidas; o importante é não misturar de modo errado. ([MDN Web Docs][1])
* Sempre usar aspas ajuda a evitar ambiguidades. ([MDN Web Docs][1])

---

## Estrutura básica de um documento HTML

Uma página HTML típica inclui:

* `<!DOCTYPE html>` — declaração que indica o tipo do documento. ([MDN Web Docs][1])
* `<html>` — elemento raiz que envolve todo o conteúdo HTML. ([MDN Web Docs][1])
* `<head>` — contém metadados (“metainformações”) que não aparecem diretamente na página, como título, codificação de caracteres etc. ([MDN Web Docs][1])
* `<meta charset="utf-8">` — define qual codificação de caracteres o documento usa; UTF-8 cobre a maioria dos caracteres de línguas humanas. ([MDN Web Docs][1])
* `<title>` — define o título que aparece na aba do navegador. ([MDN Web Docs][1])
* `<body>` — contém todo conteúdo visível ao usuário (texto, imagens, vídeos, links etc.). ([MDN Web Docs][1])

---

## Outros conceitos importantes

* **Referências de entidades HTML**: quando você quer colocar caracteres especiais como `<`, `>`, `&`, aspas dentro de texto, você usa entidades como `&lt;`, `&gt;`, `&amp;` etc. Para evitar que esses caracteres sejam interpretados como parte da marcação. ([MDN Web Docs][1])
* **Comentários**: são seções de código invisíveis para o usuário/navegador, usadas para documentação, explicações etc. Sintaxe: `<!-- comentário -->`. ([MDN Web Docs][1])
* **Espaços em branco e quebras de linha no HTML**: excesso de espaços, múltiplas quebras de linha não mudam muito a renderização — o navegador “colapsa” espaços extras em um só. Servem mais para legibilidade do código. ([MDN Web Docs][1])
