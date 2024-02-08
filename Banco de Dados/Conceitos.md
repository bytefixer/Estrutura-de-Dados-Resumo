###### {study.log 08.02.2024}

- Áreas comuns:
	- WEB;
	- Frontend;
	- Backend;
- Áreas menos disputadas:
	- BI;
	- Segurança;
	- Software Embarcado (Ex. Piloto Automático, Smart House, etc) - *pesquisar;
		- Java, C, C++;
		- C# dá pra transitar em C/C++;
			- Os mesmos são de alta remuneração;

- Para <mark style="background: #BBFABBA6;">Segurança</mark> é necessário:
	- Sistemas Operacionais;
	- Linux, Unix;
	- Linguagem C;
	- Cisco, é caro mas tem cursos básicos gratuitos;
		- Certificação Oracle também é válido;

- <mark style="background: #D2B3FFA6;">Firewall</mark>:
	- De forma análoga, é como se fosse um porteiro solicitando permissões para o usuário sobre várias ações, sendo boas ou não;
	- Controla os acessos/portas do dispositivos;

- <mark style="background: #D2B3FFA6;">Pingar</mark>:
	- Acessar vários IPs em sequencia para mascarar o acesso e destruir o caminho percorrido;

## Entidade /  Relacionamento

- <mark style="background: #ADCCFFA6;">Entidade</mark> (substantivo): Coisas/objetos;
- <mark style="background: #ADCCFFA6;">Relacionamento</mark> (verbo): Uma relação entre tabelas;
	- Sempre terá substantivo + verbo;
	- Entidade é representado por um quadrado;
	- Relacionamento é representado por um losango;

- <mark style="background: #ADCCFFA6;">Normalização</mark>:
	- Mais usados 1FN, 2FN, 3FN, 4FN:
		- <mark style="background: #FFF3A3A6;">1FN</mark>: Pede que definimos uma PK atômico, elimina grupos repetitivos e garante que cada valor em uma tabela seja atômico:
			- Campo atômico: quando não conseguimos fazer divisões, monovalorado;
			- Campo composto: conseguimos fazer uma sub divisões, dividir em vários campos atômicos;
			- Campo multivalorado: dependentes, múltiplos valores;
		- <mark style="background: #FFF3A3A6;">2FN</mark>: Elimina dependências parciais e garante que todos os atributos de uma tabela dependam totalmente da PK;
		- <mark style="background: #FFF3A3A6;">3FN</mark>: Elimina dependências transitivas, garantindo que os atributos não-chave não dependam uns dos outros;
		- <mark style="background: #FFF3A3A6;">4FN</mark> / <mark style="background: #FFF3A3A6;">5FN</mark> / <mark style="background: #FFF3A3A6;">6FN</mark>: Lidam com dependências multivaloradas e outras complexidades para alcançar maior eficiência e organização;

- Um exemplo é:
	Funcionário (substantivo) -> Tem (verbo) -> Telefone (substantivo)

## Tipos de Chaves
- <mark style="background: #FFF3A3A6;">Chave Candidata (Candidate Key)</mark>: grupo de chaves que estão propicias a serem chaves primarias, escolher a melhor chave que se adequa ao contexto (1 só);
	- Uma tabela pode ter várias chaves candidatas, mas apenas uma será escolhida como PK;
- <mark style="background: #FFF3A3A6;">Chave Composta (Compound Key)</mark>: Identificam registros únicos em um banco de dados. São combinações de duas ou mais colunas que tornam o 
- <mark style="background: #FFF3A3A6;">Chave Estrangeira (Foreign Key)</mark>: Para ligar uma tabela à outra, é necessário ter um campo em comum;

- Uma <mark style="background: #FFF3A3A6;">forma de lidar com redundâncias</mark> de dados, é criar uma nova tabela com as informações que podem ser duplicadas e "linkar" as tabelas principais que podem conter essas duplicatas;

- <mark style="background: #ADCCFFA6;">Cardinalidade</mark>: 1:N -> 1 para muitos; 1:1 -. 1 para 1;

- No <mark style="background: #FFF3A3A6;">Modelo Cascata</mark>, é necessário eliminar a tabela pai e assim vai eliminar todas as chaves que estão na tabela em questão e nas outras também;
