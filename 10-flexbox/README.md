# 1. O que é Flexbox?

Flexbox é um modelo de layout do CSS criado para organizar elementos em linha ou coluna de forma simples, flexível e responsiva.

Ele resolve problemas comuns como:

* Centralizar elementos verticalmente
* Distribuir espaço automaticamente
* Criar layouts responsivos sem usar `float`
* Organizar elementos dinamicamente

Para ativar o Flexbox:

```css
.container {
  display: flex;
}
```

Ao fazer isso:

* O elemento pai vira um **Flex Container**
* Os elementos filhos viram automaticamente **Flex Items**

---

# 🧭 2. Conceito Fundamental: Os Eixos

Antes de entender as propriedades, você precisa entender os eixos.

## Main Axis (Eixo Principal)

É a direção definida por `flex-direction`.

### Cross Axis (Eixo Cruzado)

É o eixo perpendicular ao principal.

Exemplo:

* `flex-direction: row` → eixo principal é horizontal
* `flex-direction: column` → eixo principal é vertical

---

# 3. Propriedades do Flex Container

Todas essas propriedades são aplicadas **no elemento pai**.

---

## `display`

Ativa o Flexbox.

```css
.container {
  display: flex;
}
```

Também existe:

```css
display: inline-flex;
```

---

## `flex-direction`

Define a direção dos itens no eixo principal.

| Valor            | O que faz        |
| ---------------- | ---------------- |
| `row`            | Linha (padrão)   |
| `row-reverse`    | Linha invertida  |
| `column`         | Coluna           |
| `column-reverse` | Coluna invertida |

Exemplo:

```css
.container {
  flex-direction: column;
}
```

💡 Muito usado para layouts responsivos (mudar de linha para coluna no mobile).

---

## `flex-wrap`

Define se os itens podem quebrar linha.

| Valor          | O que faz           |
| -------------- | ------------------- |
| `nowrap`       | Não quebra (padrão) |
| `wrap`         | Permite quebra      |
| `wrap-reverse` | Quebra invertida    |

Exemplo:

```css
.container {
  flex-wrap: wrap;
}
```

💡 Essencial quando há muitos elementos.

---

## `justify-content`

Alinha os itens no **eixo principal**.

| Valor           | Resultado       |
| --------------- | --------------- |
| `flex-start`    | Início          |
| `flex-end`      | Final           |
| `center`        | Centro          |
| `space-between` | Espaço entre    |
| `space-around`  | Espaço ao redor |
| `space-evenly`  | Espaço igual    |

Exemplo:

```css
.container {
  justify-content: center;
}
```

💡 Muito usado para menus horizontais.

---

## `align-items`

Alinha os itens no **eixo cruzado**.

| Valor        | Resultado                |
| ------------ | ------------------------ |
| `stretch`    | Estica (padrão)          |
| `flex-start` | Início                   |
| `flex-end`   | Final                    |
| `center`     | Centro                   |
| `baseline`   | Pela linha base do texto |

Exemplo:

```css
.container {
  align-items: center;
}
```

💡 Usado para centralização vertical.

---

## `align-content`

Alinha **as linhas** quando há múltiplas linhas (só funciona com `wrap`).

| Valor           | Resultado           |
| --------------- | ------------------- |
| `stretch`       | Estica              |
| `flex-start`    | Início              |
| `flex-end`      | Final               |
| `center`        | Centro              |
| `space-between` | Espaço entre linhas |
| `space-around`  | Espaço ao redor     |

Exemplo:

```css
.container {
  align-content: space-between;
}
```

⚠ Só funciona se houver mais de uma linha.

---

# 🎯 4. Padrões Comuns Usando Apenas o Container

## Centralizar completamente um elemento

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

---

## Criar um menu horizontal com espaçamento

```css
.container {
  display: flex;
  justify-content: space-between;
}
```

---

## Layout responsivo (desktop → mobile)

```css
.container {
  display: flex;
  flex-direction: row;
}

@media (max-width: 600px) {
  .container {
    flex-direction: column;
  }
}
```

---

# 🧠 Resumo Mental Rápido

* `display: flex` → ativa
* `flex-direction` → direção
* `flex-wrap` → quebra linha
* `justify-content` → alinha no eixo principal
* `align-items` → alinha no eixo cruzado
* `align-content` → alinha linhas
