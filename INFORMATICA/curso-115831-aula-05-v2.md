

Livro Eletrônico
Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti 06315057411 - EVA CELESTE DE SOUZA 







1
84
Sumário
1 – Segurança da Informação ....................................................................................................... 4 1.1 – Conceitos Básicos ................................................................................................................ 4 1.2 – Controles de Segurança ...................................................................................................... 8 1.3 – Terminologia ...................................................................................................................... 10 1.4 – Princípios Fundamentais .................................................................................................... 13 1.4.1 – Confidencialidade ....................................................................................................... 13 1.4.2 – Integridade .................................................................................................................. 14 1.4.3 – Disponibilidade ........................................................................................................... 15 1.5 – Princípios Adicionais .......................................................................................................... 16 1.5.1 – Autenticidade .............................................................................................................. 16 1.5.2 – Irretratabilidade ........................................................................................................... 18 2 – Criptologia ........................................................................................................................... 19 2.1 – Conceitos Básicos .............................................................................................................. 19 2.2 – Esteganografia ................................................................................................................... 20 2.3 – Criptografia e Criptoanálise ............................................................................................... 22 2.3.1 – Conceitos Básicos........................................................................................................ 22 2.3.2 – Técnicas de Criptografia.............................................................................................. 24 3 – Autenticidade ....................................................................................................................... 32 3.1 – Conceitos Básicos .............................................................................................................. 32 3.1.1 – Método de Autenticação: O que você sabe? .............................................................. 32 3.1.2 – Método de Autenticação: O que você é? ................................................................... 33 3.1.3 – Método de Autenticação: O que você tem? ............................................................... 34 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








2
84



3.2 – Autenticação Forte ............................................................................................................ 36 3.3 – Assinatura Digital ............................................................................................................... 37 3.3.1 – Conceitos Básicos........................................................................................................ 37 3.4 – Certificado Digital .............................................................................................................. 44 3.4.1 – Conceitos Básicos........................................................................................................ 44 3.4.2 – Infraestrutura de Chave Pública (ICP-Brasil)................................................................. 49 3.4.3 – Tipos de Certificado .................................................................................................... 53 Resumo ...................................................................................................................................... 55 Mapa Mental .............................................................................................................................. 58 Questões Comentadas - FCC .................................................................................................... 60 Lista de Questões - FCC ............................................................................................................ 69 Gabarito - FCC ........................................................................................................................... 75 Questões Comentadas – DIVERSAS BANCAS ........................................................................... 76 Lista de Questões – DIVERSAS BANCAS ................................................................................... 81 Gabarito – DIVERSAS BANCAS ................................................................................................. 84 












Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








3
84



APRESENTAÇÃO DA AULA 
Pessoal, o tema da nossa aula é: Segurança da Informação. Nós vamos ver os conceitos básicos, terminologias  e  princípios  fundamentais.  Depois  vamos  entender  mais  sobre  criptografia, assinatura digital e certificação digital. Esses são assuntos que estão no dia-a-dia de vocês mesmo que vocês não percebam. Quem  aí  não  viu as  tretas  que  rolaram  com  hackeamento  de  celulares recentemente na política brasileira? Pois é, ninguém está imune...

PROFESSOR DIEGO CARVALHO - www.instagram.com/professordiegocarvalho 
Galera, todos os tópicos da aula possuem  Faixas de Incidência, que  indicam se o assunto cai muito ou pouco em prova. Diego, se cai pouco para que colocar em aula? Cair pouco não significa que não cairá justamente na sua prova! A ideia aqui é: se você está com pouco tempo e precisa ver somente aquilo que cai mais, você pode filtrar pelas incidências média, alta e altíssima; se você tem tempo sobrando e quer ver tudo, vejam também as incidências baixas e baixíssimas. Fechado?

INCIDÊNCIA EM PROVA: baixíssima 
INCIDÊNCIA EM PROVA: baixa 
INCIDÊNCIA EM PROVA: média 
INCIDÊNCIA EM PROVA: ALTA 
INCIDÊNCIA EM PROVA: Altíssima 





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








4
84



1 – SEGURANÇA DA INFORMAÇÃO 1.1 – CONCEITOS BÁSICOS INCIDÊNCIA EM PROVA: baixa 

Galera, uma rotina  comum na vida de várias pessoas é: acordar, tomar um banho, escovar os dentes, comer alguma coisa, sair de casa, entrar no carro, chegar na firma, guardar suas coisas na gaveta e finalmente trabalhar. No fim do dia, você abre sua gaveta, pega as suas coisas e vai embora para casa. Não é mais ou menos assim? No entanto, há alguns detalhes que não falamos sobre essa rotina!

Ao sair, vocês por acaso deixam a porta de casa destrancada? Vocês deixam uma fresta na janela?
Vocês não usam alarme no carro? Vocês deixam seu cofre aberto? Bem, eu espero que vocês tenham respondido um sonoro não para todas essas perguntas! Por favor :) E por que vocês trancam a porta, fecham  as  janelas,  utilizam  alarmes  no  carro  e  trancam  seus  cofres  com  chave? Porque  vocês possuem ativos de valor que desejam proteger!

Ninguém quer ter casa, carro ou quaisquer itens pessoais furtados. Por conta disso, vocês tomam várias precauções: colocam uma fechadura melhor, utilizam alarme automotivo, entre outros.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








5
84




Agora, vocês já notaram que – quando se trata de informação – nós somos bem mais negligentes e muito menos cuidadosos? Vejam a notícia acima: ela afirma que, em 2017, as senhas mais comuns do planeta ainda eram “password” e “12345”. Pois é, as pessoas não têm a mesma precaução na hora de proteger suas informações quanto têm na hora de proteger seus objetos. Assim fica fácil até para um hacker relativamente habilidoso...

LISTA DE SENHAS MAIS UTILIZADAS DE 2017 12345 123456789 admin starwars hello password letmein welcome 123123 freedom 12345678 1234567 monkey dragon whatever qwerty football Login passw0rd qazwsx 123456 iloveyou abc123 master trustno1 
Claro  que  nem  toda  informação  é  relevante  ao  ponto de  necessitar  de  várias  barreiras  de segurança. Você eventualmente não precisa colocar uma senha no computador de casa ou pagar caro por um antivírus poderoso. Analogamente, se você mora em um bairro tranquilo da Suíça, dificilmente necessitará de alarme no carro ou trancar a porta de casa. Por outro lado, se você mora em um bairro perigoso de Honduras, é recomendável possuir várias barreiras de segurança.



De  toda  forma,  nós  estamos  na  era  digital!  Como  a  imagem  acima  apresenta,  a  humanidade armazena e acessa trilhões de informações todos os dias por meio de diversos meios diferentes, como computadores, celulares, conversas ou documentos. Vocês sabiam que o conteúdo digital produzido no mundo dobra em quantidade a  cada dois anos? Em 2020, devemos ter mais de 44 trilhões de gigabytes de informações digitais.

Por conta disso, as organizações gastam grande parte de seus orçamentos em equipamentos capazes  de  coletar,  processar,  analisar  e  disseminar  dados  de  forma  segura . Hoje em dia, a
informação  é  a  principal  fonte  de  renda  dos  negócios,  logo  precisa  estar  adequadamente assegurada. Galera, acreditem em mim: informação é dinheiro! Isso vale tanto para um banco quanto para uma padaria da esquina...

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








6
84





Vejam  as  notícias  acima:  informações  vazam  basicamente  todos  os  dias  tanto  de  empresas (Facebook), quanto de pessoas (Kendall Jenner), quanto de órgãos públicos (CIA).
Logo, não são
só  as  instituições  que  devem  ter  cuidado,  todos  nós  devemos  ser  mais  diligentes  com  as informações que possuímos. Bacana? Dito isso, vamos ver na tabela seguinte algumas definições de Segurança da Informação:

DEFINIÇÕES DE SEGURANÇA DA INFORMAÇÃO Proteção  de  informações  e  de  sistemas  de  informações  contra  acesso,  uso,  divulgação,  interrupção, modificação ou destruição não autorizados.
Salvaguarda  de  dados  organizacionais  contra  acesso não  autorizado  ou  modificação  para  assegurar  sua disponibilidade, confidencialidade e integridade.
Conjunto de estratégias para gerenciar processos, ferramentas e políticas necessárias para prevenir, detectar, documentar e combater ameaças às informações organizacionais.

O Decreto Nº 9.637 da Presidência da República, que institui a Política Nacional de Segurança da Informação (PNSI) nos órgãos e entidades da Administração Pública Federal busca:

“Assegurar a disponibilidade, integridade, a confidencialidade e a autenticidade da informação a nível nacional.
Para os fins do disposto neste Decreto, a segurança da informação abrange: I – a segurança cibernética; II – a defesa cibernética; III – a segurança física e a proteção de dados organizacionais; e IV – as ações destinadas a assegurar a disponibilidade, a integridade, a confidencialidade e a autenticidade da informação”.

Já a literatura acadêmica afirma que existe uma trindade sagrada da  segurança  da  informação.  São  três  princípios  (também chamados  de  propriedades  ou  atributos): Confidencialidade, Integridade e Disponibilidade – conhecidos pela sigla CID.

Se um ou mais desses princípios forem desrespeitados em algum momento,  significa  que  houve  um  incidente  de  segurança  da informação (apesar de a figura ao lado apresentar uma pirâmide numerada, não existe hierarquia entre os princípios).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








7
84



Vamos ver esses princípios em detalhes mais à frente, mas basicamente a confidencialidade é o princípio de que a informação não esteja disponível ou seja revelada a indivíduos, entidades ou processos não autorizados; a integridade é o princípio de salvaguarda da exatidão e completeza de ativos de informação; e a disponibilidade é o princípio da capacidade de estar acessível e utilizável quando demandada por uma entidade autorizada.

(UERN   –   2010   –   Letra   B) A  segurança  da  informação  é  obtida  por  meio  da implementação de um conjunto extenso de controles, que devem ser correlacionados para  garantir  a  preservação  da  confidencialidade,  integridade  e  disponibilidade  da informação.
_______________________ Comentários: conforme vimos em aula, questão impecável (Correto).

(Polícia  Federal  –  2013) Segurança da informação é caracterizada, basicamente, pelo fornecimento  de  três  serviços  de  segurança:  a  preservação  do  sigilo  ou  da confidencialidade das informações, a garantia da integridade dos dados e a manutenção da disponibilidade.
_______________________ Comentários: conforme vimos em aula, questão exata (Correto).























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








8
84



1.2 – CONTROLES DE SEGURANÇA INCIDÊNCIA EM PROVA: baixa 
Galera, selecionar e implementar controles de segurança adequados inicialmente pode ajudar uma organização a reduzir seus riscos a níveis aceitáveis. A seleção de possíveis controles deve se basear na avaliação de riscos. Os controles podem variar em natureza, mas – fundamentalmente – são formas de proteger a confidencialidade, integridade ou disponibilidade de informações.
Em geral,
eles são divididos em dois tipos:

 Controles Físicos: são barreiras que impedem ou limitam o acesso físico direto às informações ou  à  infraestrutura  que  contém  as  informações.  Ex: portas,  trancas,  paredes,  blindagem, vigilantes, geradores, sistemas de câmeras, alarmes, catracas, cadeados, salas-cofre, alarmes de incêndio, crachás de identificação, entre outros.

 Controles  Lógicos: também chamados de controles técnicos, são barreiras que impedem ou limitam o acesso à informação por meio do monitoramento e controle de acesso a informações e a sistemas de computação. Ex: senhas, firewalls, listas de controle de acesso, criptografia, biometria, IDS, IPS, entre outros.

É importante destacar que o tipo de controle se dá em razão do recurso e, não, do método de autenticação. Como assim, Diego? Se o recurso a ser acessado for físico (Ex: entrar em uma casa), trata-se de um controle físico; se o recurso a ser acessado for lógico (Ex: logar em um sistema), trata-se de um controle lógico.
Dessa forma, alguns dos exemplos apresentados acima podem variar entre controle físico ou lógico dependendo do recurso acessado.

(TRT/10 – 2013) Os mecanismos utilizados para a segurança da informação consistem em controles físicos e controles lógicos. Os controles físicos constituem barreiras de hardware, enquanto os lógicos são implementados por meio de softwares.
_______________________ Comentários: o controle de acesso físico não se limita ao hardware e o controle de acesso lógico não se limite ao software (Errado).

(TJDFT   –   2015) Na  segurança  da  informação,  controles  físicos  são  soluções implementadas nos sistemas operacionais em uso nos computadores para garantir, além da disponibilidade das informações, a integridade e a confidencialidade destas.
_______________________ Comentários: controles físicos são barreiras que limitam o contato ou acesso direto à informação ou à infraestrutura suporta essa informação (Errado).

(IF/TO – 2016) O suporte para as recomendações de segurança da informação pode ser encontrado em controles físicos e controles lógicos. Existem mecanismos de segurança que apoiam os controles físicos assim como os controles lógicos. Das alternativas abaixo qual não é um mecanismo de segurança que apoia os controles lógicos?

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








9
84



a) Assinatura digital. Um conjunto de dados criptografados, associados a um documento do qual são função, garantindo a integridade do documento associado, mas não a sua confidencialidade.

b) Mecanismos de controle de acesso. Palavras-chave, sistemas biométricos, firewalls, cartões inteligentes.

c) Sistema de controle de acesso eletrônico ao centro de processamento de dados, com senha de acesso ou identificações biométricas como digitais e íris.

d) Mecanismos de certificação. Atesta a validade de um documento.

e) Mecanismos de criptografia. Permitem a transformação reversível da informação de forma a torná-la ininteligível a terceiros.
_______________________ Comentários: (a) Errado, Assinatura Digital é um controle lógico; (b) Errado, mecanismos de controle de acesso são controles lógicos; (c) Correto. Como a questão fala que é um sistema de controle de acesso eletrônico ao Centro de Processamento de Dados (CPD) da organização, trata-se de um controle físico. Lembrando que CPD é o local onde estão concentrados os sistemas computacionais de uma organização; (d) Errado, mecanismos de certificação é um controle lógico; (e) Errado, mecanismos de criptografia são controles lógicos (Letra C).

























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








10
84



1.3 – TERMINOLOGIA
INCIDÊNCIA EM PROVA: baixíssima Sabe-se que existe o risco de que um determinado agente se aproveite de vulnerabilidades para – por  meio  de ataques  ou  de ameaças  –  gerar  um incidente  que  quebre  a  confidencialidade, integridade  ou  disponibilidade  de  um ativo  de informação  gerando  graves impactos organizacionais. Professor,  não  entendi  nada! Calma,  galera!  Vocês  só  não  entenderam porque vocês ainda não sabem o significado da maioria dessas palavras.

Na Segurança da Informação, utiliza-se um jargão muito específico. Caso – no decorrer da aula – vocês tenham alguma dúvida, é só retornar aqui e descobrir o significado. Vejamos 
TERMINOLOGIA DESCRIÇÃO ATIVO
Qualquer coisa que tenha valor para instituição, tais como: informações, pessoas, serviços, software, hardware, documentos físicos, entre outros.

INFORMAÇÃO
Ativo  que,  como  qualquer  outro  ativo  importante  para  os  negócios,  tem  valor  para  a organização e, por isso, deve ser adequadamente protegido.

AGENTE
Fonte  produtora  de  um  evento  que  pode  ter  um  efeito  adverso  sobre  um  ativo  de informação, como um funcionário, meio ambiente, hacker, etc.

VULNERABILIDADE
Fragilidades presentes ou associadas a ativos que, quando exploradas por ameaças, levam à ocorrência de incidentes de segurança.

AMEAÇA
A ameaça é um agente externo que, se aproveitando das vulnerabilidades, poderá quebrar a confidencialidade, integridade ou disponibilidade da informação, causando um desastre ou perda significativa em um ambiente, sistema ou ativo de informação.
ATAQUE
Evento decorrente da exploração de uma vulnerabilidade por uma ameaça com o intuito de obter,  alterar,  destruir,  remover,  implantar  ou  revelar  informações  sem  autorização  de acesso.
EVENTO
Ocorrência identificada de um sistema, serviço ou rede, que indica uma possível violação da política de segurança da informação ou falha de controles, ou uma situação previamente desconhecida, que possa ser relevante para a Segurança da Informação.
INCIDENTE
Fato  decorrente  de  um  ataque  bem-sucedido,  com  consequências  negativas,  uma ocorrência indicando uma violação, uma falha ou situação desconhecida, algo que possa ser relevante para a segurança da informação.
IMPACTO
Abrangência  dos  danos  causados  por  um  incidente  de segurança  sobre  um  ou  mais processos de negócio.

RISCO
Probabilidade potencial da concretização de um evento que possa causar danos a um ou mais ativos da organização.


Eu percebo que é muito comum que os alunos tenham dúvidas sobre a diferença entre ameaça e  risco. Vamos dirimi-las agora! A ameaça trata de um dano potencial, isto é, caso ocorra um Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








11
84



incidente, poderá haver dano ou não. Já o risco trata de um dano real, isto é, caso ocorra um incidente, necessariamente haverá perdas ou danos. Em geral, o risco trata da concretização de ameaças. Entendido?

Agora vamos fazer uma analogia – grosso modo – para entender melhor como essa terminologia se aplicaria à vida cotidiana. Imagine que você passe no sonhado concurso público e compre um carro –
esse carro seria um ativo. Como o carro ainda está com o cheirinho de novo, você decide estacioná-lo mais longe a fim de evitar a ocorrência de qualquer acontecimento imprevisível – isso seria um evento.

Se esse acontecimento imprevisível fosse negativo, como alguém abrir a porta do carro ao lado com força e arranhar o seu carro, isso seria incidente. No entanto, esse lugar mais longe é mais perigoso e  frequentemente  carros  são  furtados  por  diversos  assaltantes  – esses  assaltantes  seriam  os agentes. Como o carro foi comprado recentemente, você ainda não teve tempo de instalar um alarme – isso seria uma vulnerabilidade.

Dessa forma, você sabe que há chances de o carro ser furtado – isso seria um ameaça. Certo dia,
quando você se aproxima do carro para voltar para casa, um meliante anuncia um assalto – isso
seria  um risco, visto que ele ainda não o assaltou efetivamente. Ele, então, rouba a sua chave e carteira, entra no veículo e sai cantando pneu – isso seria um ataque. O agressor some com o carro, leva para um desmanche e você fica sem o carro para todo sempre – isso seria um impacto.



