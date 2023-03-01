---
title: "Entendendo Processos e Threads"
description: "O post tem o objetivo de apresentar o que são Processos e Threads."
date: 2022-12-30T17:33:17-03:00
lastmod: 2022-12-30T17:33:17-03:00
featuredImage: "/images/entendendo-processos-e-threads/"
rssFullText: true
draft: false
---

## Introdução

Neste post eu pretendo desmistificar o que são Processos, Theads, Programação Paralela e Concorrente. 

Antes de ter que lidar com processos, threads ou programação paralela, eu procurei primeiramente entender mais sobre como funcionam os processadores da atualidade.

## O que é um Processo?

De maneira bem simples, um processo é um programa em execução. Quando temos um sistema operacional em execução, temos também uma coleção de processos sendo executados.

Essa coleção de processos consistem em:

- Processos de Sistema Operacional que executam código do sistema
- Processo de Usuário que executam código de usuário

Um programa, mantido em arquivo que contém uma lista de instruções, se torna uma entidade ativa quando executado. Ou seja, se torna um *processo* pois este é *"carregado"* em memória (load) e suas instruções são então executadas uma a uma pela CPU.



Os termos *job*, *processo* ou *tarefa* são usados de forma igual para representar um programa em execução. 

Sistemas operacionais do tipo *[time-sharing](https://en.wikipedia.org/wiki/Time-sharing)*



- No UNIX, existem dois níveis de tarefa: o processo e a thread. 

## Microprocessador e Sistema Operacional

*Microprocessador*, *CPU* ou *"Unidade Central de Processamento"*, é o cérebro do computador. Sua função é executar instruções, uma após a outra, que são obtidas da *[memória principal (RAM)](https://pt.wikipedia.org/wiki/Armazenamento_de_dados_de_computador#Armazenamento_prim%C3%A1rio)*.

A palavra *"processamento"* vem da ação de *processar dados*. É *"central"* do ponto de vista de arquitetura e também por sua importância, pois está no centro ou no meio, entre os demais dispositivos que formam um computador (dispositivos de E/S, memória principal, etc). Por último, é uma *"unidade"* visto que é um *[circuito integrado](https://pt.wikipedia.org/wiki/Circuito_integrado).*

A maioria dos microprocessadores da atualidade são *[multicore (multinúcleo)](https://pt.wikipedia.org/wiki/Processador_multin%C3%BAcleo)*. Isto quer dizer que há dois ou mais núcleos de processamento (cores) dentro da mesma pastilha de silício (um único chip que contém vários processadores). Temos então o equivalente a um ambiente *multiprocessado*, onde uma única CPU pode executar mais de uma instrução ao mesmo tempo (execução paralela). O sistema operacional trata cada núcleo como se fosse um processar diferente.

Com apenas um núcleo de processamento (singlecore), o sistema operacional divide o tempo de CPU entre os diversos programas (ou processos) em execução. Ou seja, cada programa é executado um pouco de cada vez, de forma intercalada. Como essa alternância de execução entre os programas ocorre de forma muito rápida, tem-se a ilusão de que a CPU consegue executar vários programas ao mesmo tempo.

O termo *[multitarefa](https://pt.wikipedia.org/wiki/Multitarefa)* é usado quando o sistema operacional é capaz de executar mais de uma tarefa por vez, seja de forma paralela/alternada ou não.


Visto que temos muitos modelos, separei alguns que eu tenho acesso direto. São eles:

- Intel Celeron (N3350)
- Intel Core i3
- Intel Core i7
- AMD Ryzen 7 (4000 Series)

Antigamente, para se ter o real multiprocessamento, era necessário ter mais de um processador na mesma placa-mãe. 

![alt_text](/images/entendendo-processos-e-threads/motherboard-dual-cpu.png  "Motherboard Dual-CPU")

*NOTA: Hoje em dia há alguns modelos de placas que possibilitam adicionar dois processadores.*



## Definição de Processo


