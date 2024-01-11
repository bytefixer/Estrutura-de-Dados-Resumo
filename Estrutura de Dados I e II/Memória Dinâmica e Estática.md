## Memória Dinâmica e Estática

📌 As informações utilizadas por um programa estão armazenadas na memória.

📌 Para que um programa consiga armazenar dados em uma área da memória, é necessário que esta área seja previamente alocada, ou seja, é preciso solicitar ao SO que reserve determinada área para o programa e a proteja, para que outros programas não possam acessar essa parte reservada.

📌 **Alocar** uma área de memória significa solicitar ao sistema operacional que reserve um espaço exclusivo para este programa.

---

## Alocação estática - memória Stack

📌 Quando o SO inicia um programa, ele aloca regiões de memória que serão utilizadas por esse programa. Porém, o tamanho dessas áreas de memória alocados é fixo, ou seja, não pode ser alterado durante a execução de um programa.

📌 Ás vezes algumas variáveis declaradas são usadas raramente e mesmo assim consomem memória, não faz sentido ela receber uma parte da memória. O programa estaria retendo uma quantidade de memória que poderia ser utilizada por outros programas.
   - O ideal seria alocar essa quantidade de memória pouco usada somente quando necessário e liberá-la para outros programas quando não fosse mais utilizada.

📌 A alocação estática acontece antes que o programa entre em execução.

📌 Cada variável tem seu endereço fixado e a área de memória ocupada por ela se mantém constante durante toda a execução do programa.

📌 São alocadas na **Stack** da memória RAM.
   - Toda variável declarada é alocada na memória Stack.

📌 A liberação de memória é feita automaticamente pelo SO.

---

## Alocação dinâmica - memória Heap

📌 O espaço é alocado dinamicamente *durante a execução do programa*.

📌 Pode ser criada ou eliminada durante a execução do programa, ocupando espaço na memória *apenas* enquanto está sendo utilizada.

📌 São alocadas na memória *Heap (free store)* da memória RAM.
   - Liberação de memória feita manualmente pelo programador.

`A memória Heap é muito maior que a memória Stack`

📌 A memória Heap é acessada exclusivamente através de ponteiros, diferentemente da memória Stack, que acessamos através de variáveis.

📌 Não é necessário especificar no inicio da execução do programa o tamanho do bloco de memória que o programa precisará. Durante a execução, o programa define o tamanho da área que necessita e solicita ao SO o uso exclusivo de uma área de memória deste tamanho.

📌 O SO reserva a quantidade necessária e devolve para o programa o endereço do primeiro byte da área de memória alocada. Então, o programa armazena esse endereço em um ponteiro e desta forma é possível acessar diretamente a área de memória em questão.

📌 Utilizamos alocação dinâmica quando não se sabe quanto de memória será necessário para o armazenamento dos elementos. Assim, o tamanho de memória necessário é determinado conforme a necessidade e dessa forma evita-se o desperdício de memória.

---

## ✨ Alocando e liberando memória - Funções

📌 Em compiladores antigos, a biblioteca *==malloc.h==* também era utilizada para alocar memória dinâmica.

📌 No padrão C ANSI, é definido apenas 4 funções para o sistema de alocação dinâmica, disponíveis na biblioteca ==*stdlib.h*==.

📌 As funções mais utilizadas da biblioteca *malloc.h* são: ==*malloc*== e ==*free*==.

### ☁ As 4 funções de alocação:
   - **malloc** - Memory Allocation
	   - Solicita ao SO alocar uma área de memória, em tempo de execução do tamanho especificado. É muito utilizada na implementação de EDD dinâmicas, como listas encadeadas.

**Sintaxe**:
```C
tipo* v = (tipo*) malloc(n * sizeof(tipo));
float* v = (float*) malloc(5 * sizeof(float)); 
//retorna o endereço do float
```

A função recebe como argumento o tamanho em bytes e devolve um ponteiro void* para o primeiro byte da área de memória alocada. Em caso de erro (não há memória suficiente), o valor é retornado *NULL*.

**As bibliotecas necessárias para utilizar a função malloc são: malloc.h e stdlib.h**

   - **calloc - Clear Allocation**
	   - É utilizada para alocar dinamicamente memória para um Array de elementos, cada um com um tamanho específico em bytes.
	   - O bloco de memória alocado é inicializado com zero.
		   - Essa é a diferença entre calloc e malloc. Calloc inicializa todos os bits da memória com 0, enquanto malloc apenas aloca a memória sem garantia que seja inicializada.
		   - Como a memória é iniciada em 0, é uma escolha conveniente se formos trabalhar com Arrays.
	   - O código abaixo utilizamos `numElements` sendo o números de elementos que desejamos alocar.
	   - E `elementsSize` para definir o tamanho em bytes de cada elemento.
	   
**Sintaxe**:
```C
tipo* v = (tipo*) calloc(n, sizeof(tipo));
float* v = (float*) calloc(5, sizeof(float));
```

   - **realloc**
	   - Função frequentemente usada para alterar o tamanho de um bloco de memória previamente alocado por `malloc`, `calloc` ou `realloc`.
	   - Pode ser utilizada para aumentar ou diminuir o tamanho do bloco de memória.
	
**Sintaxe**:
```C
void* realloc(void* ptr, size_t size);
```
- Onde `ptr` é um ponteiro para o bloco de memória já alocado.
- E `size` é o novo tamanho que desejamos para a memória, em bytes.

- **free**
	- É uma função para liberar uma área de memória já alocada pela função *malloc()*:
```C
void free(void *p);
```

A função recebe o argumento: o ponteiro para a área de memória alocada por malloc().

---

## Lixo de memória

📌 Esse termo se refere ao conteúdo indefinido ou não inicializado que pode ter em uma área de memória. É o resultado de operações anteriores no programa, dados que foram deixados para trás.

📌 Quando alocamos memória em variáveis locais, o conteúdo inicial dessa memória não é garantido, ou seja, os valores nessas áreas podem ser imprevisíveis e, muitas vezes, contêm lixo deixado por operações anteriores no sistema ou por outras partes do programa.

📌 Após liberar o bloco de memória, ainda teremos o endereço daquele bloco armazenado no ponteiro e consequentemente teremos acesso aos dados dele. O problema é que, liberando a memória, o sistema pode realocar aquela área para outro programa que a preencherá com outros dados, ou seja, os dados do seu programa podem se tornar inconsistentes a qualquer momento.

📌 A função *free()* não limpa ou redefine o conteúdo da memória, apenas marca a memória como disponível para reutilização.

📌 Se quisermos garantir que a memória alocada dinamicamente seja inicializa com zeros, podemos usar a função *calloc*, pois a mesma se inicializa com zeros.

---