(AGU – 2010) A informação é um ativo que, como qualquer outro ativo importante para os  negócios,  tem  valor  para  a  organização  e,  por  isso,  deve  ser  adequadamente protegida.
_______________________ Comentários: Questão perfeita! Essa assertiva foi retirada de forma literal da Norma ISO/IEC 17799, que é uma norma de Gestão de Segurança da Informação (Correto).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








12
84



(SEFAZ/RS   –   2014) Considerando  os  aspectos  da  segurança  da  informação,  a possibilidade de uma determinada ameaça explorar vulnerabilidades de um ativo ou de um conjunto de ativos, prejudicando a organização, é chamada de:

a) Eventos de segurança da informação.
b) Incidentes de segurança da informação.
c) Riscos de segurança da informação.
d) Impacto organizacional.
e) Criticidade de ativo.
_______________________ Comentários: trata-se de riscos de segurança da informação (Letra C).

(PEFOCE  –  2012) As  ameaças  são  fatores  externos  que  podem  gerar  incidente  de segurança da informação por intermédio da exploração das vulnerabilidades dos ativos de informação.
_______________________ Comentários: ameaça é um agente externo que, se aproveitando das vulnerabilidades, poderá quebrar a confidencialidade, integridade ou disponibilidade da informação, causando um desastre ou perda significativa em um ambiente, sistema ou ativo de informação (Correto).

(Prefeitura de Bom Jesus/PI – 2008) Com relação à segurança da informação, o evento decorrente da exploração de uma vulnerabilidade por uma ameaça é um:

a) impacto.
b) risco.
c) antispyware.
d) repúdio.
e) ataque.
_______________________ Comentários: um ataque é um evento decorrente da exploração de uma vulnerabilidade por uma ameaça com o intuito de obter, alterar, destruir, remover, implantar ou revelar informações sem autorização de acesso (Letra E).












Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








13
84



1.4 – PRINCÍPIOS FUNDAMENTAIS 
1.4.1 – Confidencialidade INCIDÊNCIA EM PROVA: Altíssima 
Confidencialidade  é  a capacidade  de  um  sistema  de  não  permitir  que  informações  estejam disponíveis  ou  sejam  reveladas  a  entidades  não  autorizadas –  incluindo  usuários,  máquinas, sistemas ou processos. Seria algo similar à privacidade, em que pessoas autorizadas podem acessar e visualizar uma informação privada, mas pessoas não autorizadas não podem. Simples, não? É algo bem do nosso dia-a-dia...

Por exemplo: caso eu escreva uma carta e a envie dentro de um envelope para um destinatário, o carteiro pode ter acesso a minha carta, mas em tese não poderá lê-la. Caso ele rasgue o selo, aí sim ele terá acesso direto às informações lá escritas.
No entanto, nesse contexto, ele terá quebrado o  princípio  da  confidencialidade  e  uma  ou  mais  pessoas  não  autorizadas  poderão  visualizar meus dados privados contidos dentro da carta.

(IFB  –  2012) Com  relação  à  segurança  da  informação,  assinale  a  alternativa  que apresenta  o  princípio  segundo  o  qual  a  informação  só  será  acessível  a  pessoas autorizadas e será, também, protegida contra a revelação não permitida.

a) Confidencialidade b) Irretratabilidade c) Disponibilidade
d) Esteganografia
e) Integridade
_______________________ Comentários: conforme vimos em aula, a confidencialidade é a capacidade de um sistema de não permitir que informações estejam disponíveis ou sejam reveladas a entidades não autorizadas (Letra A).

(TCE/RS – 2014) José utilizou uma ferramenta para criptografar uma informação a ser transmitida para Maria, com o objetivo de proteger a informação contra acesso não autorizado. O requisito básico de segurança da informação assegurado pela criptografia é a:

a) irretratabilidade.
b) autenticidade.
c) confidencialidade.
d) disponibilidade.
e) confiabilidade.
_______________________ Comentários: conforme vimos em aula, trata-se da confidencialidade (Letra C).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








14
84



1.4.2 – Integridade
INCIDÊNCIA EM PROVA: Altíssima 
Integridade é a capacidade de garantir que a informação manipulada está correta, fidedigna e que não foi corrompida. Esse princípio geralmente trata da salvaguarda da exatidão e completeza da informação, com o intuito de aferir que a informação não tenha sido alterada sem autorização durante seu percurso, de sua origem ao seu destino, mantendo todas as características originais estabelecidas pelo proprietário da informação.

Em outras palavras, esse princípio sinaliza a conformidade dos dados armazenados com relação às   inserções,   alterações   e   processamentos   autorizados   efetuados .  Sinaliza,  ainda,  a conformidade dos dados transmitidos pelo emissor com os recebidos pelo destinatário, garantindo a não violação dos dados com intuito de alteração, gravação ou exclusão, seja ela acidental ou proposital.

No exemplo anterior, se a carta que eu enviei chegou ao destinatário exatamente da forma que eu a  enviei,  ou  seja, lacrada,  correta,  fidedigna,  precisa,  original,  impecável,  sem  nenhuma manipulação, então mantivemos o princípio da integridade da informação. É por essa razão que empresas  de  e-commerce  pedem  que  os  clientes  não  aceitem  produtos  que  estejam  com  a embalagem danificada ou sem lacre – porque ela pode ter sido manipulada por terceiros.

Percebam também que confidencialidade e integridade são princípios independentes, isto é, a quebra de um princípio não implica a quebra do outro. Por exemplo: o carteiro pode interceptar minha  carta,  colocá-la  contra  uma  luz  forte  e  eventualmente  conseguir  visualizar  a  minha mensagem sem a minha autorização – quebrando o princípio da confidencialidade. No entanto, ele não terá quebrado o princípio da integridade, visto que minha carta será entregue inalterada.

(TJ/SP  –  2014) Assinale a alternativa que apresenta corretamente a característica do requisito básico de segurança, conhecido como integridade.

a) Verificar se uma entidade é realmente quem ela diz ser.
b) Determinar as ações que uma entidade pode executar.
c) Proteger uma informação contra acesso não autorizado.
d) Proteger a informação contra alteração não autorizada.
_______________________ Comentários: conforme vimos em aula, trata-se de proteger a informação contra alteração não autorizada (Letra D).






Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








15
84



1.4.3 – Disponibilidade INCIDÊNCIA EM PROVA: Altíssima 
Disponibilidade é a propriedade  de uma informação estar acessível e utilizável sob demanda por  uma  entidade  autorizada. De certa forma, ela garante que usuários autorizados obtenham acesso à informação e aos ativos correspondentes sempre que necessário. Exemplo: se eu recebi uma carta, eu devo ter acesso a sua informação sempre que eu desejar – basicamente a qualquer momento eu posso pegar para ler.

No entanto, o exemplo da carta não é muito elucidativo para esse princípio – eu prefiro explicar esse  princípio  de  outra  maneira! Vocês  já  precisaram  fazer  uma  transferência  de  grana importantíssima e, quando foram acessar o aplicativo do seu banco, ele estava fora do ar? Pois é, isso já aconteceu comigo quando eu tinha uma conta em um banco que eu prefiro nem dizer o nome.
Isso me irritou tanto que eu abri uma conta em outro banco mais confiável!

Vocês percebem a importância desse princípio? O prejuízo de um banco quando seu sistema fica fora ar pode ser de milhões de reais – dependendo do tempo indisponível, bilhões de reais!
Por  essa
razão, há um investimento massivo em recursos que reduzem as chances de o sistema e suas informações   ficarem   indisponíveis . Quais,  professor?  Por  exemplo:  firewalls,  backups, redundâncias, equipamentos de energia, entre outros.


PEGADINHA CLÁSSICA: CONFIDENCIALIDADE X DISPONIBILIDADE A confidencialidade garante que a informação somente esteja acessível para usuários autorizados. Já a disponibilidade garante que a informação esteja disponível aos usuários autorizados sempre que necessário.
(CGM/PB – 2018) A disponibilidade pressupõe que uma informação deva estar disponível a qualquer pessoa de direito, sempre que necessário.
_______________________ Comentários: conforme vimos em aula, questão perfeita (Correto).

(SERPRO – 2013) Um ataque à infraestrutura de conectividade de um banco à Internet, interrompendo o acesso a seus serviços de home banking, afeta a disponibilidade.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








16
84



1.5 – PRINCÍPIOS ADICIONAIS 
1.5.1 – Autenticidade INCIDÊNCIA EM PROVA: Altíssima 
A autenticidade
1
é a propriedade que trata da garantia de que um usuário é de fato quem alega ser
.  Em  outras  palavras,  ela  garante  a  identidade  de  quem  está  enviando  uma  determinada informação. Sabe quando você assina um contrato? A sua assinatura é uma forma (frágil) de garantir que você é quem diz ser! O cartório tem a sua assinatura (chamada firma) e ele pode comparar com a assinatura que consta no contrato.

Galera,  eu  sei  fazer  a  assinatura  do  meu  pai  impecavelmente.  Logo,  eu  poderia  quebrar  essa garantia da autenticidade porque se trata de um método frágil, mas existem outras maneiras de melhorar  essa  garantia  de  autenticidade  –  que  discutiremos  mais  à  frente.  De  toda  forma,  a autenticidade busca garantir que a pessoa que está requisitando acesso a alguma informação é realmente quem ela diz ser .

Hoje em dia é muito fácil se passar por outro em redes sociais, por exemplo! Em tese, nada impediria que  eu  criasse  um  instagram  com  o  nome @fatima_bernardes,  um  facebook  com  o  nome @ronaldinho_gaucho_10 ou um twitter com o nome @cabo_daciolo_51.




1
Alguns autores consideram como princípios fundamentais apenas Confidencialidade, Integridade e Disponibilidade. Já outros consideram também o princípio da Autenticidade.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








17
84



No entanto, as redes sociais criaram a verificação de conta (representado pelo ícone  ). O que é isso, professor? Esse é um recurso criado inicialmente para figuras públicas, celebridades, cantores, artistas, entre outro para evitar que outras pessoas se passem por elas.
Observem nas três redes sociais acima que existe o ícone que mostra que essa conta é autêntica, isto é, ela é realmente de quem diz ser.

Alguém sempre poderá dizer: professor, não é possível garantir isso, porque o celular do dono da conta pode  ter  sido  roubado,  por  exemplo. É  verdade,  absolutamente  nenhum  sistema  é  totalmente seguro. No entanto, quando dissemos que isso garante autenticidade, nós assumimos que não ocorreu  nenhum  incidente  e  que  o  dono  utiliza  uma  autenticação  forte  em  suas  redes.  Em segurança da informação, é comum utilizar o verbo garantir sem problema.

Não se deve confundir Autenticidade com Autorização! A autenticidade verifica se uma pessoa é realmente quem diz ser. No entanto, não é só porque foi verificado que você é realmente quem diz ser que você deve ter acesso a todos os recursos do sistema.
A autorização é o mecanismo que verifica  se  uma  pessoa  possui  permissão  para  executar  determinadas  operações – esse não é considerado um dos princípios da segurança da informação!

(TRF/4 – 2014) A segurança da informação objetiva a proteção de ativos da informação contra acessos não autorizados, alterações indevidas, sendo considerada uma prática de gestão de riscos incidentes que impliquem o comprometimento de seus requisitos e conceitos  básicos.  Dentro  desta  análise  conceitual,  a  garantia  de  que  as  entidades identificadas  em  um  processo  de  comunicação  como  remetentes  ou  autores  sejam, exatamente, os mencionados nela, pode ser conceituada como:

a) severidade.
b) confidencialidade.
c) disponibilidade.
d) criticidade.
e) autenticidade.
_______________________ Comentários: conforme vimos em aula, trata-se do Princípio da Autenticidade (Letra E).

(Prefeitura  de  Vitória  –  2010) Autenticar é confirmar a identidade de uma entidade visando,  por  exemplo,  garantir  que  a  entidade  é  quem  ela  diz  ser.  As  técnicas  para autenticação  podem  basear-se  na  verificação  de  informações  como,  por  exemplo, senhas.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).




Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








18
84



1.5.2 – Irretratabilidade INCIDÊNCIA EM PROVA: Altíssima 
Também chamada de Irrefutabilidade ou Não-repúdio, o princípio da irretratabilidade trata da capacidade de garantir que o emissor da mensagem ou participante de um processo não negue posteriormente  a  sua  autoria.  No  Direito,  o  não-repúdio  implica  a  intenção  de  cumprir  as obrigações de um contrato. Implica também que uma parte de uma transação não possa negar ter recebido uma transação, nem a outra parte pode negar ter enviado uma transação.

É importante notar que, embora a tecnologia – como os sistemas criptográficos – possa ajudar nos esforços de não-repúdio, o conceito é, em sua essência, um conceito legal que transcende o  domínio  da  tecnologia. Como  assim,  professor?  Lembrem-se  do  exemplo  anterior!  Alguém sempre pode falar que teve o celular roubado ou que quem fez a postagem foi um estagiário ou que o algoritmo do sistema está com algum erro.

No  entanto,  é  possível  utilizar  uma  autenticação  forte,  o  que  aumenta  consideravelmente  a confiança  de  que  quem  enviou  a  mensagem  foi  realmente  quem  parece  ser.  Dessa  forma, alguém dificilmente conseguiria negar sua autoria. Em 2015, o Twitter Oficial do STJ publicou o tweet abaixo e o apagou minutos depois. O órgão dificilmente conseguiria negar sua autoria, visto que – como possui uma conta verificada – necessita de autenticação forte.



(TCE/PA – 2016) O princípio de não repúdio impede que o autor de um documento negue a criação e a assinatura desse documento.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).







Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








19
84



2 – CRIPTOLOGIA
2.1 – CONCEITOS BÁSICOS INCIDÊNCIA EM PROVA: baixíssima A informação sempre foi objeto de poder, portanto é comum a criação de técnicas para obter informações de modo não autorizado e, ao contrário, acaba sendo necessário o surgimento de mecanismos de defesa visando proteger as informações. Basicamente a Criptologia se ocupa da ocultação de informações e da quebra dos segredos de ocultação. A primeira pode ser alcançada por Esteganografia ou Criptografia, e a segunda pode ser alcançada por Criptoanálise.

A criptografia possui dois grandes grupos: códigos e cifras. Os códigos são palavras, frases, letras, símbolos usados para substituir elementos do texto claro. As cifras, por sua vez, são algoritmos de criptografia  e  descriptografia  de  mensagens.  Elas  se  caracterizam  por  dois  tipos  básicos  de transformação: transposição e substituição. Vejam abaixo como esses conceitos são dispostos um em relação ao outro.



(STF – 2013) A criptologia incorpora estudos e conhecimentos das áreas de criptografia e criptoanálise.
_______________________ Comentários: conforme  vimos  em  aula,  incorpora  estudos  e  conhecimentos  de  criptografia  e  criptoanálise  –  além  da esteganografia (Correto).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








20
84



2.2 – ESTEGANOGRAFIA INCIDÊNCIA EM PROVA: baixa Trata-se de uma técnica utilizada para esconder informações. Seu objetivo é que as informações sejam transmitidas de forma invisível, sem que possam ser capturadas ou monitoradas. Quem aí tem filhos? Vocês podem fazer um experimento legal com eles: escrevam uma carta secreta com suco de limão! Vocês precisarão de uma folha de papel em branco, um cotonete, um ferro de passar roupa e um copinho com limão espremido.

Molhem a ponta do cotonete no suco de limão, escrevam alguma coisa no papel em branco e deixem secar naturalmente. Vocês perceberão que a folha continuará em branco e não será possível visualizar a mensagem escrita. Após um tempo, peguem o ferro de passar roupa e passem o papel.
A mensagem escrita com o limão de forma invisível aparecerá no papel! Esse é um exemplo bem simples de esteganografia.

Vou compartilhar uma experiência pessoal com vocês! Certa vez, em uma viagem ao Deserto do Saara, fui em um povoado berbere onde um artista fazia pinturas com pigmentos de água com açúcar. Inicialmente, não era possível ver nenhuma definição do que ele estava desenhando.
Até  que  ele  passou  o  papel  em  um  maçarico  de  gás  propano  e  de repente apareceu essa imagem ao lado ! Legal, né?

O guia nos contou que, há trezentos anos atrás, essa era uma forma de enviar mensagens de forma invisível entre as famílias. Depois de um tempo, tornou-se uma forma de arte chamada Piroaquarela ou Aquarela de Fogo. Já na era moderna, a esteganografia aparece como  uma  técnica  para  ocultar  uma  mensagem  dentro  de  outra,  de  forma  que  não  sejam percebidas por terceiros . Em geral, escondem-se mensagens dentro de imagens, sons, vídeos ou textos.

Professor,  como  é  possível  esconder  uma  mensagem  em uma imagem? Não vamos entrar em muitos detalhes sobre o  funcionamento,  mas  basicamente  uma imagem  é  um conjunto pixels codificados em milhões e milhões de bits (Ex: 01101010000101110101011101101000) – como mostra a imagem ao lado!
Se eu modificar apenas alguns desses bits para guardar uma mensagem secreta, não vai fazer muita  diferença  para  você  porque  a  mudança  será imperceptível para o olho humano .

Alguém consegue notar alguma diferença entre a imagem da esquerda e a imagem da direita abaixo?
Pois é, a imagem da direita está esteganografada, isto é, há uma mensagem escondida dentro dela.
Se a pessoa que vai receber a mensagem sabe disso e sabe como decifrá-la, ela conseguirá ver a Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








21
84



mensagem escondida na imagem. Caso contrário, uma pessoa desavisada só vai achar que é uma foto de um panda. E isso pode ser feito com vários tipos de arquivos.



(UFC – 2013) Sobre Esteganografia é correto afirmar que:

a) É uma categoria de algoritmo criptográfico simétrico.
b) É a análise de desempenho dos algoritmos criptográficos.
c) É uma técnica para ocultar uma mensagem dentro de outra.
d) É um  algoritmo matemático capaz de obter a mensagem original a partir do seu código hash.
e) É uma técnica para decifrar o texto cifrado sem qualquer conhecimento da mensagem original e do algoritmo criptográfico utilizado.
_______________________ Comentários: conforme vimos em aula, trata-se de uma técnica de ocultação de uma mensagem dentro de outro (Letra C).

