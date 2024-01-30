## ✨ Testes e Manutenção de software

- 🎈 Não temos como falar sobre software sem mencionar sobre como a qualidade de um produto de software é importante. Sempre temos que gerenciar ele a fim de obter um produto de alta qualidade.

## ✨ Estratégias de teste:

- 🎈 Um teste é considerado um comunto de atividades qu deve ser planejado e realizado de forma sistematica. O planejamento e a realização das atividades de teste planejadas fazem parte do que definimos por estratégia de teste de software;
- 🎈 Testes devem ser realizados desde o inicio, desde o levantamento de requisitos, até o final do produto. Se um problema for diagnosticado cedo, mais facil será de ser arrumado;
- 🎈 Nenhum produto é testado apenas ao final do seu desenvolvimento, por isso que para cada etapa do processo, é necessaria uma estrategia especifica de teste.

## ✨ Considerando uma estratégia de teste, ela deve:

- 🎈 Acomodar testes de baixo nivel e teste de alto nivel:
  - 💡 **Baixo nivel** significa que o teste é feito pelos programadores, engenheiros, algo bem especifico;
  - 💡 O teste de **alto nivel** é o mais proximo do usuario, do analista e etc.

- 🎈 Oferecer orientaçao ao profissional;
- 🎈 Oferecer um conjunto de marcos de referencia ao administrador do projeto e de cada fase do sistema;
- 🎈 Ser mensuravel. Existem testes estatisticos que sao utilizados para testar desempenho e confiabilidade do programa para checar como ele trabalha sob determinadas condiçoes operacionais;

- 🎈 A atividade de teste num produto de software nao é a mesma realizada pela equipe de desenvolvimento, ou seja, já possui alguns vicios que significa que é como se pensasse somente dentro da caixa, o melhor mesmo é pedir a alguém de fora da equipe de desenvolvimento para ter uma nova visão, apontar o teste, o que acontecerá e os tipos de falhas que foram encontradas.

## ✨ Validação e Verificação (V&V)

- 🎈 Nome dado aos processos de verificaçao e analise que asseguram que o software cumpra com as especificaçoes e atenda as necessidades dos clientes;
  - 💡 Validação: refere-se ao conjunto de atividades que garante que o software que foi construído seja adequado às exigencias do cliente. Basicamente responde a pergunta: Estamos fazendo o produto certo?
  - 💡 Verificação: refere-se ao conjunto de atividades que garante que o software seja construído da forma correta. Basicamente responde a pergunta: Estamos fazendo o produto corretamente?

🎈 O **objetivo principal do V&V** é estabelecer um vínculo de confiança entre o sistema de desenvolvimento e o projeto aprovado pelo usuário;

🎈 O nível de confiabilidade exigida depende, em grande escala, do propósito do cliente, das expectativas do usuário (que podem ou não ser a mesma pessoa que o cliente) e o atual ambiente/segmento do mercado no qual o software será utilizado;

🎈 Testar um software significa experimenta-lo, usando dados reais do usuário e examinar a saída esperada para confirmar anomalias.

- 🎈 Existem dois tipos de testes que podem ser utilizados:
  - 💡 ***Teste de validação***: significa se o produto cumpre com os requisitos já definidos;
  - 💡 ***Teste de defeito***: verificar se há defeitos, significa que iremos identificar os defeitos, erros, bugs do projeto.

## ✨ Inspeção de Software

- 🎈 Existem ***3 vantagens sobre inspeçao de teste***:
  - 💡 Durante os testes, erros podem mascarar (ocultar) outros erros. Uma vez que um erro é descoberto, voce nunca pode estar seguro se outras anomalias de saida são devidas a um novo erro ou são efeitos colaterais do erro já descoberto. Uma única seção de inspeção pode descobrir vários erros;
  - 💡 Versões incompletas de sistemas podem ser inspecionadas sem custos adicionais;
  - 💡 Assim como procurar defeitos de programa, uma inspeção pode considerar atributos de qualidade mais amplos como conformidade com padrões, portabilidade e facilidade de manutenção. Nesse momento, podem ser localizados, inclusive, algoritmos inapropriados e estilo de programação "pobre" que dificultaria o processo de manutenção.

- 🎈 Técnicas ou métodos de testes, devemos lembrar sempre que se tratando de testes:
  - 💡 Se erros graves forem encontrados com regularidade, então a qualidade e a confiabilidade do software são suspeitas;
  - 💡 Se erros facilmente corrigiveis forem encontrados, então a qualidade e a confiabilidade do software estao aceitáveis, ou os testes são inadequados para revelar erros graves desse particular software;
  - 💡 Se não forem encontrados erros, então a configuração de testes não foi suficientemente elaborada e os erros estão escondidos no software.

- 🎈 Em todo o processo, temos que ter em mente:
  - 💡 Defeito, num software, é uma deficiência mecânica ou algoritmica que, se ativada, pode levar a uma falha;
  - 💡 Falha, num software, é um vento notavel em que o sistema viola suas especificaçoes. Geralmente aparece durante a utilização do produto pelos usuários;
  - 💡 Erro, num software, é um item de informação ou estado de execução inconsistente. Deve ser corrigido durante a fase de manutenção.

- 🎈 Toda estratégia de teste é válida, desde que considere a verificação de testes de baixo nível (lógica) e testes de alto nível (usabilidade). Deve oferecer a orientação ao profissional, um conjunto de marcos de referência ao administrador, além de ter seu resultado mensurável;
- 🎈 ***Teste da caixa preta***: Também chamado de teste funcional, é uma abordagem na qual o teste é derivado da especificação de programas ou de componentes;
- 🎈 O teste procura descobrir erros nas seguintes categorias:
  - 💡 Funções incorretas ou ausentes;
  - 💡 Erros de interface;
  - 💡 Erros nas estruturas de dados ou no acesso a BD externos;
  - 💡 Erros de desempenho;
  - 💡 Erros de inicializaçao e termino.

- 🎈 ***Teste da caixa branca***: tem como objetivo determinar defeitos na estrutura interna do produto com tecnicas que eercitem possiveis caminhos e erros de execuçao;
  - 💡 Nessa técnica, são testados caminhos logicos atrasves do software, fornecendo casos de testes que podem a prova conutos especificos de condiçoes e/ou laços definidos no sistema;
  - 💡 É um teste mais especifico, verifica cada parte de algoritmo, hardware, vai até o nivel mais baixo nos testes.

- 🎈 Bateria de testes: as politicos de teste podem ser criadas seguindo as seguintes estrategias:
  - 💡 Teste de unidade;
  - 💡 Teste de integridade;
  - 💡 Teste de validação;
  - 💡 Teste de sistema.

## ✨ Manutenção de Software

- 🎈 Podemos dividir em 3 categorias:
    - 💡 Corretivas;
    - 💡 Adaptativas;
    - 💡 Perfectivas.
- 🎈 Modificar funções existentes;
- 🎈 Incluir novas funções;
- 🎈 Efetuar melhorias em geral;
- 🎈 Melhorar a manutenibilidade ou confiabilidade futura e fornecer uma base melhor para posterior aprimoramento.
---
