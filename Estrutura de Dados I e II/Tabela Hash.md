## ✨ Conceitos

- 📌 O conceito de hash é que os registros armazenados em uma tabela são endereçados a partir de uma transformação aritmética sobre a chave de pesquisa;

- 📌 Complexidade: O(n);

- 📌 Tabelas de dispersão => tabelas de hash é um vetor cada uma de cujas posições armazena zero, uma ou mais chaves:
	- Uma tabela de símbolos é uma tabela com 2 colunas, sendo:
		- 1 coluna com as chaves (keys);
		- 1 coluna com os valores (values).
	- Cada linha da tabela é um item. Cada item associa um valor a uma chave;
	- Vetores, matrizes, listas ligadas, pilha, fila, são exemplos.

- 📌 **Parâmetros**:
	- M => número de posições na tabela de hash (valores)
	- N => número de chaves da tabela de símbolos (índices)
	- α = M / N : fator de carga

- 📌 **Hashing tem 2 ingredientes fundamentais**:
	- Função de hashing ou função de espalhamento => transforma cada chave em um índice da tabela de hash;
	- Mecanismo de resolução de colisões => dados podem ser duplicados, evita duplicatas

- 📌 Função de hashing transforma cada chave em um índice da tabela de hash;
- 📌 Espalha as chaves utilizando alguma lógica de espalhamento / balanceamento;
- 📌 A função de hashing espalha as chaves pela tabela de hash;
- 📌 A função de hashing associa um valor hash (hash value), entre 0 e M-1, a cada chave;
- 📌 A função de hashing produz uma colisão quando duas chaves diferentes têm o mesmo valor hash e portanto são levadas na mesma posição da tabela de hash.

## ✨ Função de hashing modular
- 📌 Chaves positivas utilizamos a função modular:
	- ***Resto da divisão*** por M:
	- M precisa ser primo

- Um exemplo:
	- `key 212` / M = 100, o resto disso dá **12**
	- `key 212` / M = 97, o resto disso dá **18**
	- `key 618` dividido por 100, o resto dá **18**
	- `key 618` dividido por 97, o resto dá **36**
 ---
