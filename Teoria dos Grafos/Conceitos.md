###### {study.log 06.02.2024}
## ✨ O que é Teoria dos Grafos?

- Área da matemática combinatória voltada à resolução de problemas em computação;
- É um campo dedicado à análise das relações entre elementos de um conjunto específico;
- Estuda a relação entre objetos de um conjunto;
- Muitas aplicações em computação precisam considerar um conjunto de conexões entre pares de objetos:
	- O menor caminho entre dois objetos;
	- Ir de um objeto a outro seguindo conexões;
	- Quantos outros pontos consigo atingir a partir de um determinado objeto;
- Exemplos de problemas práticos que podem ser modelados com grafos:
	- WEB:
		- Ajudar máquinas de busca a localizar informação relevante;
		- Documentos conectados por links;
	- Mapas:
		- Descobrir o roteiro mais curto para visitar as principais cidades de uma região turística;
		- Cidades conectadas por estradas;
	- Redes Sociais:
		- Descobrir pesquisadores com o maior número de colaboradores de outros países;
		- Pesquisadores conectados por projetos de pesquisa;
	- Modelagem de circuitos eletrônicos;
	- Redes de transporte/Energia;
	- Redes de computadores;

## ✨ O que são Grafos?

- Estruturas abstratas que modelam objetos com existência de relação (conexão) entre eles;
- Para o estudo de um conjunto, são utilizadas estruturas nomeadas de Grafos, onde sua fórmula é:
	- G (V, A), onde:
		- V = é um conjunto não vazio de objetos chamado vértices (ou nós);
		- A = é um subconjunto de pares não ordenados de V, chamado de arestas;
	- Também há o nome em inglês G (V, E), onde:
		- V = Vertices (vértices);
		- E = Edges (arestas);

## ✨ 2 Tipos de grafos

- <mark style="background: #FFF3A3A6;">Conexos</mark>: Aquele em que todos os pontos possuem pelo menos uma aresta;
	- Pontos separados, onde há um caminho;
- <mark style="background: #FFF3A3A6;">Não conexo</mark>: Uma parte separada;
	- Algo que não consigo alcançar;
	- Sem conexão;
	- Não tem caminho entre os pontos;
	- Sem ligação do ponto A com o B;

## ✨ Caminho entre os grafos

- Percurso entre um vértice a outro vértice;
- Nem sempre o menor caminho é o melhor caminho e vice versa, depende do algoritmo;
- Normalmente não tem repetição de vértice;

## ✨ Circuito

- Um caminho fechado, um loop, voltando pro mesmo ponto inicial

## ✨ Ciclo de tamanho

- Total de arestas que passou, quantas arestas ele passa do inicio até o final (voltando pro ponto inicial)

## ✨ Grau de um vértice

- Quantidade de arestas que saem do vértice;
- A partir de um ponto, é a contagem de arestas a partir dele;
- d(v) ex: d(A) = 4

# Grafos direcionados e não direcionados

## ✨ Definição - Grafo direcionado (Dígrafo)

- Um grafo direcionado (também chamado de grafo orientado ou dígrafo) G é um par (V,A) em que:
	- V é um conjunto finito de vértices;
	- A é um conjunto de arestas;
- Uma aresta (u, v) sai do vértice u (origem) e chega no vértice v (destino)
- <mark style="background: #FFF3A3A6;">Self-loops</mark>: Arestas de um vértices para ele mesmo;
- <mark style="background: #FFF3A3A6;">Arestas múltiplas</mark>: Arestas com mesma origem e mesmo destino;



