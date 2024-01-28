## ✨ Testes e Manutenção de software

- 🎈 Não temos como falar sobre software sem mencionar sobre como a qualidade de um produto de software é importante. Sempre temos que gerenciar ele a fim de obter um produto de alta qualidade.

## ✨ Estratégias de teste:

- 🎈 Um teste é considerado um comunto de atividades qu deve ser planejado e realizado de forma sistematica. O planejamento e a realização das atividades de teste planejadas fazem parte do que definimos por estratégia de teste de software;
- 🎈 Testes devem ser realizados desde o inicio, desde o levantamento de requisitos, até o final do produto. Se um problema for diagnosticado cedo, mais facil será de ser arrumado;
- 🎈 Nenhum produto é testado apenas ao final do seu desenvolvimento, por isso que para cada etapa do processo, é necessaria uma estrategia especifica de teste.

## ✨ Considerando uma estratégia de teste, ela deve:

- 🎈 Acomodar testes de baixo nivel e teste de alto nivel:
  - 💡 Baixo nivel significa que o teste é feito pelos programadores, engenheiros, algo bem especifico;
  - 💡 O teste de alto nivel é o mais proximo do usuario, do analista e etc.

- 🎈 Oferecer orientaçao ao profissional;
- 🎈 Oferecer um conjunto de marcos de referencia ao administrador do projeto e de cada fase do sistema;
- 🎈 Ser mensuravel. Existem testes estatisticos que sao utilizados para testar desempenho e confiabilidade do programa para checar como ele trabalha sob determinadas condiçoes operacionais;

- 🎈 A atividade de teste num produto de software nao é a mesma realizada pela equipe de desenvolvimento, ou seja, já possui alguns vicios que significa que é como se pensasse somente dentro da caixa, o melhor mesmo é pedir a alguém de fora da equipe de desenvolvimento para ter uma nova visão, apontar o teste, o que acontecerá e os tipos de falhas que foram encontradas.

## ✨ Validação e Verificação (V&V)

- 🎈 Nome dado aos processos de verificaçao e analise que asseguram que o software cumpra com as especificaçoes e atenda as necessidades dos clientes;
  - 💡 Validaçao: refere-se ao conjunto de atividades que garante que o software que foi construido seja rastravel as exigencias do cliente. Basicamente responde a pergunta: Estamos fazendo o produto certo?
  - 💡 Verificaçao: refere-se ao conunto de atividades que garante que o software seja construido da forma correta. Basicamente responde a pergunta: estamos fazendo o certo produto?

🎈 O objetivo principal do V&V é estabelecer um vinculo de confiança entre o sistema de desenvolvimento e o projeto aprovado pelo usuario.

🎈 O nivel de confiabilidade eigida depende, em grande escala, do proposito do cliente, das expectativas do usuario (que pode ou nao ser a mesma pessoa que o cliente) e o atual ambiente/segmento do mercado no qual o software será utilizado.

🎈 Testar um software significa experimenta-lo, usando dados reais do usuario e examinar a saida esperada para confirmar anomalias.

- 🎈 Existem dois tipos de testes que podem ser utilizados:
  - 💡 Teste de validação: significa se o produto cumpre com os requisitos já definidos;
  - 💡 Teste de defeito: verificar se há defeitos, significa que iremos identificar os defeitos, erros, bugs do projeto

## ✨ Inspeção de Software

- 🎈 Existem 3 vantagens sobre inspeçao de teste:
  - 💡 Durante os testes, erros podem mascarar(ocultar) outros erros. Uma vez que um erro é descoberto, voce nunca pode estar seguro se outras anomalias de saida sao devidas a um novo erro ou sao efeitos colaterais do erro já descoberto. Uma unica seção de inspeçao pode descobrir varios erros;
  - 💡 Versoes incompletas de sistemas podem ser inspecionadas sem custos adicionais;
  - 💡 Assim como procurar defeitos de programa, uma inspeçao pode considerar atributos de qualidade mais amplos como conformidade com padroes, portabildade e facilidade de manutençao. Nesse momento, podem ser localizados, inclusive, algoritmos inapropriados e estilo de programaçao "pobre" que dificultaria o processo de manutençao.

- 🎈 Tecnicas ou métodos de testes, devemos lembrar sempre que se tratando de testes:
  - 💡 Se erros gravse forem encontrados com regularidade, ntao a qualidade e a confiabilidade do software sao suspeitas;
  - 💡 Se erros facilmente corrigiveis forem encontrados, entao a qualidade e a confiabilidade do software estao aceitaveis, ou os testes sao inadquados para revelar erros graves desse particular software;
  - 💡 Se nao forem encontrados erros, entao a configuraçao de testes nao foi suficientemente elaborada e os erros estao escondidos no software.

- 🎈 Em todo o processo, temos que ter em mente:
  - 💡 Defeito, num software, é uma deficiencia mecanica ou algoritmica que, se ativada, pode levar a uma falha;
  - 💡 Falha, num software, é um vento notavel em que o sistema viola suas especificaçoes. Geralmente aparece durante a utilizaçao do produto pelos usuarios;
  - 💡 Erro, num software, é um item de informaçao ou estado de execuçao inconsistente. Deve ser corrigido durante a fase de manutençao.

- 🎈 Toda estrategia de teste é valida, desde que considere a verificaçao de testes de baixo nivel(logica) e testes de alto nivel(usabilidade). Deve oferecer a orientaçao ao profissional, um conjunto de marcos de referencia ao administrador, além de ter seu resultado mensuravel;
- 🎈 Teste da caixa preta: Também chamado de teste funcional, é uma abordagem na qual o teste é derivado da especificaçao de programas ou de componentes;
- 🎈 O teste procura descobrir erros nas seguintes categorias:
  - 💡 Funçoes incorretas ou ausentes
  - 💡 Erros de interface
  - 💡 Erros nas estruturas de dados ou no acesso a BD externos
  - 💡 Erros de desempenho
  - 💡 Erros de inicializaçao e termino.

- 🎈 Teste da caixa branca: tem como objetivo determinar defeitos na estrutura interna do produto com tecnicas que eercitem possiveis caminhos e erros de execuçao;
- 🎈 Nessa tecnica, sao testados caminhos logicos atrasves do software, fornecendo casos de testes que podem a prova conutos especificos de condiçoes e/ou laços definidos no sistema;
- 🎈 É um teste mais especifico, verifica cada parte de algoritmo, hardware, vai até o nivel mais baixo nos testes.

- 🎈 Bateria de testes: as politicos de teste podem ser criadas seguindo as seguintes estrategias:
  - 💡 Teste de unidade
  - 💡 Teste de integridade
  - 💡 Teste de validaçao
  - 💡 Teste de sistema

## ✨ Manutenção de Software

- 🎈 Podemos dividir em 3 categorias:
    - 💡 Corretivas;
    - 💡 Adaptativas;
    - 💡 Perfectivas
- 🎈 Modificar funçoes existentes
- 🎈 Incluir novas funçoes
- 🎈 Efetuar melhorias em geral
- 🎈 Melhorar a manutenibilidade ou confiabilidade futura e fornecer uma base melhor para posterior aprimoramento.
---
