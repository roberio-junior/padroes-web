# 1. O que são Media Queries?

Media Queries são recursos do CSS que permitem aplicar estilos diferentes dependendo das características do dispositivo ou da tela.

Elas são fundamentais para o **design responsivo**, ou seja, para criar sites que se adaptam a:

* Celulares
* Tablets
* Notebooks
* Monitores maiores

---

# 2. Para que servem?

Permitem alterar:

* Layout
* Tamanho de fonte
* Direção do Flexbox
* Espaçamentos
* Cores
* Exibição ou ocultação de elementos

Tudo com base em características como largura, altura ou orientação da tela.

---

# 3. Sintaxe Básica

```css
@media (condição) {
  /* regras CSS */
}
```

---

# 4. Condições Mais Utilizadas

## max-width

Aplica estilos até determinado tamanho de tela.

```css
@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }
}
```

Muito usado para adaptar layouts ao celular.

---

## min-width

Aplica estilos a partir de determinado tamanho.

```css
@media (min-width: 1024px) {
  .menu {
    display: flex;
  }
}
```

Muito usado para adaptar ao desktop.

---

# 5. Breakpoints Comuns

Não são obrigatórios, mas são referências bastante utilizadas:

* Celular: até 600px
* Tablet: 601px até 1024px
* Desktop: acima de 1024px

Exemplo prático:

```css
/* Estilo padrão */
body {
  font-size: 16px;
}

/* Tablet */
@media (min-width: 768px) {
  body {
    font-size: 18px;
  }
}

/* Desktop */
@media (min-width: 1024px) {
  body {
    font-size: 20px;
  }
}
```

---

## 6. Outras Condições Possíveis

Além de largura, é possível usar:

* `max-height`
* `min-height`
* `orientation: portrait` (vertical)
* `orientation: landscape` (horizontal)
* `print` (estilos para impressão)