(PC/DF – 2012) Esteganografia é um termo pouco utilizado no âmbito da segurança da informação,  mas  que  exige  cuidados  especiais  de  quem  se  preocupa  com  o  tema.
Assinale a alternativa que apresenta a definição de esteganografia.

a) Técnica de esconder informações dentro de arquivos como imagens, sons, vídeos ou textos.
b)  Sinônimo  de  criptografia,  é  técnica  de  codificar  a  informação  para  que  não  seja entendida por terceiros.
c) Algoritmo matemático que converte um texto claro em uma mensagem cifrada, e vice-versa.
d) Estudo de técnicas de quebra de sigilo de mensagens eletrônicas criptografadas.
e) Método para codificação de arquivos binários, transformando-os em texto ASCII.
_______________________ Comentários: conforme vimos em aula, trata-se de uma técnica de esconder informações dentro de arquivos como imagens, sons, vídeos ou textos (Letra A).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








22
84



2.3 – CRIPTOGRAFIA E CRIPTOANÁLISE 
2.3.1 – Conceitos Básicos INCIDÊNCIA EM PROVA: baixa A  Criptografia  é  a  técnica  de  tornar  uma  mensagem ininteligível! Ela remonta ao Egito por volta de 1.900 A.C., quando     um     escriba     esculpiu     alguns     símbolos hieroglíficos  em  uma  rocha  no  túmulo  do  chefe  egípcio Khnumhotep  II. A criptografia não era tão difícil naquela época, já que a maioria das pessoas era analfabeta e só a elite  podia  ler  qualquer  linguagem  escrita.  Desde  essa época, faraós, reis, imperadores, presidentes, ditadores e comandantes militares usaram a criptografia para esconder comunicações de seus inimigos.

Um  exemplo  é  Maria,  Rainha  dos  Escoceses!  Em  1577, ela  queria assassinar a Rainha Elizabeth I e – para tal – começou a trocar mensagens com seus companheiros de conluio. Para que ninguém desconfiasse caso as mensagens acabassem em mãos erradas, eles as criptografavam! Eles utilizaram uma cifra de substituição, em que você substitui umas letras por outras ou palavras comuns por símbolos.
As  mensagens  de  Maria foram  capturadas  pelos  espiões  da  Rainha  Elizabeth I,  decifradas  e Maria  foi  imediatamente  presa,  julgada  e  condenada por  traição . A
pena  foi  morte  por  decapitação  na  guilhotina.  Essa é  apenas  uma historinha  para  contextualizar  sobre  a  importância da  criptologia  no decorrer da história da humanidade. Bacana? :) 


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








23
84



Falando agora de tempos mais modernos, essa máquina acima é chamada Enigma II. Ela  é uma máquina  eletromecânica  de  criptografia  utilizada  pelos  nazistas  durante  a  Segunda  Guerra Mundial
. Quem assistiu ao filme O Jogo da Imitação (The Imitation Game), que conta a história de Allan Turing – o pai da computação –, deve conhecê-la. Se não assistiram ainda, assistam! É um filmaço! #ficadica :) 
A  Enigma  era  poderosa  e  complexa  por possuir  três  rotores  –  como  mostrado  na imagem  ao  lado  –  para  bagunçar  as  letras digitadas  e  dificultar  a  decifragem  das mensagens.  O
H  digitado  se  tornava  um J, que se tornava um M, que se tornava um Q, que  se  tornava  um P,  que  passava  por  um refletor e se tornava um I, que se tornava um H, que se tornava um N, que finalmente se tornava  um L  na  mensagem  criptografada.
Além  disso,  você  poderia  configurar  a máquina de diversas maneiras, dificultando a decifragem para quem interceptasse.

Ela era utilizada para troca de mensagens entre os generais nazistas. Foi quando o matemático britânico Allan Turing criou uma máquina chamada Bombe capaz de traduzir textos encriptados pelos  alemães  e  decifrando  diversas  mensagens  que  continham  informações  de  planos  e estratégias de guerra. Dessa forma, considera-se que a máquina de criptoanálise de Allan Turing ajudou a encerrar a guerra mais cedo, porque vários ataques alemães foram evitados .


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








24
84



2.3.2 – Técnicas de Criptografia 
Atualmente são empregadas técnicas de criptografias simétricas, assimétricas e híbridas. Essas técnicas empregam dois fundamentos principais: substituição, em que cada elemento no texto claro é mapeado para outro elemento; e transposição, em que os elementos no texto claro original são  reorganizados.  O  requisito  essencial  de  ambos  é  que  nenhuma  informação  seja  perdida!
Vejamos em detalhes...

2.3.2.1 – Criptografia Simétrica INCIDÊNCIA EM PROVA: Altíssima 
A  Criptografia  Simétrica  implica  o  uso  de  uma  chave  secreta utilizada   tanto   para   codificar   quanto   para   decodificar informações. Um dos precursores da criptografia simétrica foi o imperador  romano  Júlio  César,  que  implementou  uma  técnica que  codificava  a  mensagem  a  ser  enviada,  substituindo  cada caractere do texto por um caractere três posições à frente em relação ao alfabeto, conforme a imagem ao lado. Observem que A corresponde a D, D corresponde a G, G corresponde a J, e assim por diante.

D Culswrjudild Slphwulfd lpsolfd r xvr gh xpd fkdyh vhfuhwd xwlolcdgd  wdqwr  sdud  frglilfdu  txdqwr  sdud  ghfrglilfdu lqirupdfrhv.
Up grv suhfxuvruhv gd fulswrjudild vlphwulfd irl r lpshudgru urpdqr Jxolr Chvdu, txh lpsohphqwrx xpd whfqlfd txh frglilfdyd d phqvdjhp d vhu hqyldgd, vxevwlwxlqgr fdgd fdudfwhuh gr whawr sru xp fdudfwhuh wuhv srvlfrhv d iuhqwh hp uhodfdr dr doidehwr, frqiruph d lpdjhp dr odgr. Oevhuyhp txh A fruuhvsrqgh d D, D fruuhvsrqgh d G, G fruuhvsrqgh d J, h dvvlp sru gldqwh.

O  segundo  parágrafo  é  exatamente  o  primeiro  parágrafo,  porém  cifrado  com  a  técnica  do Imperador Júlio César. Bacana, né? Quem quiser brincar, acesse o site abaixo:


https://cryptii.com/pipes/caesar-cipher 

Se  uma  pessoa  interceptar  a  mensagem  do  segundo  parágrafo,  não  conseguirá  decifrar  a mensagem. No entanto, se ela souber qual é a chave de encriptação, facilmente ela conseguirá decodificar a mensagem. E o que seria essa chave de encriptação? É uma informação que controla a operação de um algoritmo de criptografia – na criptografia simétrica, ela é utilizada tanto para codificar quanto para decodificar a mensagem. No caso acima, a chave de Júlio César é 3! Por que?
Porque o caractere verdadeiro e o caractere codificado diferem em três posições.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








25
84




Bacana! Nós entendemos a criptografia simétrica de uma maneira simplificada. Vamos ver agora como isso se aplicaria aos tempos atuais. Vamos supor que Maria precise enviar um documento sensível para João. Ela faz uso de um software de encriptação para proteger seu documento e, para tal, utiliza uma senha ou chave. Ela então envia o documento criptografado para João! João vai conseguir abrir o documento?
Não, porque ele não sabe a senha! E agora?

Maria teria que entregar ou falar pessoalmente qual é a senha para João, mas isso poderia ser um grande  inconveniente.  Ela  poderia  enviá-la  por  e-mail,  mas  seria  arriscado,  visto  que  alguém poderia interceptá-la e utilizá-la para descriptografar o documento sensível. Percebam, então, que essa é uma boa solução para casos mais simples, mas  há  riscos e  inconvenientes. Quem quiser brincar com esse tipo de criptografia ou precisar esconder algum arquivo, eu recomendo:


https://www.aescrypt.com 




























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








26
84



Na primeira figura, eu tenho uma imagem do logo do Estratégia. Na segunda figura, eu clico com o botão direito para utilizar o programa AES Encrypt. Na terceira figura, o programa pede para que eu insira uma senha ou chave – eu utilizo ‘12345’. Na quarta figura, é criado o arquivo criptografado da  imagem.  Na  quinta  figura,  eu  tento  abrir  a  foto e  o  programa  pede  a  senha  –  eu  insiro ‘123456789’. Na última figura, é negada a abertura da imagem por senha incorreta!

Voltando ao nosso contexto: se a pessoa que vai descriptografar o arquivo futuramente for a mesma pessoa que o criptografou, não há muito problema. No entanto, eu poderia enviar esse arquivo criptografado para o meu parceiro, Professor Renato da Costa. Nesse caso, ele só conseguiria abri- lo  se  possuísse  a  senha  ou  chave  que  eu  escolhi. Dessa  forma,  eu  teria  que  encontrá-lo pessoalmente para passar a senha ou chave – isso poderia ser um inconveniente.

Por  fim, é  importante  ressaltar  que  a  criptografia  simétrica  garante  apenas  o  princípio  da confidencialidade, ou seja, ela garante que a mensagem – caso interceptada – seja ininteligível para  o  interceptador.  Ela  não  é  capaz  de  garantir  o  princípio  da  integridade,  ou  seja,  que  a mensagem não foi alterada no meio do caminho. Ademais, ela só é capaz de garantir o princípio da autenticidade caso apenas duas entidades tenham conhecimento da chave secreta.

 Principais algoritmos: DES, 3DES, AES, Blowfish, Cifragem de Júlio César, etc.

(TCE/CE  –  2016) O  método  criptográfico  que  utiliza  apenas  uma  chave  para  a decodificação da informação é conhecida por:

a) chave assimétrica;
b) chave simétrica;
c) assinatura cifrada;
d) chave de codificação distinta.
_______________________ Comentários: conforme vimos em aula, trata-se do método criptográfico conhecido por chave simétrica (Letra B).

(SEFAZ/PB – 2006) Criptografia simétrica é um método de codificação que utiliza:

a)  uma  chave  pública  e  uma  chave  privada  para  encriptar  e  decodificar  a  mesma mensagem.
b) duas chaves públicas para encriptar e decodificar a mesma mensagem.
c) uma só chave para encriptar e decodificar a mesma mensagem.
d) duas chaves privadas para encriptar e decodificar a mesma mensagem.
e)  uma  chave  pública  e  duas  chaves  privadas  para  encriptar  e  decodificar  a  mesma mensagem.
_______________________ Comentários: conforme vimos em aula, ela utiliza uma só chave para encriptar e decodificar a mesma mensagem (Letra C).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








27
84



2.3.2.2 – Criptografia Assimétrica INCIDÊNCIA EM PROVA: Altíssima 
Nós vimos que a Criptografia Simétrica tinha uma falha: havia a necessidade de compartilhar a chave de cifragem/decifragem. A Criptografia Assimétrica (também chamada de Criptografia de Chave Pública) acabou com essa vulnerabilidade ao criar duas chaves distintas e assimétricas – sendo uma pública e uma privada.
A chave pública é disponibilizada para qualquer um e a chave privada é de uso personalíssimo e restrito a um usuário, instituição ou equipamento.

Embora  sejam  chaves  criptográficas  diferentes,  elas  formam  um  par  exclusivo  em  que necessariamente ao se criptografar informações com uma chave pública, somente a chave privada correspondente do par é capaz de descriptografar essas informações e vice-versa. Para entender isso  melhor,  eu  preciso  bastante  da  atenção  de  vocês  agora  –  esse  assunto  é  um  pouquinho complexo e cai muito em prova. Vejam só...



Imaginem que agora é a Maria que precisa receber um documento sensível de João. No entanto, dessa vez, antes de receber qualquer documento, ela decide comprar um cadeado vermelho que vem acompanhado de uma chave vermelha. Dessa forma, ela vai aos correios e envia seu novo cadeado  vermelho  aberto  para  João,  permanecendo  com  a  chave  vermelha  sob  sua  posse.
Entendido?


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








28
84




João recebe o cadeado vermelho aberto e decide comprar um cadeado azul com uma única chave.
Além  disso,  ele  compra  uma  caixa.  Então, ele  insere  seu  cadeado  azul  aberto  junto  com  o documento sensível que Maria precisa, coloca tudo dentro dessa caixa, permanece com a sua chave azul, mas tranca a caixa com o cadeado vermelho que foi enviado aberto por Maria e envia a caixa para ela por meio dos correios.

Maria recebe a caixa trancada com seu cadeado vermelho e – como somente ela possui a chave vermelha para o cadeado vermelho – destranca a caixa e encontra o cadeado azul aberto de João junto  do  documento  sensível.  Pronto!  Agora  toda  vez  que  eles  precisarem  enviar  documentos sensíveis um para o outro, eles podem inseri-los na caixa junto de seu cadeado aberto e trancá-la com o cadeado do outro. Simples, né?

Esse  método  é  interessante  porque,  caso  o  carteiro ou  qualquer  outra  pessoa  intercepte  a caixa,  ele  não  conseguirá  abri-la. Por que, professor? Porque a chave nunca é enviada! O que é enviado é apenas o cadeado aberto – cada um permanece com sua chave. Em nossa analogia, o cadeado aberto representa a chave pública e a chave do cadeado representa a chave privada. No entanto, toda metáfora tem suas limitações. Logo, vamos retornar agora aos computadores!

Na Criptografia Assimétrica, nós possuímos duas chaves diferentes – uma chave pública e uma chave privada – por essa razão, é chamada de criptografia assimétrica.
Esse par de chaves formam um  par  exclusivo
,  de  modo  que  um  texto  criptografado  pela  chave  pública  só  pode  ser descriptografado  pela  chave  privada  e  um  texto  criptografado  pela  chave  privada  só  pode  ser descriptografado pela chave pública. Bacana?

A chave pública é realmente pública – você pode contar qual é a sua chave pública para todo mundo.
Evidentemente, a chave privada é exclusivamente sua!
Similarmente,  o  número  da  sua  conta corrente é público – ela seria sua chave pública. Já a senha de transação da sua conta corrente é privada – ela seria sua chave privada . Professor, quando eu quiser criptografar uma mensagem, eu devo usar a minha chave pública ou minha chave privada? Depende!



O emissor que deseja enviar uma informação sigilosa deverá utilizar a chave pública do destinatário para criptografar essa informação sigilosa. Para isto, é importante que o destinatário disponibilize Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








29
84



sua  chave  pública. O  Princípio  da  Confidencialidade  é  garantido,  uma  vez  que  somente  o destinatário que possui a chave privada específica dessa chave pública conseguirá desfazer a operação de criptografia – como mostra a imagem anterior.



Professor, o que acontece se eu utilizar minha chave privada para criptografar uma informação? Nesse caso, qualquer um que possua sua chave pública conseguirá descriptografá-la e visualizá-la. E como sua chave pública é literalmente pública, você não garantirá o princípio da confidencialidade.
Por
outro lado, você garantirá o Princípio da Autenticidade . Como assim, professor? Vejam só...

Nós sabemos que o princípio da Autenticidade garante que determinada pessoa é realmente quem ela  diz  ser.  Se  alguém  utilizar  a  minha  chave  pública  para  descriptografar  uma  informação  e conseguir,
ela terá certeza de que fui eu que realmente criptografei aquela informação. Por que?
Porque  se  a  informação  foi  descriptografada  com  minha  chave  pública,  ela  só  pode  ter  sido criptografada com minha chave privada. E adivinhem: somente eu possuo minha chave privada!

 Principais algoritmos: RSA, DSA, ECDSA, etc.

(PC/GO  –  2015) Criptografia  é  a  ciência  de transformar  mensagens  para  ocultar  seu significado  de  intrusos.  Considerando  essa  informação,  assinale  a  alternativa  que apresenta  a  técnica  de  criptografia  que  utiliza  a  chave  pública  para  codificar  as mensagens.

a) cifragem de chave simétrica b) hashing
c) estaganografia
d) cifragem de chave assimétrica e) assinatura digital _______________________ Comentários: trata-se da cifragem de chave assimétrica (Letra D).

(SEFAZ/PI – 2015) Em determinada instituição, João envia uma mensagem Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








30
84



criptografada para Antônio, utilizando criptografia assimétrica. Para codificar o texto da mensagem, João usa:

a) a chave privada de Antônio. Para Antônio decodificar a mensagem que recebeu de João, ele terá que usar sua chave privada. Cada um conhece apenas sua própria chave privada.

b) a chave pública de Antônio. Para Antônio decodificar a mensagem que recebeu de João, ele terá que usar a chave privada, relacionada à chave pública usada no processo por João. Somente Antônio conhece a chave privada.

c) a chave pública de Antônio. Para Antônio decodificar a mensagem que recebeu de João, ele terá que usar a chave privada, relacionada à chave pública usada no processo por João. Ambos conhecem a chave privada.

d) a chave privada de Antônio. Para Antônio decodificar a mensagem que recebeu de João, ele terá que usar a chave pública, relacionada à chave privada usada no processo por João. Ambos conhecem a chave privada.

e) sua chave privada. Para Antônio decodificar a mensagem que recebeu de João, ele terá que usar sua chave pública. Somente João conhece a chave privada.
_______________________ Comentários: conforme vimos em aula, caso seja para garantir a confidencialidade, João utilizará a chave pública de Antônio.
Para Antônio decodificar a mensagem que recebeu de João, ele terá que usar a chave privada, relacionada à chave pública usada no processo por João. Somente Antônio conhece a chave privada (Letra B).




























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








31
84



2.3.2.3 – Criptografia Híbrida INCIDÊNCIA EM PROVA: baixíssima 
A Criptografia Assimétrica tem vantagens em relação a Criptografia Simétrica, mas também tem desvantagens. Em geral, as chaves simétricas são bem menores que as chaves assimétricas. Dessa forma, a Criptografia Assimétrica chega a ser até cem vezes mais lenta que a Criptografia Simétrica.
Por essa razão, é comum a utilização de uma Criptografia Híbrida, ou seja, uma combinação da Criptografia Simétrica e Criptografia Assimétrica.

