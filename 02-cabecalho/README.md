### 🔹 O que são metadados / cabeçalho HTML

* O elemento `<head>` de um documento HTML contém informações **não exibidas diretamente** na página, mas que descrevem ou controlam aspectos da página (metadados). 
* Exemplos do que pode estar no `<head>`: título da página, links para CSS, favicons, metadados como autor e descrição. 

---

### 🔹 Elemento `<title>`

* `<title>` define o **título do documento**, que aparece na aba do navegador, bookmarks e resultados de busca. 
* É diferente de `<h1>`, que aparece no conteúdo da página. 

---

### 🔹 Elemento `<meta>`

* Usado para fornecer informações adicionais sobre o documento, por exemplo:

  * `<meta charset="utf-8">`: define a codificação de caracteres (UTF-8 é recomendada para suportar múltiplos idiomas). 
  * `<meta name="author" content="…">`: indica o autor da página. 
  * `<meta name="description" content="…">`: uma breve descrição da página que costuma aparecer nos resultados de busca (SEO). 
  * Algumas tags `<meta>` antigas como `keywords` já são ignoradas por mecanismos de busca modernos. 

* Também podem ser usados metadados específicos para redes sociais, como **Open Graph** (para Facebook) ou metadados do Twitter, para controlar como o link aparece quando compartilhado. 

---

### 🔹 Ícones personalizados / favicon

* O favicon é o ícone que aparece na aba do navegador ou na lista de favoritos. Ele é referenciado no `<head>` por `<link rel="shortcut icon" …>`. 
* Também podem ser incluídos ícones específicos para dispositivos (como ícones para iPhone / iPad) usando diferentes tamanhos e atributos. 

---

### 🔹 Inclusão de CSS e JavaScript

* CSS externo é normalmente referenciado no `<head>` via `<link rel="stylesheet" href="…">`. 
* Scripts JavaScript (via `<script src="…">`) **podem** ficar no `<head>`, mas muitas vezes é preferível colocá-los ao final do `<body>` para garantir que o HTML já esteja carregado antes da execução. 

---

### 🔹 Definição do idioma da página

* É recomendado usar o atributo `lang` no elemento `<html>` para indicar o idioma principal da página, por exemplo `<html lang="pt-BR">`. 
* Isso ajuda mecanismos de busca e também tecnologias assistivas (como leitores de tela) a interpretarem o conteúdo corretamente. 
* Partes dentro da página em idiomas diferentes podem usar `lang` aplicados localmente (por exemplo, em `<span lang="jp">`). 

