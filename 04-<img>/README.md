## O que é `<img>`

* O elemento **`<img>`** representa uma imagem embutida em um documento HTML. 
* É um elemento “vazio” (não tem conteúdo interno, não há fechamento) e sempre deve ter a tag de abertura. 

---

## Atributos principais

O elemento `<img>` suporta vários atributos — além dos atributos globais (como `class`, `id`, `style`, etc.). Aqui vão os mais importantes:

| Atributo           | Finalidade / Como usar                                                           |
| ------------------ | -------------------------------------------------------------------------------- |
| `src`              | **Obrigatório.** Especifica a URL da imagem que será carregada.                  |
| `alt`              | Texto alternativo que descreve a imagem. Exibido se a imagem não puder ser carregada ou para tecnologias assistivas. |
| `srcset`           | Define um conjunto de imagens com diferentes resoluções ou larguras, para permitir que o navegador escolha a mais adequada ao dispositivo. |
| `width` / `height` | Define dimensões desejadas da imagem (largura/altura).                           |
| `crossorigin`      | Permite controle de como a imagem é requisitada em contextos de CORS (relação com `<canvas>` etc). |
| `usemap`           | Associa a imagem a um “mapa de imagem” (imagem clicável com áreas definidas).    |
| `ismap`            | Indica que a imagem faz parte de um mapa de imagem do lado do servidor.          |

---

## Formatos de imagem suportados

* O padrão HTML em si não impõe uma lista fixa de formatos suportados — isso depende do navegador. 
* Exemplos de formatos comumente suportados incluem: JPEG, PNG, GIF (inclusive animado), SVG, BMP, entre outros. 