Basicamente,  utiliza-se  um  algoritmo  de  Criptografia  Assimétrica  apenas  para  trocar  chaves simétricas  –  chamadas  de  chaves  de  sessão  –  de  forma  segura .  Logo,  após  a  troca,  toda comunicação  é  realizada  utilizando  um  algoritmo  de Criptografia  Simétrica. Protocolos  como Secure  Sockets  Layer (SSL)  utilizam  chaves  de  sessão  para  criptografar  e  descriptografar informações. Entendido, galera?

(TJ/PA – 2009) Para manter a segurança das comunicações via Internet, o protocolo SSL (Secure Sockets Layer) utiliza sistemas criptográficos:

a) simétricos de chaves públicas.
b) assimétricos de chaves privadas.
c) simétricos de chaves privadas.
d) assimétricos de chaves de sessão.
e) simétricos de chaves de sessão.
_______________________ Comentários: conforme vimos em aula, utiliza sistemas criptográficos simétricos de chaves de sessão. Professor, mas ele não utiliza a criptografia assimétrica? Sim, mas apenas para trocar as chaves de sessão. A segurança da comunicação é mantida pelo SSL por meio de sistemas criptográficos simétricos de chaves de sessão (Letra E).














Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








32
84



3 – AUTENTICIDADE
3.1 – CONCEITOS BÁSICOS INCIDÊNCIA EM PROVA: baixa 
No  início  dessa  aula,  nós  vimos  que  a  Autenticidade  é  um  dos  princípios  da  Segurança  da Informação.  Em  seguida,  no  contexto  de  Criptografia,  nós  vimos  que  é  possível  garantir  a Autenticidade utilizando Criptografia Assimétrica – para tal, basta criptografar a mensagem com sua  chave  privada.
Podem-se  utilizar  diversos  métodos  de  autenticação,  inclusive  uma combinação entre eles. Veremos abaixo os principais:



3.1.1 – Método de Autenticação: O que você sabe?

Trata-se da autenticação baseada no conhecimento de algo que somente você sabe, tais como:
senhas, frases secretas, dados pessoais aleatórios, entre outros.

3.1.1.1 – Senhas

Hoje em dia, a combinação mais utilizada para autenticação em sistemas de informação é: Usuário e Senha. Essa é a forma de autenticação mais fácil de se implementar! No entanto, essa forma de autenticação pode ser comprometida se eventualmente hackers descobrirem essa combinação – como nós já vimos, a senha mais utilizada no mundo no ano passado foi ‘12345’ (cuidado com as senhas de vocês!).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








33
84




Notem que uma senha de cinco dígitos – como a senha acima – é muito fácil de ser quebrada por um computador. Só existem 10.000 possibilidades – o que  não  é  nada  para  um  computador  com  processamento  razoável.
Ele
pode  testar  todas  essas  possibilidades  em  milésimos  de  segundo  –  é  o chamado Ataque de Força Bruta . Claro que há estratégias para mitigar esse risco. Você já errou três vezes a senha do seu celular? Pois é, ele te bloqueia por um período!

Outra estratégia é obrigar que a senha tenha alguns requisitos básicos para ser mais difícil de ser quebrada ou descoberta. Vocês já devem ter visto algo mais ou menos assim:

ESTRATÉGIAS DE SENHAS Utilize pelo menos oito caracteres (algumas normas recomendam seis caracteres);
Mescle letras minúsculas e maiúsculas, números, espaços, pontuação e outros símbolos;
Evite utilizar um caractere mais de duas vezes; não a anote, memorize-a;
Evite utilizar informações pessoais, como nome do filho, aniversário da mãe, etc;
Alterar as senhas com frequência e não utilizar a mesma senha em contas diferentes;
Substituir alguns caracteres por números parecidos como: D13G0 C4RV4LH0;
Não utilizar sequências de teclado como: QWERTY, ASDFGH ou ZXCVBN;
Certificar de encerrar uma sessão ao acessar sites que requeiram uso de senhas;
Não escolher palavras que façam parte do dicionário.

Notem  que  uma  senha  de  oito  dígitos  numéricos  tem  apenas  um milhão  de  combinações  possíveis  –  é ridiculamente  fácil  para  um computador   testar   todas   as   possibilidades em  pouco  tempo
utilizando um ataque de força bruta. No entanto, uma senha de oito caracteres que podem ser números, símbolos, maiúsculos, minúsculos, entre outros, pode ter mais de 600 trilhões de combinações. Aí fica bem mais  complexo  para  qualquer  computador  pessoal! Entendido?
Prossigamos...

3.1.2 – Método de Autenticação: O que você é?

Trata-se  da  autenticação  baseada  no  conhecimento  de  algo  que  você  é,  como  seus  dados biométricos
.  Exemplos:  impressão  digital,  padrão  de  retina,  reconhecimento  de  voz, reconhecimento  facial,  assinatura  manuscrita  (característica  comportamental  individual),  etc.
Dessa forma, a não ser que você possua um irmão gêmeo univitelino, somente você possuirá a maioria dessas características físicas ou biométricas.

3.1.2.1 – Biometria

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








34
84



Utiliza características físicas únicas para verificar sua identidade. A biometria mais famosa é a impressão digital, entretanto podemos ter acessos biométricos através do reconhecimento de voz, varredura de retina e imagine, até mesmo DNA! Hoje em dia, diversos computadores portáteis trazem consigo um Leitor de Digital para, inclusive, fazer logon no Sistema Operacional.

3.1.3 – Método de Autenticação: O que você tem?

Trata-se da autenticação baseada em algo que somente o verdadeiro usuário possui, tais como:
celulares, crachás, Smart Cards, chaves físicas, tokens, etc. É um bom método de autenticação, porque resolve o problema da  adivinhação por força bruta. Ademais, ela tipicamente requer  a presença física do usuário, portanto é bem mais difícil para atacantes remotos conseguirem acesso.
Como assim, professor?

Galera, alguém em outra cidade não consegue abrir a porta do meu apartamento sem antes vir à minha cidade. Dessa forma, esse método de autenticação possui uma dificuldade bem maior de ser quebrada.
No entanto,
ele ainda pode ser comprometido se o atacante estiver fisicamente  próximo . Chaves podem ser copiadas, celulares podem ser roubados e trancas podem ser arrombadas. Entendido? Vamos ver alguns exemplos!

3.1.3.1 – Smart Cards 
Um Smart Card é um cartão inteligente. Trata-se simplesmente de um
cartão de plástico contendo um microprocessador – um chip – que armazena informações eletrônicas sobre o usuário (Ex: Chaves), servindo como uma mídia criptográfica. O e-CPF, por  exemplo,  é  um  CPF  digital  em  um  cartão  inteligente  que garante a autenticidade e a integridade na comunicação.

3.1.3.2 – Tokens

Os tokens  são  objetos  de  autenticação!  Podem  servir  para armazenar senhas aleatórias (One  Time  Password) ou podem conter  um  conector  USB  servindo  como  mídia  criptográfica, armazenando informações sobre o usuário (Certificado Digital), assim como um Smart Card.

(EMBASA  –  2018) Em  um  sistema  de  controle  de  acesso,  os  usuários  podem  ser autenticados  usando-se  biometria,  que  necessariamente  consiste  em  fazer  a digitalização e o reconhecimento de impressões digitais e é considerada uma das formas mais precisas e efetivas de autenticação.
_______________________ Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








35
84



Comentários: conforme vimos em aula, a biometria não requer necessariamente a coleta da impressão digital – há várias identificações biométricas diferentes (Errado).

(DPE/RJ – 2014) Senhas podem ser fracas ou fortes, dependendo do grau de dificuldade que um hacker, ou software malicioso, teria para quebrá-la. Um fator que fortalece uma senha é o emprego de:

a) caracteres repetidos.
b) letras maiúsculas exclusivamente.
c) letras, números e símbolos do teclado.
d) nomes próprios.
e) palavras completas.
_______________________ Comentários: conforme vimos em aula, deve-se empregar letras, números e símbolos do teclado (Letra C).





























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








36
84



3.2 – AUTENTICAÇÃO FORTE INCIDÊNCIA EM PROVA: baixa 
Nós acabamos de ver três métodos de autenticação e sabemos que todos eles possuem riscos e vulnerabilidades, no entanto – quando nós combinamos métodos de autenticação – nós temos uma confiança maior na autenticidade.
Dessa forma, surgiu a Autenticação Forte, que é um tipo de autenticação   que   ocorre   quando   se   utiliza   pelo   menos   dois   desses   três   métodos   de autenticação
. Um exemplo é a Autenticação em Dois Fatores (ou Verificação em Duas Etapas)!

Um atacante pode adivinhar sua senha ou roubar o seu celular, mas é muito mais improvável que ele consiga fazer ambos . Hoje em dia esse tipo de autenticação está ficando cada vez mais comum. Em geral, você utiliza algo que você sabe (Ex: Senha) para acessar um sistema. Ele, então, envia uma mensagem com um código para algo que você tem (Ex: Celular). Você insere esse código e pronto... estará autenticado, ou seja, o sistema saberá que você é realmente você.

Quando você saca dinheiro em um caixa eletrônico, você também utiliza dois métodos de autenticação. Primeiro, você insere seu cartão (algo que você tem). Após escolher o valor que você deseja sacar, você insere ou uma senha (algo que você sabe) ou sua impressão digital (algo que você é). É isso que vocês precisam saber!

(TRF/5  –  2017) Um  Analista  deve  implementar  o  controle  de  acesso  ao  sistema computacional do Tribunal, utilizando o mecanismo de autenticação forte baseada em dois fatores. São eles:

a) cartão de identificação e token.
b) frase de segurança e PIN.
c) token e PIN.
d) impressão digital e padrão de voz.
e) senha e frase de segurança.
_______________________ Comentários: conforme vimos em aula, é o token (algo que você tem) e o PIN (algo que você sabe). PIN é o Personal Identification Number – é como uma senha (Letra C).







Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








37
84



3.3 – ASSINATURA DIGITAL 
3.3.1 – Conceitos Básicos INCIDÊNCIA EM PROVA: Altíssima 
Galera, existem  alguns  momentos  em  que  soluções  antigas  infelizmente  não  atendem  mais nossas  demandas  modernas . Vocês já pararam para pensar como é antiquado e inseguro assinar documentos e contratos utilizando um papel e uma caneta? Pois é! No Brasil, cartórios pegam fogo com frequência. Além disso, assinaturas podem ser facilmente copiadas. As demandas modernas exigem uma solução mais flexível e responsiva! Concordam comigo?

Imaginem que Felipe mora na Itália e deseja fechar um contrato com o empresário Lucas, que mora em  Londres.  Para  que  o  contrato  chegue  até  o destinatário,
ele  deve  ir  fisicamente  e  pode demorar semanas por conta das idas e vindas .

Se  ambos  utilizassem  assinaturas  digitais,  eles poderiam fechar contratos em questão de minutos em vez de semanas. Para tal, bastaria selecionar o documento, clicar com o botão direito, assinar digitalmente utilizando um código de segurança e enviá-lo por e-mail. O processo ocorre completamente sem papel e em alguns lugares – como a União Europeia –
um contrato assinado digitalmente vale tanto quanto um contrato assinado fisicamente
. Pois bem...

Nós vimos que é possível utilizar a Criptografia Assimétrica de duas maneiras: se eu criptografo uma mensagem com a chave pública do destinatário, eu garanto o Princípio da Confidencialidade;
se eu
criptografo   uma   mensagem   com   a   minha   chave   privada,   eu   garanto   o   Princípio   da Autenticidade
.  No  entanto,  vamos  ser  mais  ambiciosos:  a  Assinatura  Digital  garantirá  a Autenticidade, a Integridade e a Irretratabilidade.

Para descobrir como ela fará isso, precisamos entender um conceito chamado: Algoritmo de Hash  (ou  Resumo)! O  Algoritmo  de  Hash  é  basicamente  um  algoritmo  criptográfico  que transforma uma entrada de dados em uma saída de dados. No entanto, essa definição é muito genérica, então vamos detalhar mais! Esse algoritmo é capaz de transformar dados de entrada de qualquer tamanho – de poucos bits a muitos terabytes – em dados de saída de tamanho fixo 2
.

Eu suma: o que vocês precisam memorizar é que o algoritmo de hash basicamente recebe dados de  entrada  de  qualquer  tamanho  e  produz  um  dado  de saída  de  tamanho  fixo. Um exemplo clássico é a Função de Resto ou Módulo. Vocês se lembram lá na segunda série do ensino fundamental 
2
Um arquivo de 50 Gb, por exemplo, pode gerar um hash (também chamado Message-Digest ou Resumo de Mensagem) de alguns bits.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








38
84



quando a Tia ensinou para a turma como funcionava uma divisão? Nós tínhamos o dividendo, divisor, quociente e resto! Vejam só:



A  Função  Resto  ou  Módulo  funcionava  assim:  dado  um dividendo  e  um  divisor,  a  função retornava um resto
. Na imagem à esquerda, o dividendo era 10 e o divisor era 3, logo a Função Resto resultou em 1. Por que? Porque 1 é o resto da divisão de 10 por 3. Na imagem à direita, o dividendo era 942.386 e o divisor era 3, logo a Função Resto resultou em 2. Por que? Porque 2 é o resto da divisão de 942.386 por 3.

Professor, o que isso tem a ver com a Função Hash? Galera, notem que – quando a entrada foi um dividendo de dois dígitos (10) – o resto teve apenas um dígito (1). E quando a entrada foi um dividendo de seis dígitos (942.386), o resto também teve apenas um dígito (2). Em outras palavras, não importa se a entrada tem um dígito ou um trilhão de dígitos, a saída sempre terá apenas um único dígito
. Legal né? Vejam quantos dígitos temos abaixo e a saída foi... 1.



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








39
84



O Algoritmo de Hash faz algo similar: dada uma entrada de tamanho qualquer, ele a transforma em uma saída de tamanho fixo. Querem outro exemplo legal? Vejam o número de um boleto:



No boleto acima, percebam que há um número 1 totalmente isolado. Esse número é chamado de Dígito Verificador e é calculado em função de todos os outros dígitos do boleto de forma que qualquer  alteração  nos  demais  dados  geraria  um  Dígito  Verificador  diferente.  Dessa  forma,  o sistema de um banco é capaz de perceber facilmente se há algum erro de digitação no boleto. Dada uma entrada, gerou-se uma saída de tamanho fixo – chamado Dígito Verificador.

Um último exemplo é o Cadastro de Pessoa Física (CPF).
Nesse caso, os dois últimos dígitos são os Dígitos Verificadores – eles são calculados de acordo com um algoritmo definido pela Receita Federal. O CPF 123.456.789-12 não é válido porque – dada a entrada 123.456.789 – a saída 12 não é válida. Por outro lado, o CPF 105.828.626-98 é válido porque – dada a entrada 105.828.626 – a única saída válida é 98. Bacana?

Agora uma pergunta: se eu souber a saída, eu consigo descobrir qual é a entrada? Não, o Algoritmo de Hash tem apenas uma direção!
Em outras palavras, eu não consigo saber qual é o número do boleto  baseado  apenas  no  dígito  verificador. Eu posso te dizer sem problema que o número verificador do meu CPF é 71. E aí, vocês conseguem descobrir qual é o restante? Não, porque ele só tem uma direção.

Outra característica do Algoritmo de Hash é que dada uma mesma entrada, a saída sempre será a mesma, ou seja, o resto da divisão de 10 por 3 é 1 – nunca será 2, 3, 4, etc.
O Algoritmo de Hash
tem um problema: diferentes entradas podem gerar a mesma saída – nós chamamos isso de colisão! Por exemplo: o resto da divisão de 10 por 3 é 1, mas o resto da divisão de 13 por 3 também é 1, isto é, para entradas diferentes, tivemos a mesma saída.


UM ALUNO RECENTEMENTE FEZ QUESTÃO DE FAZER AS CONTAS PARA PROVAR QUE ISSO É VERDADE ;) Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








40
84




A Função de Resto ou Módulo não é um bom Algoritmo de Hash para criptografia de senhas, porque ele é bastante suscetível a colisões. Uma forma de reduzir a chance de colisões é aumentando o tamanho fixo de saída.
Atualmente, Algoritmos Criptográficos de Hash exigem pelo menos 128 bits de saída –  isso é 2128 possibilidades, isso é mais que todos os grãos de areia do Planeta Terra
.

Dessa forma, é muito difícil haver uma colisão, isto é, entradas diferentes gerarem um mesmo resultado! Vamos resumir tudo que vimos: o Algoritmo de Hash é uma função unidirecional que – dada uma entrada de dados de tamanho qualquer – sempre gera uma saída de dados de tamanho fixo,
sendo que a mesma entrada sempre gerará a mesma saída e recomenda-se uma saída com um tamanho grande para evitar colisões.

Uma Função de Hash bastante famosa é o MD5! Notem que o tamanho é sempre fixo e que – por menor  que  seja  uma  mudança  –  gera  um  resultado  completamente  diferente.  Entre  as  duas primeiras frases, a única diferença é um sinal de exclamação.
No entanto, nós podemos chegar até  o  nível  de  bits,  isto  é, um  único  bit  diferente  pode  gerar  um  resultado  completamente diferente
. Vamos ver sua aplicação em algumas frases:

FRASE HASH
Oi

0f3abd55f538f9f343524200a452ffbc (32 caracteres) Oi!

7349da19c2ad6654280ecf64ce42b837 (32 caracteres) Oi, pessoal! O Professor Diego é flamenguista e o Professor Renato é vascaíno.
9ed868b2aa98ce95aaa08ef1065ad8fc (32 caracteres) 
Se eu fizesse o hash da Bíblia inteira, daria um resultado com esse mesmo tamanho fixo acima.
Quem quiser brincar um pouquinho com hash, basta acessar a página abaixo:


https://www.md5hashgenerator.com 


Quando você faz um cadastro em um site e cria uma senha, o site não armazena a sua senha – ele armazena o hash da sua senha. Por que? Porque armazenar a sua senha seria inseguro, visto que o administrador do site poderia roubá-la e utilizá-la para fins escusos.
Após o cadastro, toda vez que você acessar o site com sua senha, ele gerará outro hash e comparará com o hash que ele tem salvo do cadastro. Se forem iguais, significa que você é realmente você :)
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








41
84




