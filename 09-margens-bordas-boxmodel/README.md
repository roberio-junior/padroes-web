# Box Model (Modelo de Caixa)

No CSS, **todo elemento HTML é representado como uma caixa**.
Essa caixa é composta por:

```
+-----------------------------+
|           margin            |
|   +---------------------+   |
|   |       border        |   |
|   |   +-------------+   |   |
|   |   |   padding   |   |   |
|   |   | +---------+ |   |   |
|   |   | | content | |   |   |
|   |   | +---------+ |   |   |
|   |   +-------------+   |   |
|   +---------------------+   |
+-----------------------------+
```

Ordem de dentro para fora:

**Conteúdo → Padding → Border → Margin**

---

# 1. Padding (Preenchimento)

O **padding** é o espaço interno entre o conteúdo e a borda.

 Ele “empurra” a borda para longe do conteúdo.

## Exemplo:

```css
div {
  padding: 20px;
}
```

Isso adiciona 20px de espaço interno em todos os lados.

## Lados específicos:

```css
padding-top
padding-right
padding-bottom
padding-left
```

Ou forma resumida:

```css
padding: 10px 20px 15px 5px;
/* topo | direita | baixo | esquerda */
```

---

# 2. Border (Borda)

A **border** é a linha que fica ao redor do padding e do conteúdo.

Ela precisa de **3 propriedades principais**:

```css
border-width
border-style
border-color
```

## Exemplo completo:

```css
div {
  border: 2px solid black;
}
```

`2px` → espessura
`solid` → estilo
`black` → cor

## Tipos de borda:

* solid
* dashed
* dotted
* double
* groove
* ridge

Também pode definir lados específicos:

```css
border-top: 1px solid red;
```

---

# 3. Margin (Margem)

A **margin** é o espaço externo da caixa.

Ela afasta o elemento dos outros elementos.

## Exemplo:

```css
div {
  margin: 30px;
}
```

Isso adiciona 30px de espaço externo em todos os lados.

## Forma resumida:

```css
margin: 10px 20px 15px 5px;
/* topo | direita | baixo | esquerda */
```

## Centralizar com margin:

```css
div {
  margin: 0 auto;
}
```

Isso centraliza horizontalmente (quando há largura definida).

---

# Diferença Principal

| Propriedade | Fica onde?             | Afeta o quê?   |
| ----------- | ---------------------- | -------------- |
| padding     | Dentro da borda        | Espaço interno |
| border      | Entre padding e margin | Linha ao redor |
| margin      | Fora da borda          | Espaço externo |

---

# ⚠️ Importante: Impacto no Tamanho

Por padrão, o tamanho total da caixa é:

```
largura total = width + padding + border
```

Se quiser que padding e border não aumentem o tamanho:

```css
box-sizing: border-box;
```

Essa propriedade é muito usada em projetos modernos.
