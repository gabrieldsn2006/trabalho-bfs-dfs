# Trabalho BFS e DFS (Nordeste)
Este repositório implementa grafos e algoritmos de busca (BFS e DFS) em Python para o mapa dos estados do Nordeste do Brasil.

## Arquivos 
- `graph.py`: estrutura de grafo não direcionado com lista de adjacência (vértices, arestas, adição de arestas, iterador de adjacência).
- `breadth_first_paths.py`: classe `BreadthFirstPaths` para busca em largura a partir de um vértice origem, com métodos `has_path_to`, `path_to`, `dist_to`, `visit_order_to` e ordenação de visita (`order`).
- `depth_first_paths.py`: classe `DepthFirstPaths` para busca em profundidade a partir de um vértice origem, com métodos similares.
- `bag.py`: implementa uma coleção `Bag` para armazenar listas de adjacência e resultados de caminhos.
- `dados/nordeste.txt`: descreve grafo com 9 estados e fronteiras terrestres.
- `src/main.ipynb`: notebook de exemplo que usamos para executar os requisitos do trabalho

## Fluxo do notebook `main.ipynb`
1. importa módulos (`Graph`, `BreadthFirstPaths`, `DepthFirstPaths`, `pandas`).
2. define mapeamento de estados para índices (`AL`, `BA`, `CE`, `MA`, `PB`, `PE`, `PI`, `RN`, `SE`) e utilitários: `path_to_states`, `print_path`, `state`, `num`.
3. carrega o grafo de `dados/nordeste.txt` e imprime número de vértices/arestas.
4. define `ORIGEM` e `DESTINO` (ex.: `CE`, `SE`) e constrói instâncias `bfp` e `dfp` no vértice de origem.
5. verifica se destino é alcançável a partir da origem (`bfp.has_path_to(dst)`).
6. obtém e exibe caminho DFS e BFS entre origem e destino, convertendo índices em siglas.
7. lista estados alcançáveis via DFS.
8. exibe ordem de visita DFS e BFS e posições no caminho até o destino usando `visit_order_to`.
9. gera resumo completo com tabela pandas:
   - `Estado`,
   - `Alcançável`,
   - `Caminho DFS`,
   - `Caminho BFS`.