Agora qual é a  relação entre Algoritmo de Hash e Assinatura Digital? Nosso  objetivo  é  garantir Autenticidade, Integridade e Irretratabilidade . Nós já sabemos que – para garantir autenticidade – basta utilizar a Criptografia Assimétrica e cifrar a informação com a minha chave privada. Nós também sabemos que – para garantir a integridade – basta utilizar um Algoritmo de Hash. Então, combinamos essas duas estratégias para alcançar nosso objetivo.

Na figura a seguir, Maria possui uma mensagem em claro (sem criptografia). Ela gera um hash dessa mensagem, depois criptografa esse hash utilizando sua chave privada. Em seguida, ela envia para
João tanto a mensagem original quanto o seu hash . João gera um hash da mensagem original e obtém um resultado. Depois descriptografa o hash da mensagem utilizando a chave pública de Maria e obtém outro resultado.



Dessa forma, ele tem dois hashes para comparar: o que ele gerou a partir da mensagem em claro e o que ele descriptografou a partir da mensagem criptografada. Se forem iguais, significa que Maria realmente enviou a mensagem e que ela não pode negar que enviou o documento e, por fim, significa que o documento está íntegro.
E essa é a Assinatura Digital baseada em Hash – ela não se preocupa com a confidencialidade, qualquer um pode visualizar a mensagem.

Agora  notem  que  a  mensagem  enviada  por  Maria  foi  recebida  integralmente  por  João  sem nenhuma modificação no meio do caminho. Além disso, João tem certeza de que foi Maria quem a enviou  porque  só  uma  mensagem  criptografada  com  a  chave  privada  de  Maria  seria descriptografada com a chave pública de Maria.
Se João tem certeza de que Maria que enviou a mensagem e que ninguém a alterou do caminho, Maria não pode negar que a enviou .
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








42
84





Em outras palavras,
a garantia da autenticidade e da integridade garante automaticamente a irretratabilidade ou não-repúdio. Que fantástico, professor! Eu sei, eu sei...

 Principais algoritmos: SHA-1 (Hash de 160 bits), MD5 (Hash de 128 bits), etc 
(BAHIAGÁS – 2010) Uma assinatura digital é um recurso de segurança cujo objetivo é:

a) identificar um usuário apenas por meio de uma senha.
b) identificar um usuário por meio de uma senha, associada a um token.
c) garantir a autenticidade de um documento.
d) criptografar um documento assinado eletronicamente.
e) ser a versão eletrônica de uma cédula de identidade.
_______________________ Comentários: conforme vimos em aula, o objetivo é garantir a autenticidade de um documento (Letra C).

(TJSC – 2011) Em segurança da informação, “assinatura digital” diz respeito a:

a) Ação de digitalizar uma assinatura em papel e incluí-la em documentos eletrônicos.

b) Uma tecnologia que permite dar garantia de integridade a autenticidade a arquivos eletrônicos, através da aplicação de operações criptográficas e da utilização de chaves.

c) Ação de escrever sobre a tela de um computador com uma caneta especial.

d) Uma tecnologia que permite a digitalização das impressões digitais do usuário.

e) Ação de digitar o nome completo do usuário no momento de escrever uma mensagem de e-mail.
_______________________ Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








43
84



Comentários: conforme vimos em aula, é uma tecnologia que permite dar garantia de integridade e autenticidade a arquivos eletrônicos, através da aplicação de operações criptográficas e da utilização de chaves (Letra B).

(SEFAZ/PE   –   2014) O  método  criptográfico  normalmente  utilizado  para  gerar assinaturas digitais que, quando aplicado sobre uma informação, independentemente do tamanho que ela tenha, gera um resultado único e de tamanho fixo é chamado de:

a) abstract key.
b) hash.
c) patch.
d) hoax.
e) compact brief.
_______________________ Comentários: conforme vimos em aula, trata-se do hash (Letra B).

(ELETROBRÁS – 2016) Ao se enviar arquivos pela internet há um método criptográfico que permite verificar se o arquivo foi alterado, ou seja, se teve sua integridade violada.
Esse método, quando aplicado sobre as informações do arquivo, independente do seu tamanho, gera um resultado único de tamanho fixo. Assim, antes de enviar o arquivo pode-se aplicar esse método no conteúdo do arquivo, gerando um resultado A. Quando o arquivo é recebido pelo destinatário, pode-se aplicar novamente o método gerando um resultado B. Se o resultado A for igual ao resultado B significa que o arquivo está íntegro e não foi modificado; caso contrário, significa que o arquivo teve sua integridade violada. O método criptográfico citado é conhecido como:

a) função de hash.
b) criptografia simétrica.
c) esteganografia.
d) criptografia assimétrica.
e) certificação digital.
_______________________ Comentários: conforme vimos em aula, trata-se da Função de Hash (Letra A).









Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








44
84



3.4 – CERTIFICADO DIGITAL 
3.4.1 – Conceitos Básicos INCIDÊNCIA EM PROVA: Altíssima 
Foi legal estudar Assinatura Digital, mas ela tem um problema grave! Nós falamos que – se Maria quisesse enviar uma mensagem para João – ela deveria criptografá-la com a sua chave privada.
Entende-se, portanto, que a chave pública de Maria esteja divulgada em algum lugar para que possa ser encontrada por qualquer pessoa ou que Maria tenha enviado de alguma forma a sua chave pública para o João.

No  entanto,  Suzana  poderia  interceptar  a  mensagem  de  Maria  para  João.  Ela  poderia  jogar mensagem original fora, criar uma nova mensagem com um recado diferente, criptografá-la com a sua chave privada e enviá-la junto com a sua chave pública para João.
Quando João recebesse a mensagem,  ele  utilizaria  a  chave  pública  recebida  (de  Suzana)  para  descriptografar  a mensagem e acharia que se tratava realmente de uma mensagem de Maria.




É como se você criasse uma corrente em uma rede social pedindo doações para ajudar alguém que esteja precisando de um tratamento de saúde. No entanto, em vez de publicar o número da conta corrente  dessa  pessoa,  você  publicasse  o  seu  número  de  conta  corrente.
Isso  significa  que  a Assinatura Digital possui uma autenticação relativamente frágil, porque não é possível saber se a chave pública que foi utilizada é realmente de quem diz ser.

Notem que João utilizou a chave pública recebida (que ele pensava ser de Maria, mas era de Suzana) e conseguiu descriptografar a mensagem. Coitado, ele acreditou que tinha sido Maria que havia enviado e agora acha que ela o odeia! Legal, mas agora chegamos em um impasse! Como eu vou confiar na chave pública de alguém agora, Diego?
Para resolver esse problema, é necessária uma terceira parte confiável chamada Autoridade Certificadora (AC).

A Autoridade Certificadora é uma entidade responsável por emitir certificados digitais – ela é uma espécie de Cartório Digital. Antes da existência de cartórios, existiam muitas fraudes porque contratos eram fraudados utilizando uma cópia assinatura do contratante. Foi necessária a criação Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








45
84



de um cartório – uma terceira parte confiável – que armazenava a assinatura de várias pessoas. Se alguém quisesse confirmar essa assinatura, bastava ir a um cartório.

Um contrato de locação, por exemplo, possui a assinatura do locatário, locador e fiador. Cada um desses tem que ir ao cartório reconhecer firma – criada anteriormente. Quem nunca fez isso? Você vai ao cartório, mostra o contrato assinado e assina na frente do tabelião ou do registrador.
Dessa
forma,  você  atesta  a  autoria  da  assinatura  que  consta  em  um  documento. É  meio  frágil, concordam comigo?

A  Autoridade  Certificadora  faz  algo  similar:  ela mantém   documentos   chamados   Certificados Digitais.  Esse  documento  contém  o  nome,  registro civil e chave pública do dono do certificado, a data de validade, versão e número de série do certificado, o nome  e  a  assinatura  digital  da  autoridade certificadora, algoritmo de criptografia utilizado, etc.
A   Autoridade   Certificadora   é   responsável   por emitir,   distribuir,   renovar,   revogar   e   gerenciar certificados digitais .

Para  que  a  Autoridade  Certificadora  também  seja  confiável,  sua  chave  pública  deve  ser amplamente difundida de tal modo que todos possam conhecer e atestar a sua assinatura digital nos certificados gerados, o que dificulta possíveis fraudes. Vamos pensar no dia-a-dia agora! Vocês estão vendo aquele cadeado no canto esquerdo da Barra de Endereço? Pois é... o que será que significa esse cadeado?



Esse cadeado significa que essa página web provavelmente fornece um serviço crítico em que trafegam informações sigilosas, portanto ela oferece um canal de comunicação criptografado e  seguro
.  No  caso,  trata-se  da  utilização  do  protocolo  HTTPS,  que  é  uma  implementação  do protocolo HTTP sobre uma camada adicional de segurança que utiliza o protocolo SSL/TLS.

Essa camada adicional de segurança permite que os dados sejam transmitidos por meio de uma conexão criptografada e que se verifique a autenticidade do servidor e do cliente por meio do uso de certificados digitais. Nesse caso específico, o seu navegador precisa ter garantias de que ele está trocando informações com o banco e não com outra página web se passando pelo banco.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA ==12b2d8==









46
84



Para tal, a página do banco envia seu certificado digital, que contém seu algoritmo de criptografia, sua chave pública e o nome da autoridade certificadora que emitiu seu certificado. O seu navegador web possui uma lista de certificados confiáveis conforme é apresentado na imagem abaixo. No caso do  Google  Chrome,  essa  lista  fica  em Configurações  >  Privacidade  e  Segurança  >  Gerenciar Certificados.



O navegador verifica se a autoridade certificadora que assinou o  certificado  dele  é  uma  das  autoridades  certificadoras armazenadas no navegador. Se  realmente  for, isso  significa que  o  navegador  pode  confiar  que  o  banco  é  realmente  o banco e aparecerá o cadeado mostrando que a comunicação é segura
. Em algumas situações, você tentará utilizar um site cujo certificado não é confiável e o navegador informará sobre esse risco. Você assume o risco e decide se continua ou não.
Uma  Autoridade  Certificadora  é  também  responsável  por publicar  informações  sobre  certificados  que  não  são  mais confiáveis.

Sempre que ela descobre ou é informada de que um certificado não é mais confiável, ela o inclui em uma  "Lista  Negra",  chamada  de  Lista  de  Certificados  Revogados  (LCR). A  LCR  é  um  arquivo eletrônico  publicado  periodicamente  pela  Autoridade  Certificadora,  contendo  o  número  de série  dos  certificados  que  não  são  mais  válidos  e  a  data  de  revogação. Quando isso ocorre, geralmente aparece a mensagem abaixo ao tentar acessar um site.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








47
84





Em suma:
certificado digital é um documento eletrônico assinado digitalmente por uma terceira parte  confiável  (Autoridade  Certificadora)  e  que  cumpre  a  função  de  associar  uma  entidade (pessoa, processo, servidor, etc) a um par de chaves criptográficas com o intuito de tornar as comunicações mais confiáveis.
Em conjunto com outros recursos, ele pode garantir autenticidade, integridade e não-repúdio, e até confidencialidade.

(TJ/RS  –  2013) Assinale a alternativa que apresenta um dos dados presentes em um certificado digital.

a) Chave privada de criptografia do dono do certificado.
b) Chave única da entidade certificadora raiz.
c) Chave privada de criptografia do emissor do certificado.
d) Chave pública de criptografia do emissor do certificado.
e) Chave pública de criptografia do dono do certificado.
_______________________ Comentários: conforme vimos em aula, ele armazena a chave pública de criptografia do dono do certificado. E por que a Letra D está errada? Porque o emissor do certificado é a Autoridade Certificadora e a chave pública de criptografia da Autoridade Certificadora não fica armazenada no Certificado Digital. (Letra E).

(MPE/AL – 2018) Assinale abaixo o instrumento tecnológico que permite a identificação segura do autor de uma mensagem ou documento em uma rede de computadores.

a) Biometria.
b) Cartão inteligente.
c) Certificado digital.
d) PIN.
e) Token de segurança.
_______________________ Comentários: conforme vimos em aula, trata-se do Certificado Digital. Ele permite a identificação segura do autor, porque contém sua chave pública (Letra C).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








48
84



(CASSE/MS – 2016) Ao receber uma mensagem eletrônica, deve-se fazer a verificação da assinatura digital. Nas alternativas, assinale a que indica a resposta correta para se efetuar esse procedimento.

a) Ter acesso ao CPF e identidade do remetente.
b) Ter acesso ao certificado digital do remetente.
c) Ter acesso ao certificado digital do destinatário.
d) Ter acesso à chave criptográfica dupla do destinatário.
_______________________ Comentários: conforme vimos em aula, deve-se ter acesso ao Certificado Digital do remetente (Letra B).

































Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








49
84



3.4.2 – Infraestrutura de Chave Pública (ICP-Brasil) INCIDÊNCIA EM PROVA: média 
Nós  vimos  que  uma  Autoridade  Certificadora  é  responsável  por  –  entre  outras  atividades  – emitir certificados digitais . No entanto, nós vimos que ela também possui um certificado digital contendo sua chave pública. E quem emite o certificado digital para essa Autoridade Certificadora?
Pois  é,  nós  precisamos  de  outra  parte  confiável!  Para  tal,  existem  as  Infraestruturas  de  Chave Pública
3
(ICP). O que é isso, Diego?

Trata-se de uma entidade pública ou privada que tem como objetivo manter uma estrutura de emissão  de  chaves  públicas , baseando-se no princípio da terceira parte confiável e oferecendo uma mediação de credibilidade e confiança em transações entre partes que utilizem certificados digitais. O Certificado Digital funcionará como uma identidade virtual que permite a identificação segura e inequívoca do autor de uma mensagem ou transação.

A principal função da ICP é definir um conjunto de técnicas, práticas e procedimentos a serem adotados pelas entidades a fim de estabelecer um sistema de certificação digital baseado em chave  pública.  A  ICP  brasileira  –  definida  pela  MP  2200-2  –  é  denominada  ICP-Brasil.  Nesta infraestrutura,  há  duas  entidades:  Autoridades  Certificadoras  e  Autoridades  de  Registro,  que emitem e vendem certificados digitais respectivamente. Vejam a cadeia de certificação:



3
Em inglês, Public Key Infrastructure (PKI).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








50
84




Sabe quando vamos tirar a carteira de identidade? Pois é, a maioria das pessoas procura a Secretaria de Segurança Pública (SSP), que é responsável por expedir um documento oficial de identificação atestando quem você realmente é – seria análogo a uma Autoridade Certificadora de Nível 1. Ela está subordinada ao Ministério da Justiça, análogo a Autoridade Certificadora Raiz. Já o Instituto de Identificação da SSP seria a Autoridade de Registro.



 Autoridade Certificadora Raiz 
Trata-se  da  primeira  autoridade  da  cadeia  de  certificação.  Ela  é  responsável  por  executar  as políticas de certificados e as normas técnicas e operacionais aprovadas pelo Comitê Gestor da ICP- Brasil.
Dessa  forma,  compete  à  AC-Raiz  emitir,  expedir,  distribuir,  revogar  e  gerenciar  os certificados das autoridades certificadoras de nível imediatamente subsequente ao seu – isso costuma cair em prova.


A  AC-Raiz também  está  encarregada  de  emitir  a  Lista  de  Certificados  Revogados  (LCR) e de fiscalizar e auditar as Autoridades Certificadoras – ACs, Autoridades de Registro – ARs e demais prestadores de serviço habilitados na ICP-Brasil. Além disso, ela é responsável por verificar se as ACs  estão  atuando  em  conformidade  com  as  diretrizes  e  normas  técnicas  estabelecidas  pelo Comitê Gestor da ICP-Brasil.

 Autoridade Certificadora 
Trata-se  de  uma  entidade,  pública  ou  privada,  subordinada  à  hierarquia  da  ICP-Brasil, responsável  por  emitir,  distribuir,  renovar,  revogar  e  gerenciar  certificados  digitais.  Busca verificar se o titular do certificado possui a chave privada que corresponde à chave pública do certificado. Ela cria e assina digitalmente o certificado do assinante, onde o certificado emitido pela AC representa a declaração da identidade do titular, que possui um par único de chaves.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








51
84



Cabe  também  à  Autoridade  Certificadora  emitir  Listas  de  Certificados  Revogados  (LCR) e manter registros de suas operações sempre obedecendo às práticas definidas na Declaração de Práticas de Certificação – DPC. Além de estabelecer e fazer cumprir, pelas Autoridades de Registro –  ARs  a  ela  vinculadas,  as  políticas  de  segurança  necessárias  para  garantir  a  autenticidade  da identificação realizada.

 Autoridade de Registro 
Trata-se  de  uma  entidade  responsável  pela interface  entre  o  usuário  e  a  Autoridade Certificadora.  Vinculada  a  uma  AC,  tem  por objetivo   o
recebimento,    a    validação,    o encaminhamento de solicitações de emissão ou revogação de certificados digitais e identificação,   de   forma   presencial,   de   seus solicitantes
.  É  responsabilidade  da  AR  manter registros   de   suas   operações.  Pode   estar fisicamente  localizada  em  uma  AC  ou  ser  uma entidade de registro remota. A imagem ao lado mostra um exemplo de organização.

Em  suma:  a  Autoridade  Certificadora  Raiz  emite  certificados  digitais  para  as  Autoridades Certificadoras hierarquicamente abaixo dela, que emitem certificados para equipamentos, pessoas físicas ou jurídicas.
As Autoridades de Registro não emitem certificados digitais. Elas o recebem, validam ou encaminham e guardam um registro dessas operações. Quem emite certificado para pessoas físicas? Apenas a Autoridade Certificadora!

É importante ressaltar que existe um padrão para Infraestrutura de Chaves Públicas!
O  Padrão
X.509  (Versão  3)  especifica,  entre  outras  coisas,  o  formato  dos  certificados  digitais ,  de  tal
maneira que se possa amarrar firmemente um nome a uma chave pública, permitindo autenticação forte. Esse é o padrão utilizado pela ICP-Brasil! Por fim, vamos falar um pouquinho sobre Cadeia ou Teia de Confiança (Web of Trust). O que é isso, Diego?


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








52
84




