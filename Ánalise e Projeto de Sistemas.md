## ✨ Formatos de Arquivo para Armazenamento de Dados:

- 📌 Há 2 tipos básicos de formatos de armazenamento de dados:

	- 🌸 ***Arquivos***:
		- Um *arquivo de dados* contém uma lista eletrônica de informações, que é formatada para uma determinada transação, e essas informações são modificadas e manipuladas por programas escritos para essas finalidades.
			- 🎈 ***mestre***: Armazenam informações essenciais para o negócio, em específico para a aplicação, como informações de pedidos ou informações sobre endereços de correspondência dos clientes. Normalmente são mantidos por longos períodos, e novos registros são adicionados no final do arquivo quando novos pedidos ou clientes forem detectados pelo sistema.

			- 🎈 ***de pesquisa (look-up)***: Contêm valores estáticos usados para validar campos nos arquivos centrais.

			- 🎈 ***de transação***: armazenam temporariamente informações que serão usadas para atualizar um arquivo mestre. Esse arquivo pode ser destruído depois que as modificações terem sido efetivadas ou ser salvo no caso das transações precisarem ser acessadas no futuro.
  
			- 🎈 ***de auditoria***: registra as imagens de dados "antes" e "depois", quando forem alterados, para que possa ser executada uma auditoria no caso de a integridade dos dados ser questionada.

			- 🎈 ***de histórico***: armazena transações passadas (por exemplo, clientes antigos, pedidos atendidos), não mais necessárias ao sistema. É um arquivo armazenado off-line, porém ainda pode ser acessado quando necessário.
 
	- 🌸 ***Banco de dados***: Um banco de dados é um conjunto de agrupamentos de informações relacionadas entre si de alguma maneira, e um sistema de gerenciamento de banco de dados (SGBD) é o software que cria e manipula esses bancos de dados.

		- Há 4 tipos de bancos de dados:
			- 🎈 ***Banco de dados legado***: Refere-se aos bancos baseados em tecnologia antiga, algumas vezes obsoleta, e raramente usada para desenvolver novas aplicações. Exemplos de bancos legados:
				- 💟***Banco de dados hierárquicos***: Usam hierarquias ou árvores invertidas para representar os relacionamentos. São conhecidos por sua capacidade de pesquisa rápida e foram usados nos primeiros sistemas da indústria aeronáutica.
				- 💟***Bancos de dados em rede***: São conjuntos de registros relacionados entre si por meio de ponteiros. Basicamente, um registro é um membro em um ou mais conjuntos, e os ponteiros ligam entre si os membros de um conjunto. Desenvolvido por causa da desvantagem do hierárquico, pois o hierárquico não pode representar de forma eficiente os relacionamentos M:M.
      
			- 🎈 ***Banco de dados relacionais***: Baseado em um grupo de tabelas, cada uma representando uma chave primária, um campo, cujo valor é diferente para cada linha da tabela. É o tipo mais popular de banco de dados para o desenvolvimento de aplicações. As tabelas são relacionadas entre si por meio da chave primária de uma tabela como uma chave estrangeira na tabela relacionada. 
				- Embora seja menos "eficiente em termos de máquina" que os bancos de dados legados, é mais fácil trabalhar com ele sob uma perspectiva de desenvolvimento.
 
			- 🎈 ***Bancos de dados de objetos***: Ou chamado de orientados a objetos, a combinação de dados e processos é representada pelas classes de objetos, que são categorias principais dos objetos do sistema, e uma classe pode conter diversas subclasses ou casos especiais daquela classe. Os relacionamentos entre as classes de objetos são mostrados encapsulando uma classe de objeto dentro da outra, usados principalmente em aplicação de multimídia (gráficos, vídeo e som).

			- 🎈 ***Banco de dados multidimensional***:  É um tipo de banco de dados relacional que tornou-se popular com o crescimento da data warehousing e é amplamente usado na mesma. Data warehousing é a prática de acessar os dados de sistemas de processamento de transações de uma empresa, transformá-los e armazená-los para serem usados em um data warehouse, ou seja, um grande banco de dados. Ele armazena informações calculadas previamente na interseção de dimensões para dar suporte a aplicações que exijam que os dados sejam analisados.
