## `<p>` — elemento de parágrafo 

* O elemento HTML `<p>` representa um **parágrafo** de texto. 
* Na representação visual, parágrafos costumam aparecer como blocos de texto separados por espaço ou recuo, mas em HTML eles servem para agrupar conteúdos relacionados (texto, imagens, etc.). 
* É um elemento de **nível de bloco** (block-level). 
* Fechamento automático: se outro elemento de bloco iniciar antes da tag de fechamento `</p>`, o navegador implicitamente “fecha” o parágrafo anterior. 
* **Omissão de tag de fechamento**: em alguns casos, a tag de fechamento `</p>` pode ser omitida, conforme regras específicas — por exemplo, se outro elemento de bloco vier logo em seguida. 
* **Atributos**: aceita os atributos globais do HTML (como `class`, `id`, `style` etc.). 
* O atributo `align` (para alinhamento) está obsoleto e não deve ser usado; utilize CSS para controlar alinhamento. 
* **Acessibilidade**: segmentar o texto em parágrafos melhora a leitura por leitores de tela e outras tecnologias assistivas. 
* Evite usar `<p>` vazio apenas para criar espaçamento em branco, porque leitores de tela podem interpretar isso como um parágrafo vazio — prefira ajustar margens com CSS. 

---

## `<br>` — elemento de quebra de linha (break)

* O elemento `<br>` (break) insere uma **quebra de linha** no texto, equivalente a “enter” / retorno de carro em contexto visual.
* É útil quando a separação de linha faz sentido semanticamente (por exemplo, versos de poema, endereço postal).
* Não use `<br>` para criar espaçamentos extras entre blocos de texto — para isso, use CSS (ex: margens) ou elementos de bloco adequados.
* É um **elemento vazio** (não possui conteúdo interno ou tag de fechamento).
* Em HTML5, ele deve ser usado com uma tag de abertura (ex: `<br>`). Em XHTML, pode aparecer como `<br />`.
* Aceita os atributos globais.
* O atributo `clear`, que antigamente era usado para controlar como a quebra de linha “limpa” flutuações (floats) está **obsoleto** e **não deve mais ser utilizado** — prefira usar CSS moderno.

---