## ✨ Power Query: O primeiro Power
- 🎀 Power Query serve para conectar, transformar e preparar os dados para o Power BI fazer as análises;
- 🎀 Importar sempre a tabela e não guias de planilhas, pois vem apenas os dados brutos. É melhor para visualização;
- 🎀 A opção *Carregar* leva direto para o Power BI, sem tratamento de dados;
- 🎀 A opção *Transformar Dados* leva direto para o Power Query para tratarmos os dados.
---
## ✨ O que é o Power Query
- 🎀 Power Query é um mecanismo de transformação de dados e preparação de dados.
- 🎀 Ele vem com uma interface gráfica para obter dados de fontes e um Editor do Power Query para aplicar as transformações. Como o mecanismo está disponível em muitos produtos e serviços, o destino em que os dados serão armazenados depende de onde Power Query foi usado.
- 🎀 Usando o Power Query, você pode executar o processamento <mark style="background: #BBFABBA6;">ETL</mark>:
	- ETL significa *Extract, Transform, Load* ==> Extrair, Transformar e Carregar.
---
## ✨ Onde encontramos o Power Query / Opções de armazenamento
- 🎀 Microsoft Azure Data Lake Storage;
- 🎀 Microsoft Dataverse;
- 🎀 Microsoft Excel;
- 🎀 Microsoft Power BI.
---
## ✨ Como o Power Query ajuda?
- 🎀 Power Query habilita a conectividade com uma ampla gama de fontes de dados, incluindo dados de todos os tamanhos e formas.
- 🎀 Junta os recursos e dados de todas as fontes em um único lugar.
- 🎀 Consistência de experiência e paridade de recursos de consulta em todas as fontes de dados;
- 🎀 Experiência altamente interativa e intuitiva para criar consultar de forma rápida e interativa em qualquer fonte de dados, de qualquer tamanho;
- 🎀 Ao usar o Power Query para acessar e transformar dados, definimos um processo repetível (consulta) que pode ser atualizado facilmente no futuro para obter dados atualizados. Caso precisemos modificar o processo ou a consulta para considerar as alterações de esquema ou dados subjacentes, podemos usar a mesma experiência interativa e intuitiva usada quando definimos inicialmente a consulta.
- 🎀 O Power Query oferece a capacidade de trabalhar em um subconjunto de todo o conjunto de dados para definir as transformações de dados necessárias, permitindo que filtremos facilmente e transforme seus dados em um tamanho gerenciável. 
- 🎀 As consultar no Power Query podem ser atualizadas manualmente ou aproveitando os recursos de atualização agendadas em produtos específicos (como Power BI) ou até mesmo programaticamente (usando o modelo de objeto Excel).
---
## ✨ Experiências Power Query
- 🎀 A experiência do usuário PQ é fornecida por meio da interface do usuário Editor do Power Query.
- 🎀 O objetivo dessa interface é ajudar a aplicar as transformações necessárias simplesmente interagindo com um conjunto amigável de faixas de opções, menus, botões e outros componentes interativos.
- 🎀 O Editor do Power Query é a experiência primária de preparação de dados, em que você pode se conectar a uma ampla gama de fontes de dados e aplicar centenas de transformações de dados diferentes visualizando dados e selecionando transformações da interface do usuário.
- 🎀 Esses recursos de transformação de dados são comuns em todas as fontes de dados, quaisquer que sejam as limitações da fonte de dados subjacentes.
- 🎀 Quando você crua uma nova etapa de transformação interagindo com os componentes da interface Power Query, o PQ cria automaticamente o código M necessário para fazer a transformação para que não precise escrever nenhum código.
---
## ✨ Fluxos de dados
- 🎀 O Power Query podem ser usados em muitos produtos, como Power BI e Excel. No entanto, o uso de Power Query dentro de um produto limita seu uso apenas a esse produto específico.
- 🎀 Os *fluxos de dados* são uma versão de serviço independente do produto da experiência PQ que é executada na nuvem.
- 🎀 Usando fluxos de dados, podemos obter dados e transformar dados da mesma maneira, mas em vez de enviar a saída para Power BI ou Excel, podemos armazenar a saída em outras opções de armazenamento, como Dataverse ou Azure Data Lake Storage.
---
## ✨ Utilizando o Power Query
- 🎀 Se quisermos voltar para o Power Query após ser fechado, dentro do Power BI iremos na opção <mark style="background: #FFB8EBA6;">Transformar Dados</mark>.
- 🎀 Para dividir 2 informações que estão dividindo em 1 coluna só, é necessário clicar com o botão direito em cima do <mark style="background: #FFB8EBA6;">nome da coluna</mark> e logo em seguida <mark style="background: #FFB8EBA6;">Dividir Coluna</mark> e escolher a opção adequada.
- 🎀 Se um dado está alinhado para a esquerda => é um formato de texto.
- 🎀 Se um dado está alinhado para a direita => é um formato de número.
- 🎀 Extrair no Power Query => Manter as informações.
- 🎀 É necessário utilizar o CORTAR no Power Query para "nivelar" as informações, pois palavras com espaços no final é dado como outra informação.
	- 💭Por exemplo => Minas Gerais( ) é diferente de Minas Gerais() -> com e sem espaço.
---
