# :pencil: Guia Markdown simples

## :paperclip: Índice
- [Guia Markdown simples](#pencil-guia-markdown-simples)
- [Índice](#paperclip-índice)
- [Sobre](#dart-sobre)
- [Títulos](#pencil2-títulos)
- [Parágrafo](#clipboard-par%C3%A1grafo)
- [Negrito](#b-negrito)
- [Itálico](#%E2%84%B9%EF%B8%8F-it%C3%A1lico) 
- [Riscado (strike)](#x-riscado-strike) 
- [Listas](#bookmark_tabs-listas) 
  - [Listas numeradas](#1234-listas-numeradas) 
  - [Listas com marcadores](#hash-listas-com-marcadores) 
  - [Listas de tarefas](#pencil-listas-de-tarefas)
- [Imagens](#camera-imagens)
- [Links](#link-links)
- [Trechos de código](#computer-trechos-de-c%C3%B3digo)
- [Emojis](#smiley-emojis)
- [Tabelas](#bar_chart-tabelas)
- [Quote](#speech_balloon-quote)
- [Símbolos reservados](#symbols-s%C3%ADmbolos-reservados)
- [Linhas](#straight_ruler-linhas)
- [Referências](#page_with_curl-referências)

## :dart: Sobre 
Olá, este guia foi criado durante o mini curso sobre Markdown ministrado por mim durante o ***Hacktoberfest OpenDevUFCG*** com o intuito de ajudar você à encontrar os principais marcadores/formatadores da linguagem Markdown.

## :pencil2: Títulos

Para criar títulos, pode-se usar de um # até seis ###### para definir o nível (tamanho) do
título.

\# Exemplo 
 # Exemplo
 
\## Exemplo 
## Exemplo

\### Exemplo 
### Exemplo

---
\#### Exemplo 
#### Exemplo
---

\##### Exemplo 
##### Exemplo
---

\###### Exemplo
###### Exemplo

--- 
## :clipboard: Parágrafo

Para escrever páragrafos não temos uma formatação, basta escrever de forma contínua.

Basta escrever mesmo, e nada mais...

## :b: Negrito

Para usar o **negrito**, basta usar asteriscos duplos ao redor da palavra ou frase.

Exemplo:

**OpenDevUFCG** 

## ℹ️ Itálico

Para colocar uma palavra em *itálico*, pode-se colocá-la entre um asterisco ao derredor da palavra ou frase.

\*OpenDevUFCG*

Exemplo:

*OpenDevUFCG*

## :x: Riscado (strike)

Para ~~riscar~~ uma palavra ou frase, basta adicionar ao seu redor dois símbolos de til.

\~~OpenDevUFCG~~

Exemplo:

~~OpenDevUFCG~~

## :bookmark_tabs: Listas

### :1234: Listas numeradas

Para criar uma lista numerada, pode-se iniciar a linha utilizando qualquer número e um ponto, os demais números da lista seguirão
a sequência com base no primeiro número adicionado.

Exemplo:

1. Python
8. Java
4. JavaScript
2. C++

### :hash: Listas com marcadores

Basta usar um hífen seguido de um hífen para seja criada de uma lista com marcadores.

\- Python

Exemplo:
- Python
- Java
 - JavaScript
- C++
- EXEMPLO

### :pencil: Listas de tarefas

Adicionando \- \[ ] ou \- \[x] antes de cada item, pode-se criar uma "to do list" com
itens marcados ou desmarcados.

Exemplo:
- [ ] Header
- [x] Card dropdown
- [X] EXEMPLO 

## :camera: Imagens

Para inserir uma imagem, usa-se o símbolo \!\[ ]\( ) onde a descrição fica contida nos
colchetes e o endereço da imagem contida entre parênteses.

Ex:
<div align=left>
 <img width=300 src='https://opendevufcg.org/home/img/opendevufcg_logo.svg'/>
 </div>
 
 Obs: Neste caso está sendo utilizado HTML para que seja controlado o tamanho e a posição.
 
 Exemplo: 
 \!\[Logo Opendev](https://opendevufcg.org/home/img/opendevufcg_logo.svg)

## :link: Links

Para inserir links, basta remover a ! utilizada para utilizar imagens. 

\[Site OpenDevUFCG](https://opendevufcg.org/)

Exemplo:
[Site OpenDevUFCG](https://opendevufcg.org/)

## :computer: Trechos de código

Comando isolado

Se for citar um comando apenas, basta colocá-lo entre crases.

\`console.log('Hello world)`

Exemplo:

`console.log('Hello world)`

Trecho de código
Para compartilhar um código com mais linhas, basta colocar todas elas dentro de um
grupo delimitado entre três crases consecutivas (sem espaço entre elas).


``` jsx
const handleClick = useCallback(
        () => {
            setCurrentFilter(title)
        },
    )
```

\``` py
print("Hello world")
\```

Exemplo:

``` py
print("Hello world")
```

## :smiley: Emojis

Existem códigos especiais para emojis em Markdown, que devem ser representados entre símbolos de ::

:nome_do_emoji:

Exemplo:

:pencil:

> Você pode encontrar os nomes dos emojis [aqui](https://gist.github.com/rxaviers/7360908).

## :bar_chart: Tabelas

Criar tabelas em Markdown basta usar os pipes | e os hifens -

Nome \| Tipo \| Descrição \| Programador(a)

\:---: \| \---: \| \:--- \| \:---:

imageURL\| string \| varíavel que recebe o link com endereço de imagem \| Leandra

title \| string \| varíavel que recebe o título do comércio \| Rodrigo

Exemplo:

Nome | Tipo | Descrição | Programador(a)
:---: | ---: | :--- | :---:
imageURL| string | varíavel que recebe o link com endereço de imagem | Leandra
title | string | varíavel que recebe o título do comércio | Rodrigo


--- Formatação padrão (alinhamento à esquerda)

:---: Conteúdo Centralizado

---: Alinhamento à direita

:--- Alinhamento à esquerda

## :speech_balloon: Quote

Ao responder alguém, podemos realizar citações a outras mensagens completas ou a
trechos dela, usando sinais de > no início da linha.

\> João disse que Leandra forneceu este dado para o componente cardCategory

> João disse que Leandra forneceu este dado para o componente cardCategory

## :symbols: Símbolos reservados

Como os símbolos utilizados em Markdown são os mesmos que utilizamos para escrever em qualquer outro arquivo
pose acontecer de nós precisarmos usar um sinal desse, para isso, basta adicionar uma \ (contrabarra) na frente do símbolo, para que o símbolo seja apresentado na tela.

Exemplo:
Pode-se usar \# para criar um título semelhante ao `<h1>` do HTML.

## :straight_ruler: Linhas

Para utilizar uma linha, basta utilizar \---

--- 

## :page_with_curl: Referências

- [Guia Markdown Gustavo Guanabara - Curso em Vídeo](https://github.com/gustavoguanabara/git-github/blob/master/manuais-PDF/guia-markdown.pdf)
- [Documentação Markdown - Markdown Guide](https://www.markdownguide.org/getting-started/)

