
## 📌 O que é `<table>`

O elemento `<table>` em HTML é usado para **organizar dados em forma de tabela**, em linhas e colunas — ideal para apresentar conteúdo tabular de forma estruturada.

Exemplos de uso:

* Planilhas de informações
* Listas de valores comparativos
* Grades de dados com cabeçalhos e rodapés

---

## 🧱 Estrutura Básica

Uma tabela em HTML pode ter:

```html
<table>
  <caption>Título da Tabela</caption> <!-- opcional -->
  <thead>…</thead>   <!-- cabeçalho das colunas -->
  <tbody>…</tbody>   <!-- corpo principal -->
  <tfoot>…</tfoot>   <!-- rodapé -->
</table>
```

Elementos internos:

| Tag         | Uso                         |
| ----------- | --------------------------- |
| `<caption>` | Descrição/título da tabela  |
| `<thead>`   | Agrupa cabeçalhos de coluna |
| `<tbody>`   | Agrupa linhas de dados      |
| `<tfoot>`   | Agrupa rodapé de tabela     |
| `<tr>`      | Linha                       |
| `<th>`      | Cabeçalho da célula         |
| `<td>`      | Célula de dados             |

---

## 📊 Exemplo Simples

```html
<table>
  <caption>Estudantes e Idades</caption>
  <tr>
    <th>Nome</th>
    <th>Idade</th>
  </tr>
  <tr>
    <td>Maria</td>
    <td>22</td>
  </tr>
  <tr>
    <td>José</td>
    <td>25</td>
  </tr>
</table>
```
