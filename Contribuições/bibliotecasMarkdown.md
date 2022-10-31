# Bibliotecas que renderizam Markdown em seus sites.

Várias linguagens possuem suporte à formatação e exibição de Markdown através de bibliotecas específicas. Neste artigo, exploraremos algumas destas bibliotecas em certas linguagens de programação populares.

## Python
As duas principais bibliotecas que renderizam Markdown são:

### [Python-Markdown](https://python-markdown.github.io)

* Possui algumas features diferenciais como suporte a diversas línguas.
* Suporte a extensões de diversos sistemas web.
* Diversos formatos de saída (não apenas HTML).
* Possui uma CLI (Command Line Interface) para realizar operações em tempo real.

### [Jupyter Notebook](https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Working%20With%20Markdown%20Cells.html)

É uma ferramenta muito popular (principalmente para análise de dados). E tem integração nativa com Markdown (para estilização de headers de células).

## Javascript

### [Marked](https://github.com/markedjs/marked)
Biblioteca JS focada principalmente em:
* Construída para operar rapidamente;
* Funciona em servidores, browser ou terminais;
* Altamente leve e baixo nível de interrupção.

### [MermaidJS](https://mermaid-js.github.io/mermaid/#/)
Esta biblioteca permite criar visualizações e diagramas a partir de documentos Markdown. Alguns exemplos de diagramas podem ser vistos abaixo.

![MermaidJS](https://mermaid-js.github.io/mermaid/img/header.png)


## Java

### [Commonmark](https://github.com/commonmark/commonmark-java)

Esta biblioteca foi adaptada do Javascript, e utiliza o [mecanismo de Commonmark](https://commonmark.org) para contornar os problemas de ambiguidade, com pouquíssimas dependências externas e bastante rápido.

### [Flexmark](https://github.com/vsch/flexmark-java)

Biblioteca que substituiu o Pegdown (antiga biblioteca mais popular de Java para Markdown). Possui um enorme número de extensões e funcionalidades customizáveis.

## R

### [R Markdown](https://rmarkdown.rstudio.com/)

*R Markdown* é uma ferramenta que possibilita a criação de documentos e apresentações com *Markdown* e trechos de código em *R*. Faz parte da IDE [RStudio](https://www.rstudio.com/) e, para usar a ferramenta, basta criar um novo arquivo do tipo *R Markdown*. Os documentos e apresentações podem ser exportados em vários formatos, como HTML, PDF e Word.

Exemplo de código *R Markdown* no *RStudio*:
![Exemplo R Markdown no RStudio](https://user-images.githubusercontent.com/68706339/199090987-06d43a9d-8b46-4816-9a17-60a88b6d91e4.png)