Trata-se  de  um  modelo  de  confiança  transitiva  descentralizada,  que  busca  disponibilizar criptografia para o público geral sem custos.
Para tal, a confiança vai sendo estabelecida através de uma rede de transitividade em que, se Tony confia em Mike e Mike confia em John, então Tony confia em John. Essa rede é construída por meio de uma relação pessoal indivíduos através da assinatura de chave pública de um usuário pelo outro e assim sucessivamente.

Essas etapas acabam por gerar um laço de confiança que se converte, então, em uma rede, teia ou cadeia de confiança, como é apresentado ao lado. Hora de praticar...

(TRF/2 – 2017) “O certificado digital ICP-Brasil funciona como uma identidade virtual que permite a identificação segura e inequívoca do autor de uma mensagem ou transação feita em meios eletrônicos, como a web”.
(Sítio do Instituto Nacional de Tecnologia da Informação. Disponível em: http://www.iti.gov.br/certificacao-digital/o-que-e).

Referente à certificação digital, assinale a alternativa correta.

a) A Autoridade Certificadora Raiz é quem emite os certificados para o usuário final.
b) A criptografia simétrica utiliza duas chaves distintas: chave privada e chave pública.
c) A Autoridade Certificadora é a primeira autoridade da cadeia de certificação da ICP- Brasil.
d) O Instituto Nacional de Tecnologia da Informação é a Autoridade Certificadora Raiz da Infra-Estrutura de Chaves Públicas Brasileira.
_______________________ Comentários: (a) Errado, Autoridade Certificadora Raiz emite certificados para Autoridades Certificadores hierarquicamente abaixo; (b) Errado, essa é a Criptografia Assimétrica; (c) Errado, essa é a Autoridade Certificadora Raiz; (d) Correto, ITI é a AC- Raiz do ICP-Brasil (Letra D).

(TJDFT  –  2015) As entidades denominadas certificadoras são entidades reconhecidas pela ICP Brasil (Infraestrutura de Chaves Públicas) e autorizadas a emitir certificados digitais para usuários ou instituições que desejam utilizá-los.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita – elas emitem certificados para usuários ou instituições. AR e AC-Raiz não o fazem (Correto).









Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








53
84



3.4.3 – Tipos de Certificado INCIDÊNCIA EM PROVA: média 
Os  certificados  digitais  da  Categoria  A  costumam  ser  usados  para  fins  de  identificação  e autenticação. Você pode usá-los para assinar documentos ou validar transações eletrônicas. Já a Categoria S é direcionada a atividades sigilosas, como a proteção de arquivos confidenciais.

 Certificado de Assinatura Digital (A): reúne os certificados de assinatura digital, utilizados na confirmação  de  identidade  na  web,  em  e-mails,  em  Redes  Privadas  Virtuais  (VPNs)  e  em documentos eletrônicos com verificação da integridade das informações.

 Certificado  de  Sigilo  (S): reúne os certificados de sigilo, que são utilizados na codificação de documentos, de bases de dados relacionais, de mensagens e de outras informações eletrônicas sigilosas.

TIPO

GERAÇÃO DO PAR DE
CHAVE PÚBLICA/PRIVADA 
TAMANHO
MÍNIMO DA
CHAVE (BITS)
ARMAZENAMENTO
VALIDADE
(ANOS)
Certificado A1/S1 Por software 1024 Disco Rígido (HD) e Pendrive 1 Certificado A2/S2 Por software 1024 SmartCard (com chip) ou Token USB 2 Certificado A3/S3 Por hardware 1024 SmartCard (com chip) ou Token USB 5 Certificado A4/S4 Por hardware 2048 SmartCard (com chip) ou Token USB 6 
(SEFAZ/PE  –  2014) Duas séries de certificados previstos na ICP-Brasil são descritas a seguir:

I. Reúne os certificados de assinatura digital, utilizados na confirmação de identidade na web, em e-mails, em Redes Privadas Virtuais (VPNs) e em documentos eletrônicos com verificação da integridade das informações.

II. Reúne os certificados de sigilo, que são utilizados na codificação de documentos, de bases de dados, de mensagens e de outras informações eletrônicas sigilosas.

As séries de certificados I e II são categorizadas, respectivamente, de:

a) B e C.
b) A e B.
c) B e D.
d) A e F.
e) A e S.
_______________________ Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








54
84



Comentários: (I) conforme vimos em aula, trata-se dos Certificados de Assinatura Digital (A); (II) conforme vimos em aula, trata- se dos Certificados de Sigilo (S); (Letra E).

(SEFAZ/PI  –  2015) Considere  o  texto  a  seguir  retirado  do  portal  da  Secretaria  da Fazenda:

O certificado digital utilizado na Nota Fiscal Eletrônica (NF-e) deverá ser adquirido junto à Autoridade Certificadora credenciada pela Infraestrutura de Chaves Públicas Brasileira -  ICP-Brasil,  devendo  ser  do  tipo  ...  I...  ou  .... II...  e  conter  o  CNPJ  de  um  dos estabelecimentos da empresa.

(http://www.nfe.fazenda.gov.br/PORTAL/perguntasFrequentes.aspx?tipoConteudo=k/E5BakB80o=) 
As características dos certificados digitais I e II são descritas a seguir:

I. A chave privada é armazenada no disco rígido do computador, que também é utilizado para realizar a assinatura digital.
II. A chave privada é armazenada em dispositivo portátil inviolável do tipo smart card ou token, que possui um chip com capacidade de realizar a assinatura digital.

I e II são, respectivamente, 
a) S1 e S2.
b) A2 e A3.
c) S1 e S3.
d) A2 e A4.
e) A1 e A3.
_______________________ Comentários: Observem que ambos são utilizados para assinatura digital, logo só podem ser do Tipo A. Sobram as opções B, D e E! Em (I), a chave é armazenada no disco rígido do computador, logo só pode ser A1/S1. Sobra apenas a última opção (Letra E).













Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








55
84



RESUMO

PRINCÍPIOS DE SEGURANÇA DESCRIÇÃO Confidencialidade
Capacidade de um sistema de não permitir que informações estejam disponíveis ou sejam reveladas a entidades não autorizadas – incluindo usuários, máquinas, sistemas ou processos.
Integridade
Capacidade de garantir que a informação manipulada está correta, fidedigna e que não foi corrompida – trata da salvaguarda da exatidão e completeza da informação.
Disponibilidade
Propriedade de uma informação estar acessível e utilizável sob demanda por uma entidade autorizada.

PRINCÍPIOS ADICIONAIS DESCRIÇÃO Autenticidade
Propriedade que trata da garantia de que um usuário é de fato quem alega ser. Em outras palavras, ela garante a identidade de quem está enviando uma determinada informação.
Irretratabilidade
Também chamada de Irrefutabilidade ou Não-repúdio, trata da capacidade de garantir que o emissor da mensagem ou participante de um processo não negue posteriormente a sua autoria.

TIPO DE CRIPTOGRAFIA DESCRIÇÃO Criptografia Simétrica (Chave Secreta)
Utiliza um algoritmo e uma única chave secreta para cifrar/decifrar que tem que ser mantida em segredo.

Criptografia Assimétrica (Chave Pública)
Utiliza um algoritmo e um par de chaves para cifrar/decifrar – uma pública e a outra tem que ser mantida em segredo.
Criptografia Híbrida (Chave Pública/Secreta) Utiliza um algoritmo de chave pública apenas para trocar chaves simétricas – chamadas chaves de sessão – de forma segura. Após a troca, a comunicação é realizada utilizando criptografia simétrica.

CRIPTOGRAFIA ASSIMÉTRICA UTILIZADA PARA GARANTIR O PRINCÍPIO DA CONFIDENCIALIDADE
CRIPTOGRAFIA ASSIMÉTRICA UTILIZADA PARA GARANTIR O PRINCÍPIO DA AUTENTICIDADE


O  emissor  criptografa  o  texto  original  com  a  chave pública  do receptor de forma que somente ele consiga descriptografá-lo com sua chave privada para visualizar o texto original.
O emissor criptografa o texto original com sua chave privada de forma que o receptor possa descriptografá-lo com a chave pública do emissor.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








56
84



MÉTODOS DE AUTENTICAÇÃO DESCRIÇÃO O QUE VOCÊ SABE?
Trata-se  da autenticação  baseada no conhecimento  de  algo que  somente você  sabe,  tais como:
senhas, frases secretas, dados pessoais aleatórios, entre outros.
O QUE VOCÊ É?
Trata-se  da  autenticação  baseada  no  conhecimento  de  algo  que  você  é,  como  seus  dados biométricos.
O QUE VOCÊ TEM?
Trata-se  da autenticação  baseada em algo  que  somente  o verdadeiro usuário  possui,  tais como:
celulares, crachás, Smart Cards, chaves físicas, tokens, etc.

AUTENTICAÇÃO FORTE
Trata-se de um tipo de autenticação que ocorre quando se utiliza pelo menos dois desses três métodos de autenticação. Um exemplo é a Autenticação em Dois Fatores (ou Verificação em Duas Etapas).

ASSINATURA DIGITAL
Trata-se de um método de autenticação de informação digital tipicamente tratada como substituta à assinatura física, já que elimina a necessidade de ter uma versão em papel do documento que necessita ser assinado. Por meio de um Algoritmo de Hash, é possível garantir a integridade dos dados.



FUNCIONAMENTO da assinatura digital Maria possui uma mensagem em claro (sem criptografia). Ela gera um hash dessa mensagem, depois criptografa esse hash utilizando sua chave privada. Em seguida, ela envia para João tanto a mensagem original quanto o seu hash. João gera um hash da mensagem original e obtém um resultado. Depois descriptografa o hash da mensagem utilizando a chave pública de Maria e obtém outro resultado.
Dessa forma, ele tem dois hashes para comparar: o que ele gerou a partir da mensagem em claro e o que ele descriptografou a partir da mensagem criptografada. Se forem iguais, significa que Maria realmente enviou a mensagem, significa que ela não pode negar que enviou o documento e, por fim, significa que o documento está íntegro. E essa é a Assinatura Digital baseada em Hash – ela não se preocupa com a confidencialidade, qualquer um pode visualizar a mensagem. Nós garantimos assim a Autenticidade e a Integridade!
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








57
84



Mas cadê a irretratabilidade ou não repúdio? Para garantir a irretratabilidade ou não-repúdio, deve-se adicionar mais um passo! No início do processo, Maria criptografa a mensagem com a sua chave privada e depois criptografa o resultado com a chave pública de João.
Quando João receber, ele descriptografa o arquivo com sua chave privada e depois descriptografa o resultado com a chave pública de Maria.

Certificado digital
Certificado  Digital  é  um  documento  eletrônico  assinado  digitalmente  por  uma  terceira  parte  confiável  –  chamada  Autoridade Certificadora – e que cumpre a função de associar uma entidade (pessoa, processo, servidor) a um par de chaves criptográficas com o intuito  de  tornar  as  comunicações  mais  confiáveis  e  auferindo  maior  confiabilidade  na  autenticidade.  Ele  é  capaz  de  garantir  a autenticidade, integridade e não-repúdio, e até confidencialidade.

TIPO DESCRIÇÃO
Certificado A1/S1
Geração do par de chaves pública/privada feita por software; chaves de tamanho mínimo de 1024 bits;
armazenamento em dispositivo como disco rígido e pendrive; validade máxima de um ano;
Certificado A2/S2
Geração do par de chaves pública/privada feita por software; chaves de tamanho mínimo de 1024 bits;
armazenamento em Smart Card (com chip) ou Token USB; validade máxima de dois anos;
Certificado A3/S3
Geração do par de chaves pública/privada feita por hardware; chaves de tamanho mínimo de 1024 bits;
armazenamento em Smart Card (com chip) ou Token USB; validade máxima de cinco anos.
Certificado A4/S4
Geração do par de chaves pública/privada feita por hardware; chaves de tamanho mínimo de 2048 bits;
armazenamento em Smart Card (com chip) ou Token USB; validade máxima de seis anos.























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








58
84



MAPA MENTAL

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








59
84




Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








60
84



QUESTÕES COMENTADAS - FCC 
1. (FCC  /  TRE  SP  –  2017) Transações, comunicações e serviços realizados por meio da internet devem  obedecer  a  determinadas  regras  de  segurança  da  informação.  Na  área  pública, principalmente, alguns cuidados são necessários para garantir que as informações sigilosas não sejam acessadas por entidades inescrupulosas ou mal-intencionadas (uma entidade pode ser, por  exemplo,  uma  pessoa,  uma  empresa  ou  um  programa  de  computador).  Dentre  os mecanismos de segurança existentes, o que visa à integridade:

a) verifica se a entidade é realmente quem ela diz ser.
b) protege a informação contra alteração não autorizada.
c) determina as ações que a entidade pode executar.
d) protege uma informação contra acesso não autorizado.
e) garante que um recurso esteja disponível sempre que necessário.

Comentários:

(a) Errado, trata-se do princípio da autenticidade; (b) Correto, trata-se do princípio da integridade;
(c) Errado, trata-se da autorização; (d) Errado, trata-se do princípio da confidencialidade; (e) Errado, trata-se do princípio da disponibilidade.

Gabarito: Letra B

2. (FCC / TRF 5ª Região – 2017) Josué, Técnico de Segurança do Tribunal, sem solicitar autorização de seu superior, altera os procedimentos de segurança de acesso ao Tribunal, por entender que aquelas  alterações  seriam  mais  eficazes.  Tampouco  reporta  tal  alteração,  o  que  acaba acarretando transtornos pois o novo procedimento não foi incorporado corretamente à rotina daquele local, sendo que o departamento de segurança e sua chefia não ficaram cientes de tal alteração.

A característica básica da segurança das informações que Josué feriu é a:

a) confidencialidade.
b) integridade.
c) disponibilidade.
d) confiabilidade.
e) continuidade.

Comentários:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








61
84



Quando Josué modifica os procedimentos de segurança do Tribunal sem autorização, ele viola o princípio da Integridade. Claro que isso pode gerar consequências em relação à disponibilidade, confidencialidade, entre outros – no entanto, Josué em si fere apenas a integridade dos dados.

Gabarito: Letra B

3. (FCC / TRT 20ª Região – 2016) Considere as duas situações em que a proteção e a segurança da informação foram violadas:

I. O número do CPF de um trabalhador foi alterado, deixando seu CPF inválido.

II. Um dado sigiloso de uma causa trabalhista foi acessado por uma pessoa não autorizada.

Nas situações I e II ocorreram, respectivamente, violação da:

a) autenticação e da autorização das informações.
b) confidencialidade e da integridade das informações.
c) confidencialidade e da disponibilidade das informações.
d) identificação e da autorização das informações.
e) integridade e da confidencialidade das informações.

Comentários:

Na Situação  I,  a  informação  (Número  do  CPF)  foi  alterada/corrompida,  violando  –  assim  –  o Princípio da Integridade.

Na Situação  II,  a  informação  sigilosa  foi  violada  e  acessada  por um  terceiro  não  autorizado, violando assim o Princípio da Confidencialidade.

Gabarito: Letra E

4. (FCC / TRE RR – 2015) O processo de proteção da informação das ameaças caracteriza- se como Segurança da Informação. O resultado de uma gestão de segurança da informação adequada deve oferecer suporte a cinco aspectos principais:

I. Somente as pessoas autorizadas terão acesso às informações.

II. As informações serão confiáveis e exatas. Pessoas não autorizadas não podem alterar os dados.

III. Garante o acesso às informações, sempre que for necessário, por pessoas autorizadas.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








62
84



IV. Garante que em um processo de comunicação os remetentes não se passem por terceiros e nem que a mensagem sofra alterações durante o envio.

V. Garante que as informações foram produzidas respeitando a legislação vigente.

Os aspectos elencados de I a V correspondem, correta e respectivamente, a:

a) integridade − disponibilidade − confidencialidade − autenticidade − legalidade.
b) disponibilidade − confidencialidade − integridade − legalidade − autenticidade.
c) confidencialidade − integridade − disponibilidade − autenticidade − legalidade.
d) autenticidade − integridade − disponibilidade − legalidade − confidencialidade.
e) autenticidade − confidencialidade − integridade − disponibilidade − legalidade.

Comentários:

(I)  Esse  é  o  Princípio  da  Confidencialidade;  (II)  Esse  é  o  Princípio  da  Integridade;  (III)  Esse  é  o Princípio da Disponibilidade; (IV) Esse é o Princípio da Autenticidade; (V) Esse é o Princípio da Legalidade.

Gabarito: Letra C

5. (FCC  /  TRE  RR  –  2015) Quando se trata da segurança das informações trocadas entre duas pessoas, a criptografia garante ..I.. e a função hash permite verificar a ..II.. da mensagem.

As lacunas I e II são preenchidas, correta e respectivamente, com:

a) a confidencialidade − integridade.
b) a integridade − disponibilidade.
c) a confidencialidade − disponibilidade.
d) o não repúdio − integridade.
e) a autenticidade − irretratabilidade.

Comentários:


A criptografia é um método que codifica os dados do usuário para que só o destinatário possa ler, dessa maneira garantindo a confidencialidade da informação.

A Função de Hash é um método de criptografia que transforma uma entrada de tamanho qualquer em  uma  saída  de  tamanho  fixo,  chamado  de hash,  de  maneira  que  não  é  possível  obter  a informação  original  a  partir  do hash.  É  bastante  utilizado  para  garantir  a integridade da
informação, calculando o hash antes e depois da transmissão para fins de comparação.

Gabarito: Letra A
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








63
84




6. (FCC / SEFAZ RJ – 2014) A política de segurança da informação da Receita Estadual inclui um conjunto  de  diretrizes  que  determinam  as  linhas  mestras  que  devem  ser  seguidas  pela instituição  para  que  sejam  assegurados  seus  recursos  computacionais  e  suas  informações.
Dentre estas diretrizes encontram-se normas que garantem 
I. a fidedignidade de informações, sinalizando a conformidade dos dados armazenados com relação às inserções, alterações e processamentos autorizados efetuados. Sinalizam, ainda, a conformidade  dos  dados  transmitidos  pelo  emissor  com  os  recebidos  pelo  destinatário, garantindo a não violação dos dados com intuito de alteração, gravação ou exclusão, seja ela acidental ou proposital.

