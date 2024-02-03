## ✨ Operador sizeof

Quando declaramos uma struct, é alocado um espaço na memória para cada membro pertencente à estrutura, por exemplo:

| struct Conta | Espaço alocado| 
| -------- | -------- | 
| numConta | 2 bytes |
| tipoConta | 1 byte |
| nome[80] | 80 bytes |
| saldo | 4 bytes |
| dia | 2 bytes |
| mes | 2 bytes |
| ano | 2 bytes |

A função *sizeof* determina o número de bytes para um determinado tipo de dados.

Com esse operador, eu pego o tamanho da variável de forma dinâmica.

Dentro da struct temos variáveis, as mesmas possuem um determinado tamanho:

| Tipo de dado | Tamanho | 
| -------- | -------- | 
| char | 1 byte |
| short | 2 bytes |
| int | 4 bytes |
| long | 8 bytes |
| long long | 8 bytes |
| float | 4 bytes |
| double | 8 bytes |
| long double | 16 bytes |

Para determinar o número de bytes ocupados por uma estrutura, usamos o operador sizeof. Abaixo tem um exemplo em C:
```C
printf("%d\n", sizeof(clientenovo));
```

Esse comando equivale a:
```C
printf("%d\n", sizeof(struct Conta));
```

Ou seja, as variáveis de estrutura obtém o mesmo valor da concepção da estrutura em si.

Para saber a quantidade de bytes que uma estrutura tem, basta somar os valores de cada membro.

## ✨ Conversão bytes e bits

8 bits = 1 byte
bits para byte = dividir por 8

byte para bits = multiplicar por 8

- 📌 BIT (b) > BYTE (B) => divisão
- 📌 BYTE(B) > BIT (b) => multiplicação
	- b minúsculo = bits
	- B maiúsculo = bytes

- 📌 10 Mbps => 10 megabits por segundo
- 📌 10 Mbps / 8 = 1,25 MB (1,25 megabytes)
- 📌 800 bits = 100 bytes (foi dividido: 800 / 8 = 100)

- 📌 K = quilo = mil BYTES                       ==> (1.000)
- 📌 M = mega = milhões de BYTES       ==> (1.000.000)
- 📌 G = giga = bilhões de BYTES           ==> (1.000.000.000)
- 📌 T = tera = trilhões de BYTES           ==> (1.000.000.000.000)
