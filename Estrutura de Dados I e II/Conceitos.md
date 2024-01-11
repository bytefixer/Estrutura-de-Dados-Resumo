# Estrutura de Dados, ADT
📌 Uma estrutura de dados visa representar um processo sistemático para computar um resultado a partir de dados de entrada. Assim, nasce o termo algoritmo, que significa tratar os argumentos de forma lógica, como se fossem passos a serem seguidos com o objetivo de tirarmos conclusões.

📌 Estruturas de dados são uma **modelagem abstrata** dos objetos ou estruturas a serem manipuladas e das operações sobre eles.

📌 A **modelagem concreta** é relacionada aos Tipos Abstratos de Dados (ADT - Abstract Data Type).
- ADT é um tipo de dados que implementa objetos cujo comportamento é definido por um conjunto de valores e operações.
- São uma forma de simplificar operações em programação.
- Os principais tipos de ADTs são lista, pilha e fila.

📌 Um ADT é um modelo matemático que visa representar um conjunto de operações sobre um conjunto de valores. É normalmente representado através de uma especificação algébrica que contém 3 partes: Semântica, Sintática e Restrições.
- 📍 **Semântica**: trata do comportamento de um tipo abstrato de dados;
- 📍 **Sintático**: define a apresentação de um tipo abstrato de dados;
- 📍 **Restrições**: são responsáveis por estabelecer condições para a aplicação das operações.

---

## Dados homogêneos, dados heterogêneos
📌 *Dados homogêneos* são aqueles que possuem só **um tipo básico de dados**.
```python
lista = []
lista = ['leite', 'cafe']
print(lista)
```
No código acima, o vetor ``lista`` tem 2 strings como elementos, que são dados iguais. Dito isso, o output será uma lista de dados iguais; *homogênea*.

📌 *Dados heterogêneos* são aqueles que possuem **mais de 1 tipo básico de dados**.
```python
lista = []
lista = ['10', 'cafe']
print(lista)
```
Neste código, o vetor `lista` tem um número inteiro (10) e uma string (café). Portanto, o output desse código será uma lista de dados diferentes; *heterogênea*.

---

## Conceitos - Estruturas Lineares e Não Lineares
📌 Estruturas de dados lineares são aquelas em que os elementos são organizados em uma sequência linear, como listas, pilhas, filas.

📌 Cada elemento pode ter um único predecessor, menos o primeiro elemento e um único sucessor, menos o último.

📌 Podem ser consideradas como tendo duas extremidades, o nome mais comum pra elas são: topo e base.

📌 Estruturas de dados não lineares são aquelas em que os elementos são organizados de forma hierárquica, como árvores e grafos. Podem ter mais de um predecessor ou sucessor.

☁ **Pilha** é uma estrutura linear que permite adicionar e remover elementos somente no topo.

☁ **Fila** é uma estrutura de dados linear que permite adicionar elementos ao final e remover elementos pelo inicio.

☁ **Lista** é uma estrutura linear que permite adicionar, remover e acessar elementos em qualquer posição.

## Tipos de dados lineares:
- **Pilha**:
	- 💙 Armazenam itens um em cima do outro; como se fosse uma pilha de pratos por exemplo. Permite empilhar dados quando formos utiliza-los e desempilha-los quando quisermos remove-los.
	- 💙 Sempre que um elemento novo é inserido, o chamamos de TOPO, é o primeiro item que teremos acesso na pilha.
	- 💙 Pilha segue o padrão LIFO (Last In First Out), o último a entrar é o primeiro a sair.
	- 💙 O topo da pilha é sempre o último elemento que foi inserido.
	- 💙 Sempre que for remover um item, o último elemento da pilha é o primeiro a ser removido.
	- 💙 Pilhas são estruturas de dados muito complexas, porém estão entre as mais importantes.
	- 💙 É possível inserir objetos em uma pilha a qualquer momento, mas somente o objeto recentemente inserido poderá ser removido.
	- 💙 Na pilha, as operações básicas são:
		- 📍 push(): inserir no topo.
		- 📍 pop(): remover do topo
	- 💙 Pilha é uma estrutura de dados, uma lista linear, em que o inserção e remoção de elementos é restrito a APENAS UMA EXTREMIDADE, ou seja, somente iremos acessa-lo pelo topo da pilha, pelo último elemento inserido.
- **Fila**:
	- 💙 O primeiro elemento inserido, será o primeiro a ser retirado.
	- 💙 Serão adicionados elementos no fim da fila e removidos pelo inicio da fila, um exemplo bom seria: fila de banco, fila de caixa.
	- 💙 Pode-se dizer que é uma estrutura com 2 extremidades, retira-se pelo inicio e insere pelo fim.
	- 💙 Segue o padrão FIFO (First In First Out), o primeiro a entrar é o primeiro a sair.
	- 💙 Na fila, as operações básicas são:
		- 📍 enqueue: inserir na fila.
		- 📍 dequeue: retirar da fila.
- **Lista**:
	- 💙 Lista é uma estrutura linear que permite adicionar, remover e acessar elementos em qualquer posição.
	- 💙 Dados armazenados de forma sequencial, em estruturas chamadas de nós.
	- 💙 As listas podem ser implementadas por Arrays ou Listas Encadeadas. Mas o principal tipo é a **Lista Encadeada**.
	- 💙 Os dados são armazenados em nós, estruturas individuais compostas por um campo de informação e um campo de endereço e é aí onde há um ponteiro de ligação - link, que conecta ao próximo nó da lista.
	- 💙 A lista pode ser simples ou dupla:
		- 📍 Uma lista duplamente encadeada contém também ponteiros para elementos anteriores.
		- 📍 Uma lista encadeada também pode ser do tipo Circular, onde o último aponta para o primeiro.
 
  ---