II. que as informações estejam acessíveis às pessoas e aos processos autorizados, a qualquer momento  requerido,  assegurando  a  prestação  contínua  do  serviço,  sem  interrupções  no fornecimento de informações para quem é de direito.

III.  que  somente  pessoas  autorizadas  tenham  acesso às  informações  armazenadas  ou transmitidas por meio das redes de comunicação, assegurando que as pessoas não tomem conhecimento de informações, de forma acidental ou proposital, sem que possuam autorização para tal procedimento.

Em relação às informações, as normas definidas em I, II e III visam garantir:

a) fidedignidade, acessibilidade e disponibilidade.
b) integridade, disponibilidade e confidencialidade.
c) confidencialidade, integridade e autenticidade.
d) integridade, ininterruptibilidade e autenticidade.
e) confidencialidade, integridade e disponibilidade.

Comentários:

O item I está relacionado à integridade da informação, que visa garantir que a informação não será perdida ou modificada por alguém não autorizado.

O item II está relacionado à disponibilidade da informação, que visa garantir que a informação estará sempre acessível.

O  item  III  está  relacionado  à confidencialidade,  que  visa  garantir  que  a  informação  não  seja acessada por alguém não autorizado.

Gabarito: Letra B

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








64
84



7. (FCC / TRT 16ª Região – 2014) Diversos mecanismos de segurança foram desenvolvidos para prover e garantir proteção da informação que, quando corretamente configurados e utilizados, podem auxiliar os usuários a se protegerem dos riscos envolvendo o uso da Internet. Os serviços disponibilizados e as comunicações realizadas pela internet devem garantir os requisitos básicos de segurança e proteção da informação, como:

- Identificação: permitir que uma entidade se identifique, ou seja, diga quem ela é.
- I. Verificar se a entidade é realmente quem ela diz ser.
- II. Determinar as ações que a entidade pode executar.
- III. Proteger a informação contra alteração não autorizada.
- IV. Proteger a informação contra acesso não autorizado.
- V. Evitar que uma entidade possa negar que foi ela que executou uma ação.
- Disponibilidade: garantir que um recurso esteja disponível sempre que necessário.

As definições numeradas de I a V correspondem, respectivamente, a:

a) Integridade; Autenticação; Autorização; Acessabilidade; Não repúdio.
b) Identificação; Raio de Ação; Autorização; Acessabilidade; Negação.
c) Autenticação; Autorização; Integridade; Confidencialidade; Não repúdio.
d) Autenticação; Raio de Ação; Integridade; Confidencialidade; Identificação.
e) Integridade; Confidencialidade; Autenticação; Autorização; Negação.

Comentários:

(I)  Trata-se  da  Autenticidade/Autenticação;  (II)  Trata-se  da  Autorização;  (III)  Trata-se  da Integridade; (IV) Trata-se da Confidencialidade; (V) Trata-se do Não-repúdio.

Lembrando que
Autorização é a definição do controle de acesso e das ações que cada tipo de usuário pode executar em um sistema.

Gabarito: Letra C

8. (FCC  /  DPE  RS  –  2013)  NÃO  está  associada  ao  conceito  de  preservação  da segurança  da informação a:

a) integridade.
b) autenticidade.
c) aplicabilidade.
d) disponibilidade.
e) confidencialidade.

Comentários:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








65
84



Conforme vimos em aula, são princípios a confidencialidade, integridade e disponibilidade – além da  autenticidade  e  irretratabilidade.  A  aplicabilidade não  é  um  princípio  da  segurança  da informação.

Gabarito: Letra C

9. (FCC  /  SABESP  –  2017)  A  criptografia  de  chave  pública  utiliza  duas  chaves  distintas:  uma pública,  que  poderá  ser  livremente  divulgada,  e  uma  privada,  que  deverá  ser  mantida  em segredo por seu dono. Quando uma informação é codificada com uma das chaves, somente a outra chave do par poderá decodificá-la. Qual chave usar para codificar depende da proteção que  se  deseja,  se  confidencialidade  ou  autenticação,  integridade  ou  não  repúdio.  A  chave privada poderá ser armazenada de diferentes maneiras, como um arquivo no computador, um smartcard ou um token.

(Adaptado de: http://cartilha.cert.br/criptografia/) 
Se um Estagiário tiver que selecionar um método criptográfico que usa chave pública, poderá selecionar o:

a) AES.
b) RSA.
c) RC4.
d) 3DES.
e) Blowfish.

Comentários:

Na criptografia
simétrica existe apenas uma chave, que permite a codificação e decodificação da mensagem, ou seja, a mesma chave transforma o texto claro em cifra e a cifra em texto claro.

Na criptografia
assimétrica existe um par de chaves, uma chave  pública e uma  chave  privada.
Quando o texto é codificado com uma das chaves, somente seu par pode decodificar.

Gabarito: Letra B

10. (FCC  /  SEFAZ  RJ  –  2014) A Receita Federal do Brasil (RFB) publicou em seu site a seguinte determinação:

É obrigatória a utilização de ......, para apresentação de declarações à RFB, por todas as pessoas jurídicas, exceto as optantes pelo Simples Nacional. As pessoas físicas não estão obrigadas à sua utilização.  As  autoridades  certificadoras  (AC)  não possuem  capacidade  de  atendimento  de demanda  ilimitada.  Assim,  é  conveniente  que  as  empresas  não  deixem  para  fazer  a  sua aquisição na última hora.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








66
84



Atenção! As entidades sem fins lucrativos também estão obrigadas à entrega de declarações e demonstrativos com a sua utilização, de acordo com a legislação pertinente a cada assunto.

(Adaptado de: http://www.receita.fazenda.gov.br/atendvirtual/orientacoes/obrigatoriedadecd.htm) 
Preenche corretamente a lacuna:

a) assinatura digital autenticada.
b) certificado digital válido.
c) certificado digital autenticado pela RFB.
d) assinatura e certificado digitais emitidos pela AC-raiz.
e) assinatura e certificado digitais autenticados pela RFB.

Comentários:

(a)  Errado.  Assinaturas  Digitais  não  são  adquiridas  por  Autoridades  Certificadoras,  elas  são produzidas pelo remetente; (b) Correto. Um certificado digital válido garante que a autenticidade de  qualquer  documento  assinado  utilizando  as  chaves  relacionadas  ao  certificado.  Assim,  há  a garantia de que o remetente de uma declaração é realmente a pessoa responsável por ela; (c) Errado. A ICP-BR composta de várias autoridades certificadoras. Um certificado digital autenticado por qualquer uma delas possui validade legal; (d) Errado. A assinatura é produzida pelo detentor de um par de chaves e o certificado digital deve ser emitido por uma AC de primeiro nível ou inferior;
(e) Errado. Não há obrigatoriedade de ser autenticada pela RFB.

Gabarito: Letra B

11. (FCC / SEFAZ RJ – 2014) Considere:

- Funciona como uma impressão digital de uma mensagem, gerando, a partir de uma entrada de tamanho variável, um valor fixo pequeno.

- Este valor está para o conteúdo da mensagem assim como o dígito verificador de uma conta- corrente está para o número da conta ou o check sum está para os valores que valida.

- É utilizado para garantir a integridade do conteúdo da mensagem que representa.

- Ao ser utilizado, qualquer modificação no conteúdo da mensagem será detectada, pois um novo cálculo do seu valor sobre o conteúdo modificado resultará em um valor bastante distinto.

Os itens acima descrevem:

a) um Certificado digital b) uma Assinatura digital c) um Algoritmo de chave pública Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








67
84



d) um Algoritmo de chave secreta e) um Hash criptográfico 
Comentários:

A função hash
é um método de criptografia que transforma os dados em um texto de tamanho único, chamado de hash, de maneira que não seja possível obter a informação original a partir do hash. É bastante utilizado para garantir a integridade da informação, calculando o hash antes e depois da transmissão para fins de comparação.

Gabarito: Letra E

12. (FCC / Prefeitura de São Paulo – 2012) Considere a frase a seguir.

Na  criptografia  ..I..  ,  um  emissor  codifica  seu  documento  com  a  chave  ..II..  da  pessoa  que receberá a mensagem. O texto codificado apenas poderá ser decodificado pelo ..III.. , pois, somente ele tem a chave ..IV.. relacionada à chave ..V.. que originou o texto cifrado.

As lacunas I, II, III, IV e V devem ser preenchidas, correta e respectivamente, por 
a) de chaves públicas, privada, destinatário, pública e privada.
b) assimétrica, privada, emissor, pública e privada.
c) simétrica, pública, emissor, privada e pública.
d) assimétrica, pública, destinatário, privada e pública.
e) simétrica, privada, destinatário, pública e privada.

Comentários:

Na criptografia simétrica existe apenas uma chave, que permite a codificação e decodificação da mensagem, ou seja, a mesma chave transforma o texto claro em cifra e a cifra em texto claro. Na criptografia assimétrica existe um par de chaves, uma chave pública e uma chave privada. Quando o texto é codificado com uma das chaves, somente seu par pode decodificar.

Para resolver a questão, como se fala de chaves públicas e privadas, estamos falando de criptografia assimétrica,  eliminando  as  alternativas  C  e  E.    Além  disso,  normalmente,  cada  usuário  possui apenas a sua própria chave privada, e não a de outros usuários, ou seja, o emissor possui apenas a chave pública do destinatário. Isso elimina as alternativas A e B.

Gabarito: Letra D

13. (FCC / Prefeitura de São Paulo – 2012) A assinatura digital é o resultado da aplicação de uma função matemática que gera uma espécie de impressão digital de uma mensagem. O primeiro Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








68
84



passo no processo de assinatura digital de um documento eletrônico é a aplicação dessa função, que fornece uma sequência única para cada documento conhecida como "resumo".

A função matemática citada é mais conhecida como função:

a) quântica.
b) de Hash.
c) quadrática.
d) de Euler.
e) binária.

Comentários:

A questão trata da Função de Hash! Ela é basicamente um algoritmo criptográfico que transforma uma entrada de dados em uma saída de dados.

Gabarito: Letra B
























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








69
84



LISTA DE QUESTÕES - FCC 
1. (FCC  /  TRE  SP  –  2017) Transações, comunicações e serviços realizados por meio da internet devem  obedecer  a  determinadas  regras  de  segurança  da  informação.  Na  área  pública, principalmente, alguns cuidados são necessários para garantir que as informações sigilosas não sejam acessadas por entidades inescrupulosas ou mal-intencionadas (uma entidade pode ser, por  exemplo,  uma  pessoa,  uma  empresa  ou  um  programa  de  computador).  Dentre  os mecanismos de segurança existentes, o que visa à integridade:

a) verifica se a entidade é realmente quem ela diz ser.
b) protege a informação contra alteração não autorizada.
c) determina as ações que a entidade pode executar.
d) protege uma informação contra acesso não autorizado.
e) garante que um recurso esteja disponível sempre que necessário.

2. (FCC / TRF 5ª Região – 2017) Josué, Técnico de Segurança do Tribunal, sem solicitar autorização de seu superior, altera os procedimentos de segurança de acesso ao Tribunal, por entender que aquelas  alterações  seriam  mais  eficazes.  Tampouco  reporta  tal  alteração,  o  que  acaba acarretando transtornos pois o novo procedimento não foi incorporado corretamente à rotina daquele local, sendo que o departamento de segurança e sua chefia não ficaram cientes de tal alteração.

A característica básica da segurança das informações que Josué feriu é a:

a) confidencialidade.
b) integridade.
c) disponibilidade.
d) confiabilidade.
e) continuidade.

3. (FCC / TRT 20ª Região – 2016) Considere as duas situações em que a proteção e a segurança da informação foram violadas:

I. O número do CPF de um trabalhador foi alterado, deixando seu CPF inválido.

II. Um dado sigiloso de uma causa trabalhista foi acessado por uma pessoa não autorizada.

Nas situações I e II ocorreram, respectivamente, violação da:

a) autenticação e da autorização das informações.
b) confidencialidade e da integridade das informações.
c) confidencialidade e da disponibilidade das informações.
d) identificação e da autorização das informações.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








70
84



e) integridade e da confidencialidade das informações.

4. (FCC / TRE RR – 2015) O processo de proteção da informação das ameaças caracteriza- se como Segurança da Informação. O resultado de uma gestão de segurança da informação adequada deve oferecer suporte a cinco aspectos principais:

I. Somente as pessoas autorizadas terão acesso às informações.

II. As informações serão confiáveis e exatas. Pessoas não autorizadas não podem alterar os dados.

III. Garante o acesso às informações, sempre que for necessário, por pessoas autorizadas.

IV. Garante que em um processo de comunicação os remetentes não se passem por terceiros e nem que a mensagem sofra alterações durante o envio.

V. Garante que as informações foram produzidas respeitando a legislação vigente.

Os aspectos elencados de I a V correspondem, correta e respectivamente, a:

a) integridade − disponibilidade − confidencialidade − autenticidade − legalidade.
b) disponibilidade − confidencialidade − integridade − legalidade − autenticidade.
c) confidencialidade − integridade − disponibilidade − autenticidade − legalidade.
d) autenticidade − integridade − disponibilidade − legalidade − confidencialidade.
e) autenticidade − confidencialidade − integridade − disponibilidade − legalidade.

5. (FCC  /  TRE  RR  –  2015) Quando se trata da segurança das informações trocadas entre duas pessoas, a criptografia garante ..I.. e a função hash permite verificar a ..II.. da mensagem.

As lacunas I e II são preenchidas, correta e respectivamente, com:

a) a confidencialidade − integridade.
b) a integridade − disponibilidade.
c) a confidencialidade − disponibilidade.
d) o não repúdio − integridade.
e) a autenticidade − irretratabilidade.

6. (FCC / SEFAZ RJ – 2014) A política de segurança da informação da Receita Estadual inclui um conjunto  de  diretrizes  que  determinam  as  linhas  mestras  que  devem  ser  seguidas  pela instituição  para  que  sejam  assegurados  seus  recursos  computacionais  e  suas  informações.
Dentre estas diretrizes encontram-se normas que garantem 
I. a fidedignidade de informações, sinalizando a conformidade dos dados armazenados com relação às inserções, alterações e processamentos autorizados efetuados. Sinalizam, ainda, a Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








71
84



conformidade  dos  dados  transmitidos  pelo  emissor  com  os  recebidos  pelo  destinatário, garantindo a não violação dos dados com intuito de alteração, gravação ou exclusão, seja ela acidental ou proposital.

II. que as informações estejam acessíveis às pessoas e aos processos autorizados, a qualquer momento  requerido,  assegurando  a  prestação  contínua  do  serviço,  sem  interrupções  no fornecimento de informações para quem é de direito.

III.  que  somente  pessoas  autorizadas  tenham  acesso às  informações  armazenadas  ou transmitidas por meio das redes de comunicação, assegurando que as pessoas não tomem conhecimento de informações, de forma acidental ou proposital, sem que possuam autorização para tal procedimento.

Em relação às informações, as normas definidas em I, II e III visam garantir:

a) fidedignidade, acessibilidade e disponibilidade.
b) integridade, disponibilidade e confidencialidade.
c) confidencialidade, integridade e autenticidade.
d) integridade, ininterruptibilidade e autenticidade.
e) confidencialidade, integridade e disponibilidade.

7. (FCC / TRT 16ª Região – 2014) Diversos mecanismos de segurança foram desenvolvidos para prover e garantir proteção da informação que, quando corretamente configurados e utilizados, podem auxiliar os usuários a se protegerem dos riscos envolvendo o uso da Internet. Os serviços disponibilizados e as comunicações realizadas pela internet devem garantir os requisitos básicos de segurança e proteção da informação, como:

- Identificação: permitir que uma entidade se identifique, ou seja, diga quem ela é.
- I. Verificar se a entidade é realmente quem ela diz ser.
- II. Determinar as ações que a entidade pode executar.
- III. Proteger a informação contra alteração não autorizada.
- IV. Proteger a informação contra acesso não autorizado.
- V. Evitar que uma entidade possa negar que foi ela que executou uma ação.
- Disponibilidade: garantir que um recurso esteja disponível sempre que necessário.

As definições numeradas de I a V correspondem, respectivamente, a:

a) Integridade; Autenticação; Autorização; Acessabilidade; Não repúdio.
b) Identificação; Raio de Ação; Autorização; Acessabilidade; Negação.
c) Autenticação; Autorização; Integridade; Confidencialidade; Não repúdio.
d) Autenticação; Raio de Ação; Integridade; Confidencialidade; Identificação.
e) Integridade; Confidencialidade; Autenticação; Autorização; Negação.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








72
84



8. (FCC  /  DPE  RS  –  2013)  NÃO  está  associada  ao  conceito  de  preservação  da segurança  da informação a:

a) integridade.
b) autenticidade.
c) aplicabilidade.
d) disponibilidade.
e) confidencialidade.

9. (FCC  /  SABESP  –  2017)  A  criptografia  de  chave  pública  utiliza  duas  chaves  distintas:  uma pública,  que  poderá  ser  livremente  divulgada,  e  uma  privada,  que  deverá  ser  mantida  em segredo por seu dono. Quando uma informação é codificada com uma das chaves, somente a outra chave do par poderá decodificá-la. Qual chave usar para codificar depende da proteção que  se  deseja,  se  confidencialidade  ou  autenticação,  integridade  ou  não  repúdio.  A  chave privada poderá ser armazenada de diferentes maneiras, como um arquivo no computador, um smartcard ou um token.

(Adaptado de: http://cartilha.cert.br/criptografia/) 
Se um Estagiário tiver que selecionar um método criptográfico que usa chave pública, poderá selecionar o:

a) AES.
b) RSA.
c) RC4.
d) 3DES.
e) Blowfish.

10. (FCC  /  SEFAZ  RJ  –  2014) A Receita Federal do Brasil (RFB) publicou em seu site a seguinte determinação:

É obrigatória a utilização de ......, para apresentação de declarações à RFB, por todas as pessoas jurídicas, exceto as optantes pelo Simples Nacional. As pessoas físicas não estão obrigadas à sua utilização.  As  autoridades  certificadoras  (AC)  não possuem  capacidade  de  atendimento  de demanda  ilimitada.  Assim,  é  conveniente  que  as  empresas  não  deixem  para  fazer  a  sua aquisição na última hora.

