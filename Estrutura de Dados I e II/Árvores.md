## ✨ Explicação

📌 Árvores são estrutura de dados hierárquicas, ou há subordinação.

📌 Um subconjunto dos componentes é subordinado a outro.

📌 Relacionamento lógico.

📌 Complexidade: O(n)

📌 A raiz da árvore, que está no nível 0, é o *topo da hierarquia*, possui filhos mas não possui pai.

📌 Um nó em um determinado nível está conectado a seus filhos (nível abaixo) e a seu pai (nível acima).

📌 Uma árvore não retorna do nó filho para o pai, o filho não pode ser o pai do próprio pai.

📌 Árvores são formadas por um conjunto de elementos, os quais chamamos de nodos (ou vértices) conectados por um conjunto de arestas.

- 📌 ***Diagrama de inclusão***: Pode-se dizer que a raiz é como o *conjunto universal* na teoria dos conjuntos, ou seja, a raiz é o conjunto universal que abriga todos os outros elementos:
	- No contexto de nós, a raiz engloba todos os nodos, os nós das sub árvores são os conjuntos restantes e a cada nó há outros dentro deste conjunto.

- 📌 Onde utilizamos árvores?
	- Pasta do Explorer.
	- Histórico da WEB.
	- Rotas de um trajeto.
	- Chaves de jogos de times de futebol.
 
- 📌 Se o número de nós é igual a zero, chamamos de *árvore vazia*.

## ✨ Terminologias

- ***Raiz***: nó origem da árvore.
- ***Nó folha (nó terminal ou externo)***: nós que não tem filho, de grau 0.
- ***Nó interno (nó de derivação)***: nós que estão no caminho entre a raiz da árvore e os nós folha, maior que zero.
- ***Grau de um nó***: número de filhos de um nó (número de sub arvores de um nó)
- ***Grau de uma árvore***: número máximo entre os graus de seus nós.
	- Grau 0 => 0 filhos
	- Grau 1 => 1 filho
	- Grau 2 => 2 filhos
	- Grau 3 => 3 filhos
- ***Nível de um nó***: comprimento do caminho da raiz até o nó que queremos chegar.
	- Cima para baixo, da raiz para as folhas.
	- ***O nível começa em 1, de cima para baixo***.
	- Nível 1 = raiz.
	- Nível 2 = filhos do nível 1.
	- Nível 3 = filhos do nível 2.
	- Nível 4 = filhos do nível 3.
- ***Altura ou profundidade***: nível mais alto da árvore, comprimento do caminho mais longo entre a raiz da árvore e suas folhas.
	- Baixo para cima, das folhas para a raiz.
	- ***A altura começa em 1, de baixo para cima***.
	- A altura (profundidade)é o máximo de nível de seus nós.
	- A menor altura são os últimos elementos.
	- A altura do nó folha é 1.
- ***Aresta de uma árvore***: linha que liga 2 nós da árvore.
- ***Comprimento do caminho***: número de ligações entre os nós do caminho, número de arestas.
- ***Percurso em nível (ou largura)***: contagem dos nós, por nível, da esquerda para a direita.
- ***Floresta***: conjunto de árvores.
- ***Galhos***: nós que não são raiz e nem folhas, nós internos.
- ***Isomorfas***: Árvores que podem se tornar simultâneas nas sub árvores, ou seja, podem fazer uma "inversão" nas sub árvores. Tem a mesma estrutura, independente do valor dos nós.
- ***Árvore estritamente binária***: cada nó possui 0 ou 2 filhos.
- ***Árvore binária cheia***: todas as sub árvores vazias se localizam no último nível.
- ***Árvore binária completa***: sub árvores vazias apenas no último ou penúltimo nível.
- ***Árvore binária zigzag***: cada nó interior possui exatamente um filho (esquerdo ou direito).

- 📌 Árvore ordenada: Uma árvore é ordenada quando os filhos estão ordenados, da esquerda pra direita.
	- O valor de cada nó na ***esquerda é MENOR*** que o valor da raiz.
	- O valor de cada nó na ***direita é MAIOR*** que o valor da raiz.
---
