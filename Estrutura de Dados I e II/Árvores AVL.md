## ✨ Explicação
- 📌 Toda AVL é uma árvore binária;
- 📌 A nomenclatura "AVL" significa => Adelson-Velskii e Landis;
- 📌 Árvore cheia é uma árvore já balanceada;
- 📌 O termo "árvore não AVL" significa uma árvore de busca binária normal, sem balanceamento;
- 📌 Complexidade: O(log n);
- 📌 Arvore AVL / para balancear = altura do nó é 0;
- 📌 Arvore normal e binaria = altura do nó é 1;

- 📌 Devemos verificar a altura da árvore binária;
- 📌 Depois verificar a altura das sub-árvores da direita e da esquerda;
- 📌 Fator de balanceamento = altura nó esquerda - altura nó direita;
- 📌 O cálculo de altura é feita SEMPRE em módulo. | |, o resultado sempre será positivo:
	- | Altura da esquerda - altura da direita |, TUDO em módulo.
	- O calculo pode ser feito da seguinte forma:
		- O meu nó tem 1 filho pra esquerda e 0 pra direita:
		`1 - 0 = 1`
		- O meu nó tem 0 filho na esquerda e 1 na direita:
		`0 - 1 = -1`
		- O meu nó tem 0 esquerda, 2 direita:
		`0 - 2 = -2`

- 📌 Passo a passo do cálculo:
	- 📌 Comece colocando 0 em todos os nós folhas;
	- 📌 Faça o caminho todo pela esquerda até a raiz e depois passe pra direita, calcule cada nó;
	- 📌 Pegue um nó de referencia e conte os nós filhos que ele tem, depois subtraia os filhos entre si.

- 📌 O calculo de balanceamento é:
	- O resultado precisa ser -1, 0, 1 e isso é uma arvore balanceada;
	- Se estiver acima de 1 (2 ou mais) é porque está desbalanceada.
