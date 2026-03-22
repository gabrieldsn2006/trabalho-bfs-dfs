# trabalho-bfs-dfs

## Entrada

O programa deve receber como entrada:

- um estado de origem `X`
- um estado de destino `Y`

## Perguntas que o programa deve responder

- É possível sair do estado de origem `X` e chegar ao estado de destino `Y` atravessando apenas fronteiras terrestres?
- Qual caminho foi encontrado pela `DFS` do estado de origem `X` até o estado de destino `Y`?
- Qual caminho foi encontrado pela `BFS` do estado de origem `X` até o estado de destino `Y`?
- Quais estados são alcançáveis a partir do estado de origem `X`?
- Qual foi a ordem de visita dos estados na execução da `DFS` a partir de `X`?
- Qual foi a ordem de visita dos estados na execução da `BFS` a partir de `X`?

## Pontuação

- Verificar se o estado de origem `X` alcança o estado de destino `Y`: `0,10`
- Informar o caminho encontrado por `DFS`: `0,20`
- Informar o caminho encontrado por `BFS`: `0,20`
- Informar quais estados são alcançáveis a partir do estado de origem `X`: `0,20`
- Informar a ordem de visita da `DFS`: `0,15`
- Informar a ordem de visita da `BFS`: `0,15`

## Critérios de avaliação

- Correção da modelagem do grafo, com vértices e arestas compatíveis com as fronteiras terrestres dos estados do Nordeste.
- Uso adequado dos algoritmos `DFS` e `BFS` em `algs4`.
- Resposta correta às perguntas propostas no enunciado.
- Clareza na organização do código e na exibição da saída.
- Adequação da estrutura do projeto à linguagem escolhida.

## Requisitos

- Implementar a solução em Python ou em Java.
- Representar o grafo por lista de adjacência.
- Construir a lista de arestas com os estados do Nordeste e suas fronteiras terrestres.
- Use a ordem alfabética para mapear os vértices. Ex.: 0: AL, 1: BA, ...
- Use a ordem crescente na construção da lista de arestas. Ex.: 0 1, 0 3, 1 2, 1 7, ...
- Permitir informar origem e destino.
- Exibir os resultados de forma clara.