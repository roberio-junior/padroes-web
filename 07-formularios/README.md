# Estrutura Completa de um Formulário Web

Um formulário bem estruturado envolve:

* `<form>`
* `<label>`
* `<input>`
* `<fieldset>`
* `<legend>`
* Elementos estruturais como `<div>`, `<p>` ou listas
* Atributos importantes (`for`, `id`, `name`, `required`, etc.)

---

# O elemento `<form>`

É o **container principal** do formulário.

### Principais atributos:

| Atributo       | Função                                  |
| -------------- | --------------------------------------- |
| `action`       | URL para onde os dados serão enviados   |
| `method`       | Método HTTP (`GET` ou `POST`)           |
| `autocomplete` | Ativa/desativa preenchimento automático |

### Exemplo:

```html
<form action="/cadastro" method="post">
```

Sem `<form>`, os campos existem visualmente, mas **não enviam dados**.

---

## 🔎 Diferença entre GET e POST

| Método | Característica                        |
| ------ | ------------------------------------- |
| GET    | Envia os dados pela URL               |
| POST   | Envia os dados no corpo da requisição |

* Use **GET** para buscas.
* Use **POST** para envio de dados sensíveis ou formulários maiores.

---

# 🔹 O atributo `name`

O atributo `name` define a **chave que será enviada ao servidor**.

```html
<input type="text" name="usuario">
```

Se o usuário digitar:

```
Robério
```

O envio será algo como:

```
usuario=Robério
```

---

# O elemento `<label>` (MUITO importante)

O `<label>` associa um texto descritivo a um campo.

### Forma correta:

```html
<label for="email">E-mail:</label>
<input type="email" id="email" name="email">
```

O `for` do `<label>` deve ser igual ao `id` do `<input>`.

Se você clicar no texto “E-mail”, o campo será ativado.

---

# `<fieldset>` — Agrupamento Semântico

Ele agrupa campos relacionados.

Muito útil quando:

* Você tem grupos de rádio (`radio`)
* Grupos de checkbox
* Seções como "Dados Pessoais", "Endereço", etc.

---

# `<legend>` — Título do Grupo

O `<legend>`:

* Deve ser o **primeiro elemento dentro do `<fieldset>`**
* Descreve o conjunto de campos

Exemplo completo:

```html
<fieldset>
  <legend>Informações Pessoais</legend>

  <p>
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome">
  </p>

  <p>
    <label for="idade">Idade:</label>
    <input type="number" id="idade" name="idade">
  </p>
</fieldset>
```

---

# Estruturação Interna do Formulário

A MDN recomenda organizar os campos usando:

* `<p>` para cada campo
* `<div>` para agrupamento
* Listas `<ul>` e `<li>` quando fizer sentido

Exemplo estruturado:

```html
<form>
  <fieldset>
    <legend>Contato</legend>

    <p>
      <label for="email">E-mail:</label>
      <input type="email" id="email" name="email" required>
    </p>

    <p>
      <label for="telefone">Telefone:</label>
      <input type="tel" id="telefone" name="telefone">
    </p>
  </fieldset>
</form>
```

---

# Atributos importantes em formulários

| Atributo      | O que faz                        |
| ------------- | -------------------------------- |
| `required`    | Torna o campo obrigatório        |
| `placeholder` | Texto de exemplo dentro do campo |
| `readonly`    | Campo apenas leitura             |
| `disabled`    | Campo desativado                 |
| `pattern`     | Validação via regex              |
| `min` / `max` | Limites para números             |

---

# Exemplo Completo Profissional

```html
<form action="/enviar" method="post">
  
  <fieldset>
    <legend>Dados Pessoais</legend>

    <p>
      <label for="nome">Nome:</label>
      <input type="text" id="nome" name="nome" required>
    </p>

    <p>
      <label for="email">E-mail:</label>
      <input type="email" id="email" name="email" required>
    </p>

  </fieldset>

  <fieldset>
    <legend>Preferências</legend>

    <p>
      <input type="checkbox" id="newsletter" name="newsletter">
      <label for="newsletter">Receber newsletter</label>
    </p>

  </fieldset>

  <button type="submit">Enviar</button>
</form>
```