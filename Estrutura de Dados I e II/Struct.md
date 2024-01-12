## ✨ Explicação Struct

📌 Struct é uma estrutura de dados onde os elementos individuais podem ser de tipos diferentes.

📌 É uma coleção de variáveis referenciadas por um nome, através dela é possível agrupar informações relacionadas.

📌 Essa estrutura pode conter `int`, `float` e `char`. Ponteiros, matrizes e outros também podem ser elementos de uma Struct.

📌 Esses elementos individuais são chamados de _membros_.

---

## Definindo uma estrutura
```c
struct tag{
	membro1;
	membro2;
	membron;
};
```
`struct` => necessário para criar a estrutura;
`tag` => nome que identifica a estrutura, também chamado de id;
`membro1`... são as declarações dos membros individuais.

Outro exemplo de declaração de Struct:
```C
struct Conta{
	int numConta;
	char tipoConta;
	char nome[80];
	float saldo;
};
```
Aqui podemos declarar as variáveis de estrutura: `cliente novo` e `clienteantigo` do tipo Conta. 
```C
struct Conta clientenovo, clienteantigo;
```
Também há outra forma de representar as variáveis estrutura, que é já embutir elas ao final da declaração da Struct:
```C
struct Conta{
	int numConta;
	char tipoConta;
	char nome[80];
	float saldo;
}clientenovo, clienteantigo;
```

---

## Acessando e trabalhando com Estruturas

Sabendo que dentro do bloco de código de uma Struct, há membros que serão processados individualmente. Sendo assim, precisamos saber como acessar os membros individuais.
```C
variavel.membro
```

**Operador ponto (.)** => pertence ao grupo de maior precedência e sua associatividade é da esquerda para a direita.
**variável** => é o nome de uma variável Struct.
**membro** => é o nome de um membro da estrutura.

Para acessar o endereço do início da estrutura cliente, utiliza-se a seguinte expressão:
```C
&cliente.saldo;
```

E para acessar o endereço de um membro da expressão, é utilizado:
```C
&cliente.saldo;
```

Se o membro de uma estrutura é uma outra struct, então o membro da estrutura interna pode ser acessado dessa forma:
```C
variavel.membro.submembro
```

Um exemplo é: Considerando a struct *Conta*, para acessar o mês do último pagamento da variável estrutura *Cliente*:
```C
cliente.ultpag.mes
```

Também podemos acessar determinada posição na nossa estrutura, aqui um exemplo acessando o terceiro elemento da matriz `cliente.nome` da struct `Conta`:
```C
cliente.nome[2]
```
---
