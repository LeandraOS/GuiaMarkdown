# ⋆⁺₊⋆Programação Concorrente⋆₊⁺⋆ *uma pequena introdução*

<img src="https://c.tenor.com/r2_RSuOMIwIAAAAC/whisper-of-the-heart-cartoon.gif" width="350" align="right">

## :paperclip: Índice

- [Uma pequena introdução à Programação Concorrente](#⋆⁺₊⋆programação-concorrente⋆₊⁺⋆-uma-pequena-introdução)
- [Índice](#paperclip-índice)
- [Introdução](#pencil2-introdução)
- [Porque Programação concorrente](#thinking-porque-precisamos-de-programação-concorrente)
- [Programação Concorrente X Programação Paralela](#bulb-programação-concorrente-x-programação-paralela)
- [Implementação de sistemas concorrentes](#computer-maneiras-de-implementar-sistemas-concorrentes)
- [Conceitos importantes](#books-conceitos-importantes)
- [Exclusão mútua](#bookmark_tabs-requisitos-para-solução-de-exclusão-mútua)
- [Como soluciono a Condição de Corrida???](#runner-como-soluciono-a-condição-de-corrida)
- [Semáforo](#vertical_traffic_light-semáforo)

## :pencil2: Introdução

Como diz o título, esta será uma pequena introdução ao tema de programação concorrente e alguns conceitos prévios importantes.
### O que é Programação Concorrente, afinal?
- A **Programação Concorrente** é um paradigma de programação que possibilita a criação de programas de computador com execução simultânea de tarefas computacionais, estas podem ser implementadas como programas separados ou como um conjunto de threads criado por um único programa. Essas tarefas podem ser executadas por um único processador, vários processadores em um único equipamento ou processadores distribuídos por uma rede.

## :thinking: Porque precisamos de programação concorrente?

Os principais motivos são:
1. **Desempenho**: programas concorrentes trazem melhorias no quesito de desempenho, pois fazem com que alguns fluxos não precisem esperar o término de outros para iniciar. A existência de vários processadores faz com que a programação concorrente faça ainda mais sentido.
2. **Responsividade**: um exemplo clássico é fazer com que a movimentação do  mouse seja independente do carregamento do background de alguma interface gráfica, essas coisas precisam acontecer de maneira paralela para que haja responsividade entre a ação do usuário e a resposta do computador.

*Existem também tarefas que são por natureza concorrentes.*


## :bulb: Programação Concorrente X Programação Paralela

Em computação, **paralelismo** é a execução simultânea de instruções. Pode ocorrer, por exemplo, ao executar duas tarefas iguais, mas com diferentes dados, em dois processadores diferentes do mesmo computador, ou em computadores diferentes.
Exemplo: cada processador está computando um quadrante diferente de um mapa.

*Todo sistema paralelo é concorrente.*

**Um programa é concorrente** quando possui tarefas, ou fluxos, que podem ser executadas em ordens diferentes.


## :computer: Maneiras de implementar sistemas concorrentes

- **Shared Memory** (memória compartilhada): num contexto onde existem vários fluxos de execução (várias threads ou processos), ao realizar computações, esses fluxos precisarão eventualmente de compartilhar memória.

- **Troca de mensagem**: neste método, ao invés de compartilhar memória, os processos se comunicam entre si para atualização ao fim da computação.


## :books: Conceitos importantes

- **Região Crítica**: é um trecho de código que está sujeito a uma condição de corrida.
- **Condição de Corrida**: é um condição em que, a depender de como os fluxos de execução são escalonados, o resultado final da computação pode ser diferente.
- **Exclusão mútua**: é uma técnica para evitar a condição de corrida que garante que só um fluxo de execução execute a região crítica por vez.

     ~~*ps.: definições do prof Manel*~~


## :bookmark_tabs: Requisitos para solução de exclusão mútua:

1. Deve **garantir a exclusão mútua** no acesso às regiões críticas.
2. Não pode fazer hipóteses sobre o número de processadores ou a velocidade relativa dos processadores.
3. Só deve impedir que um fluxo entre na região crítica se outro fluxo estiver usando a região crítica.
4. Deve evitar **inanição (starvation)**, ou seja, todos os fluxos precisam ganhar em algum momento a região crítica para que eles possam avançar na sua computação.

## :runner: Como soluciono a Condição de Corrida???

Uma solução possível é a **espera ocupada** (busy wait), para isso é necessário que haja adição de um trecho de código que checa se a região crítica já está sendo executada por outro fluxo, caso positivo, a região crítica não será executada e o fluxo permanecerá num loop de espera até que a mesma seja liberada e ele possa executá-la. Ao fim da execução haverá algum código sinalizando que a região crítica não estará mais sendo usada por aquele fluxo.

## :vertical_traffic_light: Semáforo:

Bom, quando se trata de concorrência quase tudo é resolvido usando semáforos.

### E o que são esses tais semáforos?

⋆⁺₊⋆ O semáforo é uma variável especial protegida (ou tipo abstrato de dados) que tem como função controlar o acesso a recursos compartilhados ⋆⁺₊⋆

### Ele funciona assim:

1. É inicializado com um valor inteiro associado;
2. Esse valor pode ser alterado através de duas operações:
    - signal (incremento)
    - wait (decremento);
3. Quando uma thread executa a operação wait de um semáforo e o valor ficar negativo, a thread bloqueia;
4. Quando uma thread executa a operação signal e o valor não for mais negativo, se houverem threads bloqueadas, uma delas é desbloqueada.

Bem... É isso por enquanto ☾ ⋆⁺₊⋆

Muito obrigada por chegar até aqui! Espero que você tenha sido motivado a procurar mais sobre o assunto 💜

<div align="center">
    <img src="https://i.pinimg.com/originals/c5/44/fa/c544fac358589c8374a588cda0a1317c.gif" width="350">
</div>