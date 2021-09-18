# :pencil: Guia Markdown simples

## Índice
- [Guia Markdown simples](#pencil-guia-markdown-simples)

Olá, nesse guia você vai encontrar os principais marcadores/formatadores da linguagem markdown.

## Títulos

Para criar títulos, pode-se usar de um # até seis ###### para definir o nível (tamanho) do
título.

# Exemplo
## Exemplo
### Exemplo
#### Exemplo
##### Exemplo
###### Exemplo

## Parágrafo

Para escrever páragrafos não temos uma formatação, basta escrever de forma contínua.

Basta escrever mesmo, e nada mais...

## Negrito

Para usar o **negrito**, basta usar asteriscos duplos ao redor da palavra ou frase.

Exemplo:

**OpenDevUFCG** 

## Itálico
Para colocar uma palavra em *itálico*, pode-se colocá-la entre um asterisco ao deredor da palavra ou frase.


Exemplo:

*OpenDevUFCG*

## Riscado (strike)
Para ~~riscar~~ uma palavra ou frase, basta adicionar ao seu redor dois símbolos de til.

Exemplo:
~~OpenDevUFCG~~

## Listas

### Listas numeradas

Para criar uma lista numerada, pode-se iniciar a linha utilizando qualquer número e um ponto, os demais números da lista seguirão
a sequência com base no primeiro número adicionado.

Exemplo:

1. Python
8. Java
4. JavaScript
2. C++

### Listas com marcadores

Basta usar um hífen seguido de um hífen para seja criada de uma lista com marcadores.

Exemplo:
- Python
- Java
 - JavaScript
- C++
- EXEMPLO

### Listas de tarefas

Adicionando - [ ] ou - [x] antes de cada item, pode-se criar uma "to do list" com
itens marcados ou desmarcados.

Exemplo:
- [ ] Header
- [x] Card dropdown
- [X] EXEMPLO 

## Imagens

Para inserir uma imagem, usa-se o símbolo ![ ]( ) onde a descrição fica contida nos
colchetes e o endereço da imagem contida entre parênteses.

Ex:
<div align=left>
 <img width=300 src='https://opendevufcg.org/home/img/opendevufcg_logo.svg'/>
 </div>
 
 ![Logo Opendev](https://opendevufcg.org/home/img/opendevufcg_logo.svg)

## Links

Para inserir links, basta remover a ! utilizada para utilizar imagens. 

Ex:
[Site OpenDevUFCG](https://opendevufcg.org/)

## Trechos de código

Comando isolado

Se for citar um comando apenas, basta colocá-lo entre crases.

Exemplo:

`console.log('Hello world)`


Trecho de código
Para compartilhar um código com mais linhas, basta colocar todas elas dentro de um
grupo delimitado entre três crases consecutivas (sem espaço entre elas).

Ex:

``` jsx
const handleClick = useCallback(
        () => {
            setCurrentFilter(title)
        },
    )
```

``` py
print("Hello world")
```

## Emojis

Existem códigos especiais para emojis em markdown, que devem ser representados
entre símbolos de ::


Exemplo:
Este é um guia sobre markdown :pencil:

## Tabelas

Criar tabelas em markdow basta usar os pipes | e os hifens -

Exemplo:

Nome | Tipo | Descrição | Programador(a)
:---: | ---: | :--- | :---:
imageURL| string | varíavel que recebe o link com endereço de imagem | Leandra
title | string | varíavel que recebe o título do comércio | Rodrigo


--- Formatação padrão (alinhamento à esquerda)
:---: Conteúdo Centralizado
---: Alinhamento à direita
:--- Alinhamento à esquerda

Exemplo1| Exemplo2 
:---: | :---:
exemplo1 | exemplo2

Quote

Ao responder alguém, podemos realizar citações a outras mensagens completas ou a
trechos dela, usando sinais de > no início da linha.


> João disse que Leandra forneceu este dado para o componente cardCategory

> Exemplo


Utilizando símbolos reservados

Como os símbolos utilizados em markdown são os mesmos que utilizamos para escrever em qualquer outro arquivo
pose acontecer de nós precisarmos usar um sinal desse, para isso, basta adicionar uma / na frente do símbolo, para que o símbolo
seja apresentado na tela.

Exemplo:
Pode-se usar \# para criar um título semelhante ao `<h1>` do HTML.

