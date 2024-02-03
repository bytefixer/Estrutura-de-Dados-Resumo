## ✨ Rotação SE, SD, DE, DD

###### SE -> Simples à Esquerda; SD -> Simples à Direita; DE -> Dupla à Esquerda; DD -> Dupla à Direita.

- 🎈 A transformação a ser feita na árvore para que ela fique balanceada, é chamada de rotação;
- 🎈 Para ajustarmos o fator de balanceamento, podemos rotacionar a sub árvore em torno do nó que está desbalanceado.
#
- 🎈 ***Simples à esquerda*** => Move a sub árvore da direita pra esquerda
	- 💡 Filho da direita vira a nova raiz;
	- 💡 A raiz original vira o filho da esquerda da nova raiz.
#
- 🎈 ***Simples à direita*** => Move a sub árvore da esquerda pra direita.
	- 💡 Filho da esquerda vira a nova raiz.
#
- 🎈 ***Dupla direita esquerda***:
	- 💡 Rotação primeiro para a direita;
	- 💡 A rotação ocorre primeiro no filho a direita que tá desbalanceado;
	- 💡 Depois roda para a esquerda.
#
- 🎈***Dupla esquerda direita***:
	- 💡 Rotação primeiro para a esquerda;
	- 💡 Depois roda para a direita.
#
- 🎈 ***Fator de balanceamento - Valores***:
	- 💡 Se o FB é negativo, tá pendendo para a direita -> as rotações são feitas à direita;
	- 💡 Se o FB é positivo, tá pendendo para a esquerda -> as rotações são feitas à esquerda.
#
- 🎈 ***Regras de operação de rotação***:
	- 💡 Inserção a direita no filho da direita => rotação a esquerda;
	- 💡 Inserção a esquerda no filho da esquerda => rotação a direita;
	- 💡 Direita no filho da esquerda => rotação esquerda-direita;
	- 💡 Esquerda no filho da direita => rotação direita-esquerda.
 ---
