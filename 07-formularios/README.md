# 📌 Estrutura de um Formulário HTML

Um formulário HTML é composto por um elemento `<form>` que contém controles interativos responsáveis pela coleta e envio de dados ao servidor.

---

## `<form>`

Elemento raiz responsável por encapsular os campos e definir como os dados serão enviados.

### Atributos principais

| Atributo       | Descrição                               |
| -------------- | --------------------------------------- |
| `action`       | URL de destino dos dados                |
| `method`       | Método HTTP utilizado (`GET` ou `POST`) |
| `autocomplete` | Controla preenchimento automático       |

### Exemplo

```html
<form action="/cadastro" method="post">
```

> Campos fora do `<form>` não participam do envio.

---

### GET vs POST

| Método | Comportamento                         |
| ------ | ------------------------------------- |
| GET    | Dados enviados na URL                 |
| POST   | Dados enviados no corpo da requisição |

* **GET** → consultas e buscas
* **POST** → envio de dados sensíveis ou extensos

---

## `<label>`

Define uma descrição textual para um campo de formulário.

```html
<label for="email">E-mail</label>
<input type="email" id="email" name="email">
```

* O valor de `for` deve corresponder ao `id` do campo.
* Melhora acessibilidade e usabilidade.

---

## Agrupamento Semântico

### `<fieldset>`

Agrupa campos relacionados semanticamente.

### `<legend>`

Define o título do grupo e deve ser o primeiro elemento dentro do `<fieldset>`.

```html
<fieldset>
  <legend>Dados Pessoais</legend>
</fieldset>
```

---

## `<input>`

Elemento utilizado para criar controles interativos.

O comportamento depende do atributo `type`.

---

### Atributos essenciais

| Atributo      | Função                          |
| ------------- | ------------------------------- |
| `name`        | Chave enviada ao servidor       |
| `value`       | Valor enviado ou inicial        |
| `required`    | Campo obrigatório               |
| `checked`     | Seleção padrão (radio/checkbox) |
| `disabled`    | Desativa o campo                |
| `readonly`    | Somente leitura                 |
| `placeholder` | Texto de exemplo                |
| `pattern`     | Validação por expressão regular |

---

## Principais tipos de `<input>`

### `type="checkbox"`

Permite múltiplas seleções independentes.

* Se marcado → envia `name=value`
* Se não marcado → não envia valor

```html
<input type="checkbox" id="newsletter" name="newsletter" value="yes">
<label for="newsletter">Receber newsletter</label>
```

---

### `type="radio"`

Permite selecionar apenas uma opção dentro de um grupo.

* Radios do mesmo grupo devem compartilhar o mesmo `name`.

```html
<input type="radio" id="male" name="gender" value="male">
<label for="male">Masculino</label>

<input type="radio" id="female" name="gender" value="female">
<label for="female">Feminino</label>
```

---

## Estrutura Interna Recomendada

Para organização:

* `<p>` para cada campo
* `<div>` para agrupamentos
* Listas quando necessário

```html
<form>
  <fieldset>
    <legend>Contato</legend>

    <p>
      <label for="email">E-mail</label>
      <input type="email" id="email" name="email" required>
    </p>
  </fieldset>
</form>
```

---

# Exemplo Completo

```html
<form action="/enviar" method="post">

  <fieldset>
    <legend>Dados Pessoais</legend>

    <div class="form-group">
      <label for="nome">Nome</label><br>
      <input 
        type="text" 
        id="nome" 
        name="nome" 
        placeholder="Digite seu nome completo"
        required>
    </div>

    <div class="form-group">
      <label for="email">E-mail</label><br>
      <input 
        type="email" 
        id="email" 
        name="email" 
        placeholder="exemplo@email.com"
        required>
    </div>

    <div class="form-group">
      <label for="telefone">Telefone</label><br>
      <input 
        type="tel" 
        id="telefone" 
        name="telefone" 
        placeholder="(84) 99999-9999">
    </div>

  </fieldset>

  <fieldset>
    <legend>Gênero</legend>

    <div class="form-group">
      <input 
        type="radio" 
        id="masculino" 
        name="genero" 
        value="masculino" 
        required>
      <label for="masculino">Masculino</label>
    </div>

    <div class="form-group">
      <input 
        type="radio" 
        id="feminino" 
        name="genero" 
        value="feminino">
      <label for="feminino">Feminino</label>
    </div>

    <div class="form-group">
      <input 
        type="radio" 
        id="outro" 
        name="genero" 
        value="outro">
      <label for="outro">Outro</label>
    </div>

  </fieldset>

  <fieldset>
    <legend>Preferências</legend>

    <div class="form-group">
      <input 
        type="checkbox" 
        id="aceitar_termos" 
        name="aceitar_termos" 
        value="sim"
        required>
      <label for="aceitar_termos">Aceito os termos de uso</label>
    </div>

  </fieldset>

  <button type="submit">Enviar</button>

</form>
```
