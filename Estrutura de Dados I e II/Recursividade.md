## ✨ Conceito

📌 Recursividade consiste em diminuir o problema em partes menores desse mesmo problema, tornando-se mais simples, até que o tamanho do mesmo permita resolvê-lo de forma direta, *sem recorrer a si mesmo*.

📌 Uma função é dita recursiva quando dentro do código há uma chamada para si mesma.
```python
#algoritmo recursivo
def fat(n):
	if(n == 0): #estrutura de condição
		return 1
	if(n > 0):
		return n * fat(n - 1) #chamando ela mesma
```

📌 Uma função não recursiva é aquela que utiliza laços de repetição, for, while, do while:
```python
#não recursivo
def fatNR(n):
	x = 1
	for i in range(2, n + 1): #note a estrutura de repetição
		x = x * i
	return x
```
- 📌 Requisitos para ser um algoritmo recursivo:
	- Toda recursividade precisa de uma condição de parada.
	- Deve conter pelo menos 1 estrutura de **condição/seleção**:
		- if
		- if-else
		- switch-case
	- Deve ter invocar a si mesmo pelo menos uma vez ao ser executado.

---

- 📌 Há 2 tipos de recursividade:
	- **Recursão direta**: Quando uma função chama a si mesma diretamente.
```C
	int imprimirDezPares(int p){
		if(p < 20){
			printf("%d, \t", p);
			imprimirDezPares(p + 2);
		}
	}
```

- **Recursão indireta**: Quando uma função chama outra, e esta, por sua vez chama a primeira.
```C
	int imprimirDezPares(int p){
		printf("%d,\t", p);
		trocaPar(p);
	}

	int trocaPar(int p){
		if(p < 18){
			imprimirDezPares(p + 2);
		}
	}
```

📌 Para todo algoritmo recursivo existe um outro correspondente iterativo, que executa a mesma tarefa. E aqui é usado o for, while, estruturas de REPETIÇÃO.

📌 Algoritmos recursivos possuem código mais claro, legível e mais compacto do que os iterativos.

- 📌A recursividade tem desvantagens, como:
	- Possui desempenho inferior a iteratividade; pois algoritmos iterativos consomem menos memória e tornam-se mais eficiente em termos de performance.
	- Consomem mais recursos, mais memoria e processamento do PC, devido ao uso intensivo da pilha.
	- São mais difíceis de serem depurados quando há várias chamadas simultâneas, não acessam a pilha com facilidade.

- 📌 O exemplo mais comum de recursividade, é o fatorial:
		$n! = \frac{1}{n * (n - 1)}$
		se n = 0
		se n > 0

- Basicamente os resultados no fatorial é um empilhamento de números e depois desempilhando para gerar a multiplicação.

- 📌 Diferenças de utilização de estruturas de repetição:
	- **for** => quando sabemos quantas iterações serão necessárias.
	- **while** => utilizado quando não sabemos quantas iterações serão necessárias, e a condição para continuar é avaliada antes de cada iteração.
	- **do while** => A condição é avaliada após a execução do bloco de código, garantindo que o bloco seja executado pelo menos uma vez.

---