Atenção! As entidades sem fins lucrativos também estão obrigadas à entrega de declarações e demonstrativos com a sua utilização, de acordo com a legislação pertinente a cada assunto.

(Adaptado de: http://www.receita.fazenda.gov.br/atendvirtual/orientacoes/obrigatoriedadecd.htm) 
Preenche corretamente a lacuna:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








73
84



a) assinatura digital autenticada.
b) certificado digital válido.
c) certificado digital autenticado pela RFB.
d) assinatura e certificado digitais emitidos pela AC-raiz.
e) assinatura e certificado digitais autenticados pela RFB.

11. (FCC / SEFAZ RJ – 2014) Considere:

- Funciona como uma impressão digital de uma mensagem, gerando, a partir de uma entrada de tamanho variável, um valor fixo pequeno.

- Este valor está para o conteúdo da mensagem assim como o dígito verificador de uma conta- corrente está para o número da conta ou o check sum está para os valores que valida.

- É utilizado para garantir a integridade do conteúdo da mensagem que representa.

- Ao ser utilizado, qualquer modificação no conteúdo da mensagem será detectada, pois um novo cálculo do seu valor sobre o conteúdo modificado resultará em um valor bastante distinto.

Os itens acima descrevem:

a) um Certificado digital b) uma Assinatura digital c) um Algoritmo de chave pública d) um Algoritmo de chave secreta e) um Hash criptográfico 
12. (FCC / Prefeitura de São Paulo – 2012) Considere a frase a seguir.

Na  criptografia  ..I..  ,  um  emissor  codifica  seu  documento  com  a  chave  ..II..  da  pessoa  que receberá a mensagem. O texto codificado apenas poderá ser decodificado pelo ..III.. , pois, somente ele tem a chave ..IV.. relacionada à chave ..V.. que originou o texto cifrado.

As lacunas I, II, III, IV e V devem ser preenchidas, correta e respectivamente, por 
a) de chaves públicas, privada, destinatário, pública e privada.
b) assimétrica, privada, emissor, pública e privada.
c) simétrica, pública, emissor, privada e pública.
d) assimétrica, pública, destinatário, privada e pública.
e) simétrica, privada, destinatário, pública e privada.

13. (FCC / Prefeitura de São Paulo – 2012) A assinatura digital é o resultado da aplicação de uma função matemática que gera uma espécie de impressão digital de uma mensagem. O primeiro Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








74
84



passo no processo de assinatura digital de um documento eletrônico é a aplicação dessa função, que fornece uma sequência única para cada documento conhecida como "resumo".

A função matemática citada é mais conhecida como função:

a) quântica.
b) de Hash.
c) quadrática.
d) de Euler.
e) binária.

































Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








75
84



GABARITO - FCC

1. LETRA B
2. LETRA B
3. LETRA E
4. LETRA C
5. LETRA A
6. LETRA B
7. LETRA C
8. LETRA C
9. LETRA B
10. LETRA B
11. LETRA E
12. LETRA D
13. LETRA B



























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








76
84



QUESTÕES COMENTADAS – DIVERSAS BANCAS 
1. (CONSULPLAN / TJ MG – 2017) Segurança da informação é o mecanismo de proteção de um conjunto de informações com o objetivo de preservar o valor que elas possuem para uma pessoa ou  organização.  Está  correto  o  que  se  afirma  sobre princípios  básicos  de  segurança  da informação, EXCETO:

a) Disponibilidade garante que a informação esteja sempre disponível.
b) Integridade garante a exatidão da informação.
c) Confidencialidade garante que a informação seja acessada somente por pessoas autorizadas.
d) Não repúdio garante a informação é autêntica e que a pessoa recebeu a informação.

Comentários:

A
Autenticidade garantir que quem envia a informação é quem diz ser. Uma maneira de garanti-la é com a autenticação de usuários (Senhas ou Tokens). Já o Não-repúdio  (ou  irretratabilidade) garante que o autor não negará ter criado e assinado o conteúdo da informação. Uma maneira de garanti-la é com o uso de certificados digitais. Conforme vimos em aula, o princípio que garante que a informação é autêntica é o Princípio da Autenticidade.

Gabarito: Letra D

2. (ESAF  /  Ministério  da  Fazenda  –  2014)  Assinale  a  opção  correta  relativa  à  Segurança  da Informação.

a) Criptografia: técnica para converter uma mensagem de texto entre sistemas operacionais distintos.
b)  Autenticação:  sequência  de  símbolos  destinada  a permitir  que  o  algoritmo  cifre  uma mensagem em texto claro ou decifre uma mensagem criptografada.
c) Autenticação: procedimento destinado a autorizar a sintaxe de determinada mensagem.
d) Autenticação: procedimento destinado a verificar a validade de determinada mensagem.
e)  Inicializador:  sequência  de  símbolos  destinada  a  permitir  que  o  algoritmo  inicie  uma mensagem em texto claro para decifrar uma mensagem criptografada.

Comentários:

(a) Errada. A criptografia é um método que codifica os dados do usuário para que só o destinatário possa ler, dessa maneira garantindo a confidencialidade da informação;

(b) Errada. Autenticação é um procedimento que visa garantir que quem envia a informação é quem diz ser. Lembrando que a sequência de símbolos na questão é chamada de chave de criptografia;

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








77
84



(c) Errada. Autenticação é um procedimento que visa garantir que quem envia a informação é quem diz ser;

(d) Correto. Autenticação é um procedimento que visa garantir que quem envia a informação é quem diz ser. Ou seja, que verifica que uma mensagem é válida (verdadeira) ou não.

(e) Errada. A sequência de símbolos em questão é chamada de chave de criptografia.

Gabarito: Letra D

3. (INAZ do Pará / CRO RJ - 2016) Quando navegamos na internet, sempre nos preocupamos na segurança das informações. Marque a alternativa correta em que o browser demonstra que o site está seguro.

a) http
b) https
c) http://
d) Antivírus
e) Worm


Comentários:

Pessoal, o protocolo de internet mais conhecido é o http. Quando navegamos de forma segura, em sites de compra ou no seu banco, por exemplo, é utilizado o https. Para não esquecer, lembre-se sempre de S de Segurança.

Gabarito:
Letra B

4. (INAZ  do  Pará  /  Prefeitura  de  Curuçá  –  2014) Em função de muitos ataques de hacker em diversos dados sigilosos, atualmente a maioria das empresas estão utilizando a certificação digital  como  uma  forma  de  envio  mais  seguro  das  informações  a  diversos  órgãos governamentais e privados. Qual a técnica que garante a veracidade do envio da informação pelo real remetente?

a) VPN.
b) Senha.
c) Não repúdio.
d) Integridade.
e) Confidencialidade.


Comentários:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








78
84



Galera, o princípio do não-repúdio é o que garante que a informação/mensagem foi realizada por aquela  pessoa  determinada.  Isto  é,  o  autor  não  negará  ter  criado  e  assinado  o  conteúdo  da informação. Uma maneira de garanti-la é com o uso de certificados digitais.

Gabarito: Letra C

5. (INAZ do Pará / BANPARÁ – 2014) Segundo os padrões internacionais, o tripé da segurança da informação são:

a) Antivírus, Firewall e Certificação Digital b) Senha, Antivírus e AntiSpam c) Consistência, Autenticidade, Integridade d) Confidencialidade, Disponibilidade e Integridade e) Navegabilidade, Acessibilidade e Usabilidade 

Comentários:

Os três princípios consagrados da segurança da informação são: Confidencialidade, Integridade e Disponibilidade – conhecidos como CID. Se um ou mais desses princípios forem desrespeitados em algum momento, significa que houve um incidente de segurança da informação.

Relembrando rapidamente o conceito de cada um, temos que a confidencialidade é o princípio de que a informação não esteja disponível ou seja revelada a indivíduos, entidades ou processos não autorizados; a integridade é o princípio de salvaguarda da exatidão e completeza de ativos de informação; e a
disponibilidade é o princípio da capacidade de estar acessível e utilizável quando demandada por uma entidade autorizada.

Gabarito: Letra D

6. (IBADE  /  PM  AC  –  2017) Quanto mais a tecnologia se desenvolve, mais atividades são feitas pelos computadores pessoais, como pagamento de contas e armazenamento de arquivos com informações pessoais. Diante disso, cada vez mais deve-se pensar na segurança da informação.
A melhor maneira de um usuário proteger informações quando está longe de seu computador é:

a) bloquear o computador com uma senha.
b) deixar o computador em modo de baixa energia.
c) ativar a proteção de tela.
d) desligar a rede sem fio.
e) desligar o monitor.

Comentários:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








79
84



(a)  Correto.  Esse  procedimento  realmente  protege  informações  do  usuário;  (b)  Errado.  Esse procedimento não protege informações do usuário; (c) Errado. Esse procedimento não protege informações do usuário; (d) Errado. Esse procedimento não protege informações do usuário; (e) Errado. Esse procedimento não protege informações do usuário;

Gabarito:
Letra A

7. (FUNDATEC / SEFAZ RS – 2009) O Decreto-Lei no 2.848, de 7 de dezembro de 1940 (Código Penal), em seu artigo 313-A, incluído pela Lei no 9.983, de 2000, diz o seguinte: "Inserir ou facilitar, o funcionário autorizado, a inserção de dados falsos, alterar ou excluir indevidamente dados corretos nos sistemas informatizados ou bancos de dados da Administração Pública com o fim de obter vantagem indevida para si ou para outrem ou para causar dano: Pena - reclusão, de 2 (dois) a 12 (doze) anos, e multa.". Esse artigo do Código Penal auxilia na preservação das informações existentes nas entidades e órgãos públicos, através da fixação de pena de reclusão, caso seja violado, nas condições desse artigo, o(s) seguinte(s) princípio(s) fundamental(ais) da Segurança da Informação:

I. Integridade.
I. Disponibilidade.
III. Confidencialidade.

Quais estão corretas?

a) Apenas I.
b) Apenas II.
c) Apenas III.
d) Apenas I e II.
e) I, II e III.

Comentários:

Essa é uma questão polêmica! Fica evidente que não houve quebra da confidencialidade porque se trata de um funcionário autorizado. Fica claro também que houve quebra da integridade porque dados foram inseridos, alterados ou excluídos – modificando a informação original. Por outro lado, a  análise  da  disponibilidade  é  complexa!  Eu  e  o  Prof.  Renato  da  Costa  discutimos  e  nós  não concordamos que tenha havido uma quebra da disponibilidade. A simples exclusão de um dado não caracteriza a perda da disponibilidade. Caso assim fosse, toda quebra de integridade implicaria necessariamente em quebra da disponibilidade. Dessa forma, eu discordo do gabarito oficial da banca de que foram violados os princípios da integridade e disponibilidade.

Gabarito: Letra D

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








80
84



8. (FUNDATEC  /  DPE  SC  –  2018)  A  certificação  digital  é  utilizada  para  garantir, de  forma eletrônica, a autoria de determinado documento, como por exemplo, o perito responsável por determinado laudo. Um dos componentes da certificação digital é a utilização de criptografia.
Diante do exposto, é correto afirmar que, para verificar a assinatura digital de um perito em relação a um laudo pericial emitido por ele, a primeira etapa é a aplicação:

a) Da chave criptográfica privada do perito.
b) Da chave criptográfica pública do perito.
c) Da chave criptográfica simétrica de quem quer validar.
d) De um algoritmo de hash simétrico de tamanho qualquer.
e) De um algoritmo de hash assimétrico de tamanho mínimo de 128 bits.


Comentários:

(a) Errado. Para verificar a assinatura digital do perito, eu não posso utilizar sua chave privada porque somente ele tem acesso a ela; (b) Correto. Para verificar a assinatura digital do perito, utiliza-se  a  chave  pública  dele  correspondente  à  chave  privada,  de  modo  que  seja  possível identificá-lo  inequivocamente;  (c)  Errado.  Não  se  utiliza  criptografia  simétrica  na  certificação digital; (d) Errado. Algoritmo de Hash é apenas o algoritmo utilizado no processo de assinatura digital e não é capaz de verificar a assinatura do perito – e não existe algoritmo de hash simétrico;
(e) Errado. Algoritmo de Hash é apenas o algoritmo utilizado no processo de assinatura digital e não é capaz de verificar a assinatura do perito – e não existe algoritmo de hash assimétrico;

Gabarito: Letra B

9. (IDECAN / AGU – 2014) O recurso que estuda os princípios e técnicas pelas quais a informação pode ser transformada da sua forma original para outra ilegível, com o objetivo de dificultar a leitura de pessoas não autorizadas, denomina-se 
a) Backup.
b) Webgrafia.
c) criptografia.
d) quarentena.
e) endereçamento.

Comentários:

Quando necessitamos ocultar uma informação, deixando-a ilegível para pessoas não autorizadas utilizamos a criptografia.

Gabarito: Letra C
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








81
84



LISTA DE QUESTÕES – DIVERSAS BANCAS 
1. (CONSULPLAN / TJ MG – 2017) Segurança da informação é o mecanismo de proteção de um conjunto de informações com o objetivo de preservar o valor que elas possuem para uma pessoa ou  organização.  Está  correto  o  que  se  afirma  sobre princípios  básicos  de  segurança  da informação, EXCETO:

a) Disponibilidade garante que a informação esteja sempre disponível.
b) Integridade garante a exatidão da informação.
c) Confidencialidade garante que a informação seja acessada somente por pessoas autorizadas.
d) Não repúdio garante a informação é autêntica e que a pessoa recebeu a informação.

2. (ESAF  /  Ministério  da  Fazenda  –  2014)  Assinale  a  opção  correta  relativa  à  Segurança  da Informação.

a) Criptografia: técnica para converter uma mensagem de texto entre sistemas operacionais distintos.
b)  Autenticação:  sequência  de  símbolos  destinada  a permitir  que  o  algoritmo  cifre  uma mensagem em texto claro ou decifre uma mensagem criptografada.
c) Autenticação: procedimento destinado a autorizar a sintaxe de determinada mensagem.
d) Autenticação: procedimento destinado a verificar a validade de determinada mensagem.
e)  Inicializador:  sequência  de  símbolos  destinada  a  permitir  que  o  algoritmo  inicie  uma mensagem em texto claro para decifrar uma mensagem criptografada.

3. (INAZ do Pará / CRO RJ - 2016) Quando navegamos na internet, sempre nos preocupamos na segurança das informações. Marque a alternativa correta em que o browser demonstra que o site está seguro.

a) http
b) https
c) http://
d) Antivírus
e) Worm


4. (INAZ  do  Pará  /  Prefeitura  de  Curuçá  –  2014) Em função de muitos ataques de hacker em diversos dados sigilosos, atualmente a maioria das empresas estão utilizando a certificação digital  como  uma  forma  de  envio  mais  seguro  das  informações  a  diversos  órgãos governamentais e privados. Qual a técnica que garante a veracidade do envio da informação pelo real remetente?

a) VPN.
b) Senha.
c) Não repúdio.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








82
84



d) Integridade.
e) Confidencialidade.

5. (INAZ do Pará / BANPARÁ – 2014) Segundo os padrões internacionais, o tripé da segurança da informação são:

a) Antivírus, Firewall e Certificação Digital b) Senha, Antivírus e AntiSpam c) Consistência, Autenticidade, Integridade d) Confidencialidade, Disponibilidade e Integridade e) Navegabilidade, Acessibilidade e Usabilidade 

6. (IBADE  /  PM  AC  –  2017) Quanto mais a tecnologia se desenvolve, mais atividades são feitas pelos computadores pessoais, como pagamento de contas e armazenamento de arquivos com informações pessoais. Diante disso, cada vez mais deve-se pensar na segurança da informação.
A melhor maneira de um usuário proteger informações quando está longe de seu computador é:

a) bloquear o computador com uma senha.
b) deixar o computador em modo de baixa energia.
c) ativar a proteção de tela.
d) desligar a rede sem fio.
e) desligar o monitor.

7. (FUNDATEC / SEFAZ RS – 2009) O Decreto-Lei no 2.848, de 7 de dezembro de 1940 (Código Penal), em seu artigo 313-A, incluído pela Lei no 9.983, de 2000, diz o seguinte: "Inserir ou facilitar, o funcionário autorizado, a inserção de dados falsos, alterar ou excluir indevidamente dados corretos nos sistemas informatizados ou bancos de dados da Administração Pública com o fim de obter vantagem indevida para si ou para outrem ou para causar dano: Pena - reclusão, de 2 (dois) a 12 (doze) anos, e multa.". Esse artigo do Código Penal auxilia na preservação das informações existentes nas entidades e órgãos públicos, através da fixação de pena de reclusão, caso seja violado, nas condições desse artigo, o(s) seguinte(s) princípio(s) fundamental(ais) da Segurança da Informação:

I. Integridade.
I. Disponibilidade.
III. Confidencialidade.

Quais estão corretas?

a) Apenas I.
b) Apenas II.
c) Apenas III.
d) Apenas I e II.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








83
84



e) I, II e III.

8. (FUNDATEC  /  DPE  SC  –  2018) A  certificação  digital  é  utilizada  para  garantir, de  forma eletrônica, a autoria de determinado documento, como por exemplo, o perito responsável por determinado laudo. Um dos componentes da certificação digital é a utilização de criptografia.
Diante do exposto, é correto afirmar que, para verificar a assinatura digital de um perito em relação a um laudo pericial emitido por ele, a primeira etapa é a aplicação:

a) Da chave criptográfica privada do perito.
b) Da chave criptográfica pública do perito.
c) Da chave criptográfica simétrica de quem quer validar.
d) De um algoritmo de hash simétrico de tamanho qualquer.
e) De um algoritmo de hash assimétrico de tamanho mínimo de 128 bits.


9. (IDECAN / AGU – 2014) O recurso que estuda os princípios e técnicas pelas quais a informação pode ser transformada da sua forma original para outra ilegível, com o objetivo de dificultar a leitura de pessoas não autorizadas, denomina-se 
a) Backup.
b) Webgrafia.
c) criptografia.
d) quarentena.
e) endereçamento.




















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








84
84



GABARITO – DIVERSAS BANCAS 
1. LETRA D
2. LETRA D
3. LETRA C
4. LETRA A
5. LETRA B
6. LETRA C
7. LETRA D
8. LETRA A
9. LETRA D
10. LETRA B
11. LETRA C

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 05
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 