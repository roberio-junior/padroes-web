# Lista de Exercícios de CSS

Nesta pasta você encontrará exercícios para praticar CSS.
A pasta contém um arquivo `index.html` com a estrutura básica de uma página web para teste dos exercícios e arquivos .css onde estão as resoluções dos exercícios separadas por tema. Para testar as regras CSS, basta editar o arquivo `index.html` adicionando o endereço do arquivo CSS no elemento `<link>` dentro do `<head>`.

## Sintaxe Básica

1. Crie uma regra CSS que altere a cor do texto de todos os parágrafos (`<p>`) para azul.
2. Defina uma regra CSS que mude o fundo da página para um cinza claro.
3. Crie uma regra CSS que defina a fonte de todos os títulos (`<h1>`, `<h2>`, etc.) como Arial.
4. Adicione uma regra CSS que defina uma margem de 20px para todos os parágrafos.
5. Crie uma regra CSS que defina um espaçamento interno (`padding`) de 10px para todas as `div`.

---

## Seletor de Classe

6. Crie uma classe chamada `.destaque` que altera a cor do texto para vermelho e aplique-a a um parágrafo.
7. Crie uma classe `.fundo-azul` que define o fundo de um elemento como azul e aplique-a a uma `div`.
8. Defina uma classe `.texto-grande` que aumente o tamanho da fonte para 24px e aplique-a a um parágrafo.
9. Crie uma classe `.borda-verde` que adicione uma borda de 2px sólida verde e aplique-a a uma imagem.
10. Defina uma classe `.alinhado-centro` que centralize o texto e aplique-a a um título (`<h1>`).

---

## Seletor de ID

11. Crie um ID `#cabecalho` que centralize o texto e aplique-o a um `<header>`.
12. Crie um ID `#rodape` que altere a cor de fundo para preto e o texto para branco, e aplique-o a um `<footer>`.
13. Defina um ID `#menu` que adicione um `padding` de 10px e aplique-o a um `<nav>`.
14. Crie um ID `#principal` que defina um espaçamento externo (`margin`) de 20px e aplique-o a uma `<section>`.
15. Defina um ID `#banner` que altere a altura para 200px e aplique-o a uma imagem de banner.

---

## Seletor de Atributo

16. Crie uma regra CSS que selecione todos os links (`<a>`) cujo atributo `target` seja `_blank` e altere a cor do texto para verde.
17. Defina uma regra que selecione todos os `input` cujo `type` seja `text` e defina a borda como 1px sólida preta.
18. Crie uma regra CSS que selecione todas as imagens (`<img>`) com o atributo `alt` presente e adicione uma borda de 5px sólida vermelha.
19. Crie uma regra que selecione todos os botões (`<button>`) cujo atributo `disabled` esteja presente e defina a cor de fundo para cinza.
20. Defina uma regra CSS que selecione todos os `input` cujo `type` seja `password` e altere a cor do texto para azul.

---

## Agrupamento de Seletores

21. Crie uma regra CSS que defina a margem para 20px para todos os elementos `<h1>`, `<h2>` e `<h3>`.
22. Agrupe os seletores de parágrafo (`<p>`) e `div` para terem um `padding` de 10px.
23. Crie uma regra CSS que altere a cor de fundo de todos os elementos `<header>` e `<footer>` para cinza.
24. Defina uma regra que mude a cor do texto de todos os links (`<a>`) e botões (`<button>`) para roxo.
25. Crie uma regra CSS que adicione uma borda de 1px sólida preta a todas as tabelas (`<table>`) e células de tabela (`<td>`).

---

## Combinadores

### Combinador Descendente

26. Crie uma regra CSS que defina a cor do texto dos parágrafos (`<p>`) dentro de uma `<div>` como roxa.
27. Defina uma regra que altere a cor de fundo de todos os links (`<a>`) dentro de uma `<nav>` para amarelo.
28. Crie uma regra que altere a cor do texto dos itens de lista (`<li>`) dentro de um `<ul>` para marrom.

---

### Combinador Filho

29. Crie uma regra CSS que defina a cor de fundo de todos os parágrafos (`<p>`) que são filhos diretos de uma `<div>` como verde.
30. Defina uma regra que altere a cor do texto dos itens de lista (`<li>`) que são filhos diretos de um `<ol>` para azul.
31. Crie uma regra CSS que defina o `padding` de 20px para todos os itens de menu (`<li>`) que são filhos diretos de um `<nav>`.

---

### Combinador Adjacente

32. Crie uma regra CSS que mude a cor de fundo de um parágrafo (`<p>`) que venha imediatamente após um `<h1>` para cinza.
33. Defina uma regra que altere a cor do texto de um `<h2>` que venha imediatamente após uma `<div>` para vermelho.
34. Crie uma regra CSS que adicione uma margem de 10px a qualquer `<li>` que venha imediatamente após outro `<li>`.

---

### Combinador Generalizado

35. Crie uma regra CSS que altere a cor de fundo de todos os parágrafos (`<p>`) que vêm após um `<h2>` para azul.
36. Defina uma regra que mude a cor do texto de todos os links (`<a>`) que vêm após um `<p>` para verde.
37. Crie uma regra CSS que adicione um `padding` de 15px a todos os itens de lista (`<li>`) que vêm após um `<ul>`.

---

## Utilização do `!important`

38. Crie uma regra CSS que defina a cor do texto de todos os parágrafos (`<p>`) como preto com a prioridade `!important`.
39. Defina uma regra que altere o tamanho da fonte de todos os títulos (`<h1>`, `<h2>`, etc.) para 30px com a prioridade `!important`.