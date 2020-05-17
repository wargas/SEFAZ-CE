

Livro Eletrônico
Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti 06315057411 - EVA CELESTE DE SOUZA 





1
128




Sumário
1 – Malwares .................................................................................................................................... 5 1.1 – Conceitos Básicos ................................................................................................................ 5 1.2.1 Infecção ............................................................................................................................ 5 1.2.2 Prevenção......................................................................................................................... 6 1.2 – Terminologia ........................................................................................................................ 7 2 – Principais Malwares .................................................................................................................... 9 2.1 – Vírus ..................................................................................................................................... 9 2.1.1 Vírus de Script ................................................................................................................ 13 2.1.2 Vírus de Macro ............................................................................................................... 14 2.1.3 Vírus de Boot .................................................................................................................. 15 2.1.4 Vírus de Arquivo ............................................................................................................. 17 2.1.5 Vírus Polimórfico ............................................................................................................ 18 2.1.6 Vírus Stealth ................................................................................................................... 20 2.1.7 Vírus Time Bomb ............................................................................................................ 21 2.2 – Worm ................................................................................................................................. 22 2.3 – Bot e Botnet....................................................................................................................... 24 2.4 – Trojan Horse ...................................................................................................................... 27 2.5 – Spyware ............................................................................................................................. 30 2.6 – Backdoor ............................................................................................................................ 32 2.7 – Rootkit ............................................................................................................................... 34 2.8 – Tabela Comparativa ........................................................................................................... 36 3 – Outros Malwares ...................................................................................................................... 37 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





2
128




3.1 – Ransomware....................................................................................................................... 37 3.2 – Keyloggers ......................................................................................................................... 39 3.3 – Screenloggers .................................................................................................................... 41 3.4 – Adwares ............................................................................................................................. 42 3.5 – Sniffer ................................................................................................................................. 44 3.6 – Bombas Lógicas ................................................................................................................. 46 3.7 – Exploits .............................................................................................................................. 48 3.8 – Hijacker .............................................................................................................................. 49 4 – Ataques e Golpes ..................................................................................................................... 51 4.1 – Engenharia Social .............................................................................................................. 51 4.2 – Força Bruta ........................................................................................................................ 54 4.3 – Denial of Service (DoS) ...................................................................................................... 56 4.4 – IP Spoofing ........................................................................................................................ 58 4.5 – E-mail Spoofing ................................................................................................................. 60 4.6 – Phishing Scam .................................................................................................................... 62 4.7 – Pharming ............................................................................................................................ 67 4.8 – Hoax................................................................................................................................... 70 4.9 – Man in the Middle.............................................................................................................. 72 4.10 – Defacement ..................................................................................................................... 73 Resumo .......................................................................................................................................... 74 Mapa Mental .................................................................................................................................. 78 Questões Comentadas - FCC ........................................................................................................ 83 Lista de Questões - FCC ................................................................................................................ 93 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





3
128




Gabarito ....................................................................................................................................... 101 Questões Comentadas – DIVERSAS BANCAS ............................................................................. 102 Lista de Questões – DIVERSAS BANCAS ..................................................................................... 118 Gabarito ....................................................................................................................................... 128 






























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





4
128




APRESENTAÇÃO DA AULA Fala, galera! O assunto da nossa aula de hoje é Softwares Maliciosos (Malware)! Pessoal, essa aula serve para que vocês façam provas de concurso, mas que também servem para a vida. Vamos ver aqui diversas pragas virtuais (categorias e ações maliciosas) – além de descobrir como nos prevenir.
Eu sou especialista nisso, porque minha esposa já instalou tudo que vocês puderem imaginar no computador dela! Falaremos também de ataques e golpes comuns na internet. Ok?

PROFESSOR DIEGO CARVALHO - www.instagram.com/professordiegocarvalho 
Galera, todos os tópicos da aula possuem Faixas de Incidência, que indicam se o assunto cai muito ou pouco em prova. Diego, se cai pouco para que colocar em aula? Cair pouco não significa que não cairá justamente na sua prova! A ideia aqui é: se você está com pouco tempo e precisa ver somente aquilo que cai mais, você pode filtrar pelas incidências média, alta e altíssima; se você tem tempo sobrando e quer ver tudo, vejam também as incidências baixas e baixíssimas. Fechado?

INCIDÊNCIA EM PROVA: baixíssima 
INCIDÊNCIA EM PROVA: baixa 
INCIDÊNCIA EM PROVA: média 
INCIDÊNCIA EM PROVA: ALTA 
INCIDÊNCIA EM PROVA: Altíssima 






Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





5
128




1 – MALWARES
1.1 – CONCEITOS BÁSICOS INCIDÊNCIA EM PROVA: baixa 
Malwares  (Malicious  Softwares)  – também  chamados  de  Softwares  Maliciosos  ou  Pragas Virtuais  –  são  programas  especificamente  desenvolvidos  para  executar  ações  danosas  e atividades maliciosas em um computador. Eles são inseridos intencionalmente em um sistema computacional com um propósito prejudicial. Algumas das formas como eles podem infectar ou comprometer um computador são:

FORMAS comuns DE INFECÇÃO DE MALWARES Pela  exploração  de  vulnerabilidades  existentes  nos programas  instalados  ou  pela  auto-execução  de  mídias removíveis infectadas, como pen-drives;
Pelo acesso a páginas maliciosas, utilizando navegadores vulneráveis ou pela ação direta de atacantes que, após invadirem o computador, incluem arquivos contendo códigos maliciosos;
Pela execução de arquivos previamente infectados, obtidos em anexos de mensagens eletrônicas, via mídias removíveis, em páginas web ou de outros computadores.

Uma vez instalados, os códigos maliciosos passam a ter acesso aos dados armazenados no computador e podem executar ações em nome dos usuários , de acordo com as permissões de cada usuário. Os principais motivos que levam um atacante a desenvolver e a propagar códigos maliciosos são a obtenção de vantagens financeiras, a coleta de informações confidenciais, o desejo de autopromoção e o vandalismo.

Além  disso, os  códigos  maliciosos  são  muitas  vezes  utilizados  como  intermediários  e possibilitam a prática de golpes virtuais, a realização de ataques e a disseminação de spam (mensagens  indesejadas) .  Em  suma:  o  termo malware  abrange  qualquer  tipo  de  software indesejado,  instalado  sem  o  devido  consentimento  no  computador  do  usuário.  As  principais categorias de malware são: Vírus, Worm, Bot, Trojan, Spyware, Backdoor e Rootkit.



1.2.1 Infecção

A principal porta de entrada para os malwares hoje é a Internet! Ela pode ocorrer por meio da execução  de  arquivos  infectados  obtidos  de  anexos  de  mensagens  eletrônicas,  de  mídias removíveis ou dispositivos de memória flash (Ex: PenDrive), de páginas web comprometidas, de PRINCIPAIS CATEGORIAS DE MALWARES VÍRUSWORMBOTTROJANSPYWAREBACKDOORROOTKIT Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





6
128




redes  sociais  ou  diretamente  de  outros  equipamentos.  É  interessante  também  tomar  muito cuidado ao fazer o download de arquivos com alguns formatos específicos.

1.2.2 Prevenção

É muito provável que a maioria dos seus dados está gravado em seu computador pessoal e, é por meio dele, que você acessa seus e-mails e redes sociais, e realiza transações bancárias e comerciais.
Por conta disso, mantê-lo seguro é essencial para se proteger dos riscos envolvidos no uso da Internet.  Além  disso,  ao  manter  seu  computador  seguro,  você  diminui  as  chances  de  ele  ser indevidamente utilizado para atividades maliciosas.

Por diversas vezes, os atacantes estão interessados em conseguir o acesso a grande quantidade de computadores, independentemente de quais são e das configurações que possuem.
Dessa forma,
acreditar que seu computador está protegido, por não apresentar atrativos para um atacante, pode ser um erro gigantesco . Logo, para manter seu computador pessoal seguro, é importante seguir os seguintes procedimentos:

PROCEDIMENTOS DE SEGURANÇA Manter os programas instalados com as versões mais recentes;
Ser cuidadoso ao instalar aplicativos desenvolvidos por terceiros;
Utilizar apenas softwares originais (sem pirataria);
Manter os programas instalados com todas as atualizações aplicadas;
Utilizar mecanismos de proteção (antivírus, firewall, etc);
Ser cuidadoso ao enviar seu computador para serviços de manutenção;
Utilizar configurações de segurança disponíveis;
Ser cuidadoso ao manipular arquivos;
Proteger seus dados (utilizando backup, por exemplo);
Manter seu computador com data e hora corretas;
Criar um disco de recuperação de sistema;
Ser cuidadoso ao utilizar o computador em locais públicos.



Para mais informações, eu recomendo que vocês acessem o site do CERT.BR. Essa aula teórica foi completamente baseada em seus documentos. Acessem: http://www.cert.br.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





7
128





1.2 – TERMINOLOGIA
INCIDÊNCIA EM PROVA: baixíssima 


TERMINOLOGIA DESCRIÇÃO Hacker
O conceito de Hacker é o de um usuário experiente – um exímio programador – que invade sistemas computacionais para provar sua capacidade e habilidades com computadores.

Cracker
Elementos que invadem sistemas para roubar informações e causar danos às vítimas, além de ser  também uma denominação  associada  àqueles  que  decifram  códigos  indevidamente  e destroem proteções de software favorecendo a pirataria.
Script Kiddies
Também chamado de Newbies, essa terminologia é utilizada para o hacker iniciante, que utiliza de ferramentas prontas na internet para realizar ataques a sistemas computacionais.

Insiders
Ameaças internas a uma instituição, funcionários descontentes ou insatisfeitos, corruptos ou subornados ou até mesmo enganados.

Phreaking
É um especialista em telefonia, sua principal atividade é a realização de ligações gratuitas, clonagem e instalação de escutas em telefones fixos ou celulares.

Warez
Software pirata distribuído ilegalmente pela internet.


Spam
Termo usado para se referir aos e-mails não solicitados geralmente enviados para um grande número de pessoas com finalidade comercial.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





8
128





(SEAD/AP  -  2010)  Quando  se  trata  da  Gestão  da  Segurança  da  Informação,  a terminologia empregada no mundo dos hackers assume papel de importância. A esse respeito, dois termos são a seguir descritos.

I. É o hacking de sistemas telefônicos, geralmente com o objetivo de fazer ligações gratuitas ou para espionar ligações alheias;
II.  É  o  software  pirata  distribuído  ilegalmente  pela  Internet.  Esses  dois  termos  são denominados, respectivamente como:

a) phishing e worm.
b) phreaking e warez.
c) war dialer e worm.
d) phreaking e phishing.
e) phishing e warez.
_______________________ Comentários: conforme vimos em aula, trata-se do Pheaking e Warez (Letra B).

(PCDF  -  2012) No  mundo cibernético,  qual é  o termo  utilizado  para  designar  quem pratica quebra de proteções de softwares cedidos a título de demonstração usando-os por tempo indeterminado como se fossem cópias legítimas.

a) worm
b) hacker
c) trojan
d) malware
e) cracker
_______________________ Comentários:  conforme  vimos  em  aula,  trata-se  do  indivíduo  que “quebra”  um  sistema  de  segurança  indevidamente, geralmente associados à pirataria (Letra E).

(Câmara De Araraquara - 2016) O termo técnico, em inglês, que se refere a e-mails não solicitados,  que  geralmente  são  enviados  para  um  grande  número  de  pessoas  com intuitos geralmente comerciais é denominado:

a) zombie
b) worm
c) spam
d) wiki
_______________________ Comentários: conforme vimos em aula, trata-se do spam (Letra C).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





9
128





2 – PRINCIPAIS MALWARES 2.1 – VÍRUS
INCIDÊNCIA EM PROVA: Altíssima 


Os  vírus  de  computador  foram  introduzidos  na  década  de  1980,  com  funções  simples  que ocasionalmente  geravam  inconvenientes  ou  apenas  mostravam  informações  ao  usuário.
Atualmente esse tipo de código traz um risco significativo com potencial destrutivo e que demanda grande esforço das organizações para manterem seus sistemas a salvo. Mas o que é um vírus de computador?

O vírus é um programa ou parte de um programa, normalmente malicioso 1
, que se propaga
infectando, inserindo cópias de si mesmo, anexando-se ou hospedando-se em arquivos ou programas existentes na máquina . Para que um código malicioso seja considerado um vírus, ele deve ter a capacidade de auto replicação, ou seja, fazer uma cópia de si mesmo e distribuir essa cópia para outros arquivos e programas do sistema infectado.

O principal objetivo de um vírus é replicar-se e contaminar o maior número possível de programas, de maneira a comprometer outros sistemas.
Para tal, o vírus depende da execução do programa ou arquivo hospedeiro para se tornar ativo e dar continuidade à infecção 2
! Essa informação é

1
Eles não precisam ser necessariamente destrutivos ou maliciosas para o sistema do usuário. Um vírus pode, por exemplo, simplesmente mostrar uma imagem na tela do computador.
2
Para que um vírus recebido em um anexo de um e-mail seja ativado é necessário que anexo contaminado seja aberto ou executado. Logo, não é necessária a execução explícita do vírus em si, apenas do arquivo ou programa infectado.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





10
128




bastante  importante:  vírus  não  são  autossuficientes,  eles  necessitam  da  execução  de  um hospedeiro para se propagar pelas redes enviando cópias de si mesmo.

Pode-se dizer, então, que um vírus realiza duas tarefas: primeiro, replica-se das mais variadas formas;
segundo, executa  seu  código  malicioso,  podendo  exercer  diversas  funcionalidades danosas na máquina infectada – como exibir uma mensagem na tela do computador, tornar a máquina mais lenta, reiniciar o computador, apagar arquivos fundamentais do disco rígido ou, no limite, causar a destruição total de todos os dados armazenados na máquina.

(TJ/SE  –  2014)  Vírus  são  programas  que  podem  apagar  arquivos  importantes armazenados no computador, podendo ocasionar, até mesmo, a total inutilização do sistema operacional.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).

Um vírus é composto basicamente de três partes: um mecanismo de infecção, um mecanismo de ativação e uma carga útil. Vejamos na tabela a seguir como essas partes são definidas:

COMPOSIÇÃO DE UM VÍRUS MECANISMO DE INFECÇÃO MECANISMO DE ATIVAÇÃO CARGA ÚTIL Meios  ou  formas  pelas  quais  um vírus se propaga, habilitando-o a se reproduzir.  É  também  conhecido como Vetor de Infecção.
Evento ou condição que determina quando  a  carga  útil  é  ativada  ou entregue.  Às  vezes,  é  conhecido como Bomba Lógica.
O que o vírus faz, além de se espalhar.
A carga útil pode envolver algum dano ou atividade benigna, porém notável.

(Polícia Federal – 2018) Uma das partes de um vírus de computador é o mecanismo de infecção,  que  determina  quando  a  carga  útil  do  vírus  será  ativada  no  dispositivo infectado.
_______________________ Comentários: conforme vimos em aula, a questão trata – na verdade – do Mecanismo de Ativação (Errado).

Quando se trata de vírus de computador, eles podem ser classificados em quatro fases de execução:
Dormência, Propagação, Ativação e Ação. Vejamos:

FASES DESCRIÇÃO
DORMÊNCIA
Nessa fase, o vírus está ocioso. A certa altura, ele será ativado por algum evento, como uma data, a presença de outro programa ou arquivo, ou a ultrapassagem de algum limite de capacidade de disco. Nem todos os vírus têm esse estágio.

PROPAGAÇÃO
Nessa fase, o vírus instala uma cópia de si mesmo em outros programas ou em certas áreas do sistema no disco. A cópia pode não ser idêntica à versão de propagação; muitas vezes, os vírus mudam de forma para escapar à detecção. Agora, cada programa infectado conterá um clone do vírus, que também entrará em uma fase de propagação.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





11
128




ATIVAÇÃO
Nessa fase, o vírus é ativado para executar a função pretendida. Como ocorre com a fase de dormência, a fase de ativação pode ser causada por uma variedade de eventos de sistema, incluindo a contagem do número de vezes que essa cópia de vírus fez uma cópia de si mesma.
AÇÃO
Nessa fase, a função é executada. Ela pode ser inofensiva, como uma mensagem na tela, ou danosa, como a destruição de programas e arquivos de dados.



(CBM/SC – 2015) Um dos grandes problemas que afeta quem trabalha com computação, seja usuário avançado ou mesmo doméstico, é a possibilidade de infecção de seu sistema por um vírus. Com o crescimento da internet, cresce também a criminalidade virtual, e nos noticiários muitas vezes se vê algo relacionado ao tema. De acordo com Goodrich e Tamassia (2013), um vírus de computador, ou normalmente como é chamado, vírus, trata-se de um programa de computador, que pode ser replicado pela modificação de outros  arquivos  e/ou  programas,  para  inserir  código  capaz  de  replicação  posterior.
Segundo os autores, os vírus de um computador, normalmente seguem quatro fases de execução. São elas:

a)  Dormente; Propagação; Ativação; e, Ação.
b)  Ataque; Penetração; Replicação; e, Liberação.
c)  Diversidade; Robustez; Autoexecução; e, Privilégio.
d)  Anonimato; Garantia; Autenticidade; e, Disponibilidade.
_______________________ Comentários: conforme vimos em aula, trata-se da Dormência, Propagação, Ativação e Ação (Letra A).

A  maioria  dos  vírus  que  infectam  arquivos  de  programas  executáveis  realiza  seu  trabalho  de maneira que sejam específicos para um sistema operacional em particular e, em alguns casos, específicos até mesmo para uma determinada plataforma de hardware.
Dessa forma, eles são projetados para tirar proveito dos detalhes e fraquezas de sistemas particulares. Em outras palavras, em geral um malware que funciona em um sistema não funciona em outro.

Dito  isso,  existe  uma  lenda  de  que  o Linux  e  o  Mac  OS  são  sistemas operacionais  imunes  a  vírus!
Todo
Sistema  Operacional  (SO)  pode  ser alvo  de  vírus.  O  que  ocorre  é  que  – como   a   grande   maioria   dos computadores utiliza Windows – a taxa de replicação acaba sendo maior nesse sistema  operacional.  Ademais,  existe maior  interesse  em  se  criar  softwares maliciosos para esse SO!

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





12
128




(TJ/SE – 2014) Os computadores com sistema operacional Linux não são afetados por vírus; os que têm sistemas Windows são vulneráveis a vírus, por falhas específicas de kernel.
_______________________ Comentários: conforme vimos em aula, nenhum sistema operacional é imune a vírus e o Linux não é uma exceção (Errado).

Alguns tipos de vírus procuram permanecer ocultos, infectando arquivos do disco e executando uma série de atividades sem o conhecimento do usuário. Outros tipos de vírus permanecem inativos durante certos períodos, entrando em atividade apenas em datas específicas – quando sua carga útil é ativada.
Galera, existem diversos tipos de vírus – vamos vê-los em detalhes nas próximas páginas.

































Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





13
128




2.1.1 Vírus de Script INCIDÊNCIA EM PROVA: Altíssima 
Seus lindos, o que vocês acham que é um script? Um ator, por exemplo, possui um script para saber o que ele deve falar em uma cena. De forma similar, no mundo da tecnologia da informação, um script é um conjunto de instruções que devem ser executadas.
Por exemplo: páginas web estão lotadas de scripts escritos em uma linguagem chamada JavaScript que têm o intuito de tornar as páginas mais dinâmicas.

Se vocês desabilitarem esses scripts das páginas, vocês vão perceber que as páginas ficarão mais estáticas  e  sem  diversas  funcionalidades.  Da  mesma forma,  documentos  e  arquivos  de  um computador podem conter scripts. Querem um exemplo ? Documentos do Excel podem possuir as famosas  macros,  que  são  basicamente  scripts  que  executam  alguma  funcionalidade  no documento.
Como assim, Diego?

Galera, eu posso criar botão em um arquivo do MS-Excel que calcula, por exemplo, a média de valores de produtos vendidos em um supermercado – isso é feito por um macro, que é um tipo de script! Diferente  dos  scripts  de  páginas  web,  essas  macros são  scripts  escritos  em  uma linguagem chamada VBScript! Em suma, vírus de script são softwares maliciosos que podem ser escritos em alguma linguagem de script (Ex: JavaScript ou VBScript).

Em geral, eles são recebidos quando um usuário acessa uma página web ou faz o download de algum arquivo por-email, como um arquivo anexo ou como parte do próprio e-mail escrito em formato HTML. Logo, tomem bastante cuidado com os e-mails que vocês recebem – não saiam abrindo arquivos em anexo sem verificar antes – mesmo que seja recebido de algum remetente conhecido (lembre-se que o computador dele pode estar infectado).

Os  vírus  de  script  podem  ser  automaticamente  executados,  dependendo  da  configuração  do navegador web ou do programa leitor de e-mails do usuário.

(IFS/MS – 2016) Os vírus de scripts, que são os vírus que exploram as linguagens de script,  são  executados  automaticamente  pelos  softwares  de  leitura  de  e-mails,  por exemplo.
_______________________ Comentários: conforme vimos em aula, eles realmente exploram linguagens de script e são executados automaticamente pelos softwares de leitura de e-mails (Correto).

(PRF – 2019) No acesso a uma página web que contenha o código de um vírus de script, pode  ocorrer  a  execução  automática  desse  vírus,  conforme  as  configurações  do navegador.
_______________________ Comentários: conforme vimos em aula, eles – de fato – podem ser executados automaticamente no acesso a uma página web que contenha o código de um vírus de script (Correto).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





14
128




2.1.2 Vírus de Macro INCIDÊNCIA EM PROVA: Altíssima 
Nós a-ca-ba-mos de ver o que é uma macro! Nós já sabemos que se trata de um tipo de script, logo os vírus de macro são um tipo específico de vírus de script – escrito em linguagem de macro – que
tenta infectar arquivos manipulados por aplicativos que utilizam essa linguagem como, por exemplo, os arquivos de dados que compõem o Microsoft Office (Excel, Word, PowerPoint, Access, entre outros). Esse tipo de vírus despeeeeeenca em prova!

Os vírus de macro utilizam técnicas de propagação baseadas em anexos de documentos que executam macros, uma vez que os usuários frequentemente compartilham documentos com recursos  de  macro  habilitados.
Quando  um  software  carrega  um  arquivo  com  esse  código malicioso,  ele  executa  as  instruções  do  vírus  nele contidas,  que  geralmente  são  as  primeiras instruções executadas.

Galera,  vejam  a  imagem  a  seguir!
Um  dia  desses  eu  recebi  um  e-mail  de  um  remetente desconhecido falando comigo como se já nos conhecêssemos.
Havia três anexos com formato .mp4, .xlsx, .pptx. Era muito provável que os dois últimos tratassem de vírus de macro, apesar de haver outras possibilidades. O que eu fiz? Bloqueei o remetente e exclui a mensagem. Enfim, serviu pelo eu mostrar um caso real para vocês. Jamais abram anexos sem verificar antes!





vírus de macro
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





15
128




Ele infecta documentos e, não, programas – grande parte das informações em um sistema de computador se encontra na forma de documentos e, não, de programas;
Ele é fácil de se propagar, já que os documentos que eles exploram normalmente são compartilhados – um método muito comum de distribuição é por meio do envio de e-mails;
Como  ele  infecta  documentos  de  usuário,  os  tradicionais  controles  de  acesso  a  sistemas  de  arquivo  são de efetividade limitada para impedir que eles se espalhem;
Eles  geralmente  infectam  arquivos  de  dados  produzidos  por  suítes  de  aplicativos  de  escritório  como  o Microsoft Office;
Vírus de Macro costumam alterar ou substituir um conjunto de comandos utilizados por programas para executar ações comuns;
É necessário que o arquivo que contém o vírus de macro seja aberto para que ele execute suas automaticamente instruções maliciosas e infecte outros arquivos no computador;
Eles podem ser bloqueados por meio de uma configuração específica dos programas do MS-Office. Para tal, deve- se bloquear a execução de macros em documentos;
A propagação ocorre quando documentos por ele infectados são remetidos por correio eletrônico para outros usuários;
A assinatura digital de um arquivo por meio da utilização de um certificado digital é possível evitar vírus de macro.

(TRE/TO – 2011) Arquivos de dados produzidos por suíte de aplicativos para escritório, por ex. Microsoft Office, costumam ser alvo predileto de contaminação por:

a) trojans.
b) worms.
c) hijackers.
d) vírus de boot.
e) vírus de macro.
_______________________ Comentários: conforme vimos em aula, arquivos de dados de aplicativos de escritório são típicos de contaminação por vírus de macro (Letra E).

(CLDF – 2018) Um usuário de um computador relatou para o Administrador do sistema computacional que, ao abrir um arquivo do tipo .DOC recebido por e-mail, o computador utilizado começou a realizar ações erráticas e desordenadas. A partir desse relato, o Administrador concluiu que o computador foi infectado pelo malware do tipo:

a) Spyware
b) vírus de macro.
c) Trojan Dropper.
d) Backdoor.
e) Worm.
_______________________ Comentários: conforme vimos em aula, abrir um arquivo de uma suíte de escritório (MS-Word) podem conter macros, que podem conter vírus de macro capazes de realizar ações maliciosas (Letra B).
2.1.3 Vírus de Boot
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





16
128




INCIDÊNCIA EM PROVA: baixíssima 
Diego, o que é Boot? Galera, trata-se do procedimento de inicialização do computador durante o carregamento do sistema operacional, logo após a máquina ser ligada!
O Vírus de Boot – também chamado de Vírus de Setor ou Vírus de Setor de Inicialização – é um dos primeiros tipos de vírus conhecidos  e  infecta  a  parte  de  inicialização  do  sistema  operacional,  escondendo-se  no primeiro setor da memória.

Ele é ativado quando o computador é ligado e é carregado na memória antes mesmo do carregamento do sistema operacional. Os Vírus de Boot afetam  o  procedimento  descrito  anteriormente  e  podem  impedir  que  o sistema operacional seja executado de forma adequada – aliás, eles podem afetar inclusive dispositivos móveis de armazenamento como pendrives!

A  formatação rápida  de  um  pendrive  infectado  não  garante  a  remoção completa de vírus, uma vez que alguns malwares conseguem se alojar na MBR (Master  Boot  Record)  –  que  é  o  setor  de  inicialização  de  dispositivos  de armazenamento.  Recomenda-se,  portanto,  não  selecionar  a  opção  de Formatação Rápida apresentada na imagem acima.

(BB – 2011) Ativado quando o disco rígido é ligado e o sistema operacional é carregado;
é um dos primeiros tipos de vírus conhecido e que infecta a partição de inicialização do sistema operacional. Trata-se de:

a) vírus de boot.
b) cavalo de Troia.
c) verme.
d) vírus de macro.
e) spam.
_______________________ Comentários: conforme vimos em aula, trata-se do vírus de boot (Letra A).

(CODHAB – 2018) O vírus de boot é um vírus que age diretamente na inicialização do sistema de computadores conectados à rede. Contudo, ele não é espalhado por meio de dispositivos, como, por exemplo, pen drives.
_______________________ Comentários: conforme vimos em aula, eles podem ser espalhados por meio de dispositivos de armazenamento móveis, uma vez que





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





17
128




2.1.4 Vírus de Arquivo INCIDÊNCIA EM PROVA: Altíssima 
Também chamado de Vírus de Programa ou Vírus Parasitário, trata-se do vírus mais tradicional no cotidiano das pessoas.
Ele infecta arquivos executáveis, sobrescrevendo o código original e causando danos quase sempre irreparáveis. Em geral, replicam-se ao localizar outros arquivos executáveis, embora possam também infectar arquivos que sejam requisitados para a execução de alguns programas, como os arquivos com as seguintes extensões.



(SEPLAG/MG – 2013) Assinale a única alternativa correta, que corresponde a seguinte definição: “Estes tipos de vírus são os que mais causam danos, pois atacam arquivos executáveis (.exe, .com, .ovl, .dll) sobrescrevendo o código original e causando danos quase sempre irreparáveis. Para ser contaminado por este vírus se deve executar um arquivo já infectado.”:

a) Vírus invisível.
b) Vírus de macro.
c) Vírus de boot.
d) Vírus de programa.
_______________________ Comentários: conforme vimos em aula, trata-se do Vírus de Programa (Letra D).

(Câmara de Jaru/RO – 2019) Dos tipos de arquivo abaixo, você evitaria abrir para se proteger da instalação de um vírus o arquivo:

a) .AWS
b) .JPEG
c) .MP3
d) .EXE
e) .XLS
_______________________ Comentários: conforme vimos em aula, seria interessante evitar de abrir arquivos no formato .exe (Letra D).





FORMATOS DE ARQUIVO DE ALTO RISCO .EXE.VBS.COM.CMD.PIF.SYS.SRC.BAT.HLP.ASP.REG Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





18
128




2.1.5 Vírus Polimórfico INCIDÊNCIA EM PROVA: média 


Também chamado de Vírus Mutante, é capaz de assumir múltiplas formas a cada infecção com o intuito de burlar o software de antivírus. Como ele faz isso, professor? Ele muda sua assinatura, mantendo  suas  funcionalidades  e  alterando  apenas  o seu  padrão  de  bits.  A  assinatura  é  uma característica  utilizada  pelos  antivírus  para  detectar  a  sua  presença.  Pode  ser  um  nome,  um comportamento ou o tamanho do vírus.

Os vírus polimórficos são capazes de criar uma nova variante a cada execução, alterando tanto a rotina de encriptação quanto a rotina de decriptação.
Em geral, para realizar a detecção dessas ameaças, os antivírus fazem a decriptação do vírus usando um emulador ou realizam uma análise de padrão do corpo do vírus, uma vez que verificar a assinatura é pouco efetivo em um contexto em que o código muda, mas a semântica, não.

(CFA – 2010) Tem a capacidade de gerar réplicas de si mesmo utilizando-se de chaves de encriptação diversas, fazendo com que as cópias finais possuam formas diferentes. A polimorfia visa a dificultar a detecção de utilitários antivírus, já que as cópias não podem ser detectadas a partir de uma única referência do vírus. Tal referência normalmente é um pedaço do código virótico, que no caso dos vírus polimórficos varia de cópia para cópia.

O texto do enunciado da questão está se referindo aos vírus:

a) de scripts.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





19
128




b) criptografados.
c) mutantes.
d) stealth ou furtivos.
_______________________ Comentários: conforme vimos em aula, trata-se dos vírus mutantes (Letra C).

(CRESS/GO  –  2019)  Um  vírus  polimórfico  é  um  vírus  que  muda  a  cada  infecção, impossibilitando a detecção por sua assinatura.
_______________________ Comentários: conforme vimos em aula, eles realmente não podem ser detectados por meio da sua assinatura (Correto).

(CRESS/SC – 2019) O vírus polimórfico cria cópias idênticas de si durante a reprodução, o que o torna difícil de ser identificado pelos programas antivírus. Essas cópias possuem padrões de bits iguais.
_______________________ Comentários: conforme vimos em aula, eles criam cópias diferentes, inclusive seu padrão de bits (Errado).

Uma  variação  do  vírus  polimórfico  é  o  vírus  metamórfico  que,  diferentemente  do  vírus polimórfico – se reescreve completamente a cada infecção, podendo mudar seu tamanho e comportamento, aumentando a dificuldade de detecção. Aqui não tem muito o que falar: basta lembrar que o Vírus Polimórfico muda apenas a sua assinatura, mantendo sua funcionalidade, e o Vírus Metamórfico muda sua assinatura e sua funcionalidade.

(SUGEP – 2018 – Letra B) O vírus metamórfico muda a cada infecção, se reescrevendo completamente a cada iteração, aumentando a dificuldade de detecção.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).














Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





20
128




2.1.6 Vírus Stealth
INCIDÊNCIA EM PROVA: baixíssima 


Vocês já ouviram falar no avião Lockheed Blackbird SR-71? Ele é conhecido por ser o avião mais incrível de toda a história da aviação. Por que ele era tão especial, Diego? Galera, esse avião tinha uma característica muito peculiar: ele era praticamente invisível a radares, sendo capaz de refletir ou absorver ondas eletromagnéticas.
Por conta disso, ele ganhou a denominação de Avião Furtivo ou Stealth. Professor, o que isso tem a ver com a aula?

Pessoal,  vocês  acreditam  que  nós  temos  um  tipo  de  vírus  chamado  de  Vírus  Stealth?
Também
chamado de Vírus Furtivo, eles são projetados explicitamente para não serem detectados pelo antivírus
, possuindo a capacidade de se remover da memória do computador temporariamente para evitar que o antivírus o detecte. Da mesma forma que o avião stealth era capaz de se esconder de radares, o vírus stealth é capaz de se esconder de antivírus.

(TCU – 2015) O vírus do tipo stealth, o mais complexo da atualidade, cuja principal característica é a inteligência, foi criado para agir de forma oculta e infectar arquivos do Word e do Excel. Embora seja capaz de identificar conteúdos importantes nesses tipos de  arquivos  e,  posteriormente,  enviá-los  ao  seu  criador,  esse  vírus  não  consegue empregar técnicas para evitar sua detecção durante a varredura de programas antivírus.
_______________________ Comentários: conforme vimos em aula, a questão trata – na verdade – dos Vírus de Macro (Errado).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





21
128




2.1.7 Vírus Time Bomb INCIDÊNCIA EM PROVA: média 
Também conhecido como Vírus Bomba Relógio, trata-se de um vírus que – após infectar a máquina –  permanece  latente  (oculto),  apenas  se  replicando.
Além  disso, seu  código  malicioso  é programado para ser ativado em um determinado momento específico, executando sua carga útil. É comumente distribuído como anexo de e-mails e se instalam em computadores pela ação do usuário, ao executar o arquivo.

Os  Time  Bombs  se  instalam  silenciosamente  e  agem  apenas  em  datas  ou  momentos determinados, que são definidos pelo seu criador. Alguns vírus conhecidos foram:

 Sexta-feira 13 (ações danosas apenas nas sextas-feiras 13);
 I Love you (ação danosa apenas no dia dos namorados – 12 de junho)  Chernobyl (ação danosa apenas no dia do acidente nuclear – 25 de abril) 
(MTE – 2014) Quando ativado na máquina, a principal característica do vírus time bomb é a sua capacidade de remover o conteúdo do disco rígido em menos de uma hora.
_______________________ Comentários: conforme vimos em aula, a principal característica do Vírus Time Bomb é sua capacidade de ser ativado em momentos específicos – definidos pelo criador. Não há necessariamente nenhuma relação com a remoção do conteúdo do disco rígido em menos de uma hora (Errado).

(UFMT – 2014 – Letra D) Time bomb (ou bomba relógio) são vírus programados para se ativarem em determinados momentos, por exemplo em uma determinada data do ano.
_______________________ Comentários: conforme vimos em aula, essa é exatamente a definição desse tipo de vírus (Correto).

(UFES – 2018 – Letra D) O vírus do tipo Time Bomb é um programa ou script que toma posse do navegador, instala barra de navegação e exibe propagandas e janelas de pop- up até estourar a capacidade do navegador.
_______________________ Comentários: conforme vimos em aula, essa descrição não tem nenhuma relação com os vírus de bomba relógio (Errado).






Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





22
128




2.2 – WORM
INCIDÊNCIA EM PROVA: Altíssima 


Worm (ou Verme) é um programa capaz de se replicar automaticamente, enviando cópias de si mesmo de computador para computador.
Diferente dos vírus, ele não se propaga por meio da inclusão de cópias de si mesmo em outros programas ou arquivos através da rede, mas – sim – pela  exploração  automática  de  vulnerabilidades  existentes  em  programas  instalados  em computadores ou pela execução direta de suas cópias.

Pois é! Nesse primeiro parágrafo, nós temos dois pontos que necessitam de mais atenção: primeiro, worms podem – sim – ser executados diretamente, apesar de não ser a regra; segundo, worms não infectam outros arquivos, eles mesmos são os arquivos. Eles identificam computadores ativos na rede e exploram as conexões ou através da Internet por meio de correio eletrônico, redes sociais, bate papo, entre outros.

Worms são notadamente responsáveis por consumir muitos recursos, devido à grande quantidade de cópias de si mesmo que costumam propagar e, como consequência, degradam sensivelmente o desempenho de redes e podem lotar o disco rígido de computadores.
O processo de propagação ocorre em quatro fases: identificação dos computadores alvos; envio das cópias; ativação das cópias; e reinício do processo.

 Identificação de computadores-alvo: também conhecido como scanning, após infectar um computador, ele tenta se propagar e continuar o processo de infecção. Para tal, ele necessita identificar os computadores alvos para os quais tentará se copiar;

 Envio de cópias: após identificar os alvos, ele efetua cópias de si mesmo e tenta enviá-las para estes  computadores  anexadas  a  e-mails,  via  canais  de  IRC,  via  programas  de  troca  de mensagens instantâneas, incluídas em pastas compartilhadas em redes locais, etc;
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





23
128





 Ativação de cópias: após realizado o envio da cópia, ele necessita ser executado para que a infecção ocorra, o que pode acontecer imediatamente após ter sido transmitido, diretamente pelo usuário ou condicionado a algum evento específico (como a inserção de uma mídia).

Os worms são capazes de entrar em uma máquina sem qualquer interação do usuário. Em geral, podem ser obtidos automaticamente pela rede, recebidos por e-mail, baixados de páginas na web, pelo compartilhamento de arquivos, pelo uso de mídias removíveis infectadas, por meio de redes sociais, por meio de mensagens instantâneas, por conta de uma invasão de um hacker ou pela ação de outro código malicioso.

E quais são as ações maliciosas mais comuns de um worm?
Sua ação maliciosa mais comum consiste em  consumir  muitos  recursos,  devido  à  grande  quantidade  de  cópias  de  si  mesmo  que costumam  propagar  e,  como  consequência,  podem afetar  o  desempenho  de  redes  e  do computador.
Além disso, eles podem instalar outros códigos maliciosos no computador, desferir ataques na internet e enviar e-mails sem autorização.

Sobre ações maliciosas, é importante destacar novamente que worms não infectam arquivos.
Em resumo, os worms são programas autorreplicantes completos e autônomos que não necessitam de  um  programa  hospedeiro  para  se  propagar.  Diferentemente  dos  vírus,  esse  programa  não embute  cópias  de  si mesmo  em  outros  programas  ou  arquivos  –  além  de  não  precisarem  ser explicitamente executados para se propagar. Fechado?

worm = verme
alguns dizem que seu nome vem de:
write once run everywhere 
(Prefeitura de Apodi/RN – 2019) Os malwares são programas maliciosos cujo objetivo é roubar informações ou contaminar os computadores. O malware que tem a capacidade de se propagar na rede de computadores é o:

a) vírus  b) worm     c) netmal    d) trojan.
_______________________ Comentários: conforme vimos em aula, o malware que busca se propagar na rede de computadores é o Worm (Letra B).

(PC/MG – 2018) O tipo de ameaça à segurança de um computador que consiste em um programa completo que se replica de forma autônoma para se propagar para outros computadores é:

a) Worm     b) Vírus     c) Spyware   d) Spam.
_______________________ Comentários: conforme vimos em aula, programa completo que se replica de forma autônoma só pode ser Worm (Letra A).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





24
128




2.3 – BOT E BOTNET
INCIDÊNCIA EM PROVA: ALTA 


Bot é um programa que dispõe de mecanismos de comunicação com o invasor que permitem que ele seja controlado remotamente. Possui processo de infecção e propagação similar ao do Worm, ou seja, é capaz de se propagar automaticamente, explorando vulnerabilidades existentes em  programas  instalados  em  computadores.  A  comunicação  entre  o  invasor  e  o  computador infectado pode ocorrer via IRC, Servidor Web, Redes P2P, entre outros.

Ao se comunicar, o invasor pode enviar instruções para que ações maliciosas sejam executadas, como desferir ataques, furtar dados do computador infectado e enviar spam. Um computador infectado  por  um  bot  costuma  ser  chamado  de  zumbi, porque  ele  pode  ser  controlado remotamente e sem o conhecimento do seu dono. É chamado de Zumbi de Spam quando o bot instalado o transforma em um servidor de e-mails e o utiliza para o envio de spam.

Diegão, não entendi muito bem! Galera, imagine que você está aí todo feliz no seu computador, mas ele possui um bot zumbi instalado. Sabe  o  que  isso  significa? Significa que alguém pode estar controlando à distância o bot presente no seu computador, podendo realizar diversas atividades maliciosas.
Em alguns casos específicos, o hacker nem quer destruir nada em seu computador, ele quer apenas utilizá-lo para enviar e-mails spam para outras pessoas.

O  ideal  para  proteger  seus  dados  quando  se  detecta que  ele  está  infectado  por  um  bot  é desconectar o computador da rede o mais rápido possível.
Já uma Botnet é uma rede formada por centenas ou milhares de computadores zumbis e que permitem potencializar as ações danosas Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





25
128




executadas pelos bots. Quanto mais zumbis participarem da Botnet, mais potente serão as ações danosas. Compreendido?

O atacante que a controlar – além de usá-la para seus próprios ataques – também pode alugá- la  para  outras  pessoas  ou  grupos  que  desejem  que  uma  ação  maliciosa  específica  seja executada. As ações maliciosas mais comuns são: ataques de negação de serviço; propagação de códigos maliciosos (inclusive do próprio Bot); coleta de informações de outros computadores; envio de spam; camuflagem da identidade de hackers; entre outros.

O esquema simplificado apresentado a seguir exemplifica o funcionamento básico de uma botnet (rede de bots):

1. Um atacante propaga um tipo específico de bot na esperança de infectar e conseguir a maior quantidade possível de zumbis;

2. Os zumbis ficam então à disposição do atacante, agora seu controlador, à espera dos comandos a serem executados;

3. Quando o controlador deseja que uma ação seja realizada, ele envia aos zumbis os comandos a serem executados, usando, por exemplo, redes do tipo P2P ou servidores centralizados;

4. Os zumbis executam então os comandos recebidos, durante o período predeterminado pelo controlador;

5. Quando a ação se encerra, os zumbis voltam a ficar à espera dos próximos comandos a serem executados.

Em  suma:  bot  é  um  programa  que  possui  mecanismos  de  replicação,  infecção  e  ações maliciosas similares aos de um worm, entretanto dispõe de mecanismos de comunicação que permitem que ele seja controlado remotamente. É utilizado para realizar ações repetitivas, se fazendo passar por um ser humano, em que a máquina infectada passa a ser chamada de zumbi e sem o conhecimento do usuário pode ser utilizada para ações maliciosas.

bot
= diminutivo de robot = robô; net = rede;
bot = robô; botnet = rede de robôs 
(PF – 2014) Computadores infectados por botnets podem ser controlados remotamente bem como podem atacar outros computadores sem que os usuários percebam.
_______________________ Comentários: conforme vimos em aula, computadores infectados por botnets realmente podem ser controlados remotamente como podem atacar outros computadores sem serem notados (Correto).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





26
128




(TRE/SP – 2017) Em uma situação hipotética, um tipo de código malicioso foi detectado no TRE-SP e tinha a característica de ser controlado pelo invasor via processo de infecção e  propagação  automática.  Ele  explorava  diversas  vulnerabilidades  existentes  em programas instalados. Foi verificado, ainda, que a comunicação entre os infectados e o invasor ocorria de várias formas, via servidores Web, canais IRC, redes tipo P2P, entre outros  meios  e  eram  recebidos,  automaticamente,  pela  rede.  Um  Programador  de Sistemas  analisou  estas  características  e  observou que  os  computadores  atingidos ficavam  semelhantes  a  zumbis  (zombie  computer)  pelo  fato  de  serem  controlados remotamente, sem o conhecimento de seu usuário.

Trata-se de um código malicioso conhecido como:

a) Trojan DoS.
b) Screenlogger.
c) Rootkit.
d) Keylogger.
e) Bot.
_______________________ Comentários:  pode  ser  controlado  pelo  invasor,  pode  se  propagar  automaticamente,  explora  diversas  vulnerabilidades, computadores atingidos ficavam semelhantes a zumbis – todas são características de um Bot (Letra E).

(Prefeitura de Teresina/PI – 2016) Um funcionário de uma empresa percebeu que seu computador estava sendo controlado remotamente sem seu consentimento, quando foi notificado pelo administrador da rede que, a partir de seu computador, estavam sendo enviados  spams,  realizados  ataques  de  negação  de  serviço  e  propagação  de  outros códigos maliciosos.

Com  base  nestas  características  e  ações,  conclui-se  que  o  computador  deve  estar infectado por um:

a) vírus.
b) rootkit.
c) keylogger.
d) spyware.
e) bot.
_______________________ Comentários: permite controlar remotamente um computador infectado sem consentimento do usuário, permite enviar spams, realizar ataques de negação de serviço e propagar outros códigos maliciosos – todas são características de um Bot (Letra E).




Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





27
128




2.4 – TROJAN HORSE
INCIDÊNCIA EM PROVA: ALTA 


O Trojan é um software malicioso que age por meio da utilização do princípio do Cavalo de Troia. Quem se lembra dessa história? Os gregos queriam invadir a cidade de Troia, no entanto essa cidade era cercada por uma grande muralha. Como a invasão de uma cidade fortificada era bastante complexa, os gregos tiveram a ideia de dar um presente aos troianos. O que era, Diego? Era uma grande estátua de madeira no formato de um cavalo, mas tinha uma particularidade...

Dentro do cavalo de madeira estavam diversos soldados gregos. Os troianos acharam que os gregos estavam sendo corteses, aceitaram o presente e levaram o cavalo para dentro da cidade fortificada.
À  noite,  os  soldados  gregos  que  estavam  escondidos dentro  do  cavalo  saíram,  dominaram  os sentinela  e  possibilitaram  a  entrada  do  exército  grego,  levando  a  cidade  à  ruína.
Resumo  da
história: muito cuidado com os “presentes de grego” que vocês aceitam!

O Trojan Horse – também chamado de Cavalo de Troia – é um programa que, além de executar as  funções  para  as  quais  foi  aparentemente  projetado,  também  executa  outras  funções, normalmente maliciosas, e sem o conhecimento do usuário. Ele é enviado se fazendo passar por um aplicativo útil, mas é capaz de abrir portas de comunicação de um computador para que a máquina possa ser invadida ou monitorada através da Internet.

Em  outras  palavras,  eles podem  ser  instalados  por  atacantes  que  –  após  invadirem  um computador – alteram programas já existentes para que, além de continuarem a desempenhar Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





28
128




as funções originais, também executem ações maliciosas. Exemplos de trojans são programas que você recebe ou obtém de sites na Internet e que parecem ser apenas cartões virtuais animados, álbuns de fotos, jogos e protetores de tela, entre outros.

Estes programas, geralmente, consistem de um único arquivo e necessitam ser explicitamente executados para que sejam instalados no computador – ao contrário dos vírus, ele não se replica automaticamente. O Cavalo de Troia trabalha com um modo de infecção que envolve despertar a curiosidade do usuário para que este o execute e, assim, possa infectar e comprometer o sistema.

Professor, agora estou com medo – o que eu tenho que fazer para evitar que um Trojan seja instalado  no  meu  computador  uma  vez  que você disse que ele parece inofensivo? Pois é!
Quem  é  mais  velho  como  eu  (31  anos)  se identificará  com  a  imagem  ao  lado.  Você acessava um site e, não mais que de repente, aparecia um pop-up na tela informando que você havia ganhado um prêmio. Para buscá- lo, bastava clicar no botão apresentado. Esse era  o  momento  em  que  você  fazia  o download   de   um   trojan   capaz   de comprometer   a   segurança   do   seu computador.   Então   prestem   bastante atenção  em  tudo  que  vocês  baixam  na internet,  em  especial  aqueles  arquivos recebidos por e-mail e não baixem softwares piratas! Estão vendo agora como informática é maravilhoso?  Diz  aí  no  fórum  se  não  é  a matéria mais legal da vida?
Se você não acha,
mente no fórum um pouquinho pelo menos para eu ficar feliz :) 

Há diferentes tipos de trojans, classificados de acordo com as ações maliciosas que costumam executar ao infectar um computador. Ahhh... eles podem ser considerados um tipo de vírus!

TIPO DE
TROJAN
DESCRIÇÃO
Trojan
Downloader
Instala outros códigos maliciosos, obtidos de sites na Internet.

Trojan
Dropper
Instala outros códigos maliciosos, embutidos no próprio código do trojan.
Trojan
Backdoor
Inclui backdoors, possibilitando o acesso remoto do atacante ao computador.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





29
128




Trojan
DoS
Instala ferramentas de negação de serviço e as utiliza para desferir ataques.
Trojan
Destrutivo
Altera ou apaga arquivos e diretórios, formata o disco rígido e pode deixar o computador fora de operação.
Trojan
Clicker
Redireciona a navegação do usuário para sites específicos, com o objetivo de aumentar a quantidade de acessos a estes sites ou apresentar propagandas Trojan
Proxy
Instala  um  servidor  de  proxy,  possibilitando  que  o computador  seja  utilizado  para  navegação anônima e para envio de spam.
Trojan
Spy
Instala programas spyware e os utiliza para coletar informações sensíveis, como senhas e números de cartão de crédito, e enviá-las ao atacante.
Trojan
Banker
Coleta dados bancários do usuário através da instalação spyware que são ativados quando sites de Internet Banking são acessados – similar ao Trojan Spy, mas com objetivos específicos.

trojan = troia; horse = cavalo trojan horse = cavalo de troia 
(TRT/PE – 2018) Considere o texto abaixo:

Um grupo de especialistas em segurança encontrou um novo tipo de malware, que está se espalhando  massivamente  por  meio  do  Facebook  Messenger.  Trata-se  do  Digmine,  um malware que usa sistemas infectados para extrair a criptomoeda Monero. Esse malware é enviado às vítimas como um link para um arquivo de vídeo, quando na verdade é um script executável  que  afeta  as  versões  desktop  e  web  do  Facebook  Messenger,  usando  o navegador Google Chrome para minerar a moeda Monero no computador.

(Adaptado de: https://guiadobitcoin.com.br/) 
Esse tipo de malware, que parece ser uma coisa (vídeo), mas na realidade é outra (script de mineração), é categorizado como:

a) trojan.
b) backdoor.
c) adware.
d) rootkit.
e) ransomware.
_______________________ Comentários: trata-se de um malware que parece ser uma coisa, mas é outra? Como um presente de grego? Só pode ser um Trojan (Letra A).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





30
128




2.5 – SPYWARE
INCIDÊNCIA EM PROVA: Altíssima 


Um spyware é um software espião, capaz de violar a privacidade das informações de usuários, coletando dados da máquina ou da rede e disponibilizando-as a terceiros. Pode ser usado tanto de forma legítima quanto maliciosa, dependendo de como é instalado, das ações realizadas, do tipo de informação monitorada e do uso que é feito por quem recebe as informações coletadas. Pode ser considerado de uso:

 Legítimo:  quando  instalado  em  um  computador  pessoal,  pelo  próprio  dono  ou  com consentimento deste, com o objetivo de verificar se outras pessoas o estão utilizando de modo abusivo ou não autorizado.

 Malicioso:  quando  executa  ações  que  podem  comprometer  a  privacidade  do  usuário  e  a segurança do computador, como monitorar e capturar informações referentes à navegação do usuário ou inseridas em outros programas (por exemplo, conta de usuário e senha).

Como esse é um dos malwares que mais cai em prova, eu resolvi fazer uma consolidação das
principais definições encontradas em prova. Dessa forma, pode-se dizer que um Spyware é:

DEFINIÇÕES DE SPYWARE Um programa automático de computador que recolhe informações sobre o usuário e as envia a uma entidade externa na Internet, sem o conhecimento/consentimento do usuário.
Um software malicioso que recolhe informações sobre o usuário do computador e as transmite para alguém externo, sem conhecimento do usuário.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





31
128




Um  programa  espião  que  monitora  as  atividades  de  um  sistema  e  envia  as  informações  coletadas  para  os invasores/terceiros.
Uma praga virtual que se aloja em uma máquina e, quando em ação, produz uma falsa impressão de normalidade, obtendo dados importantes (Ex: senhas).
Um programa automático instalado em um computador, que têm como finalidade capturar informações sobre o usuário e transmiti-las externamente sem a sua prévia autorização.
Uma  aplicação  que  recolhe automaticamente  dados  sobre  atividades  e  hábitos  de um  usuário  na internet  e transmite essa informação a uma entidade externa.

Informações adicionais: assim como os worms e diferentemente dos vírus, os spywares precisam ser explicitamente executados pelo usuário para infectar uma máquina (a infecção de vírus é feita  pela  execução  do  arquivo  hospedeiro).  Ademais,  para  combatê-los,  recomenda-se  a utilização de um Anti-Spyware, que são softwares que se destinam a detectar e remover spywares.
Bacana? Os tipos mais comuns de spywares são os keyloggers, screenloggers, adwares e sniffers.

spy
= espião
spyware = software espião 
(PC/ES - 2012) Ter receio de se fazer compras on-line ou de se acessar o sítio de um banco pela  Internet  justifica-se,  atualmente,  pela  possibilidade  de  perda  de  privacidade causada por softwares maliciosos capazes de enviar dados privativos referentes a senhas de  acesso  a  contas  bancárias  e  números  de  cartão  de  crédito  a  outras  máquinas conectadas remotamente na Internet.
_______________________ Comentários: conforme vimos em aula, a questão trata do spyware (Correto).

(TCE-SP - 2015) Dentre os tipos de malwares, o spyware se caracteriza por:

a) capturar as teclas digitadas no computador infectado e enviar as informações para o invasor.

b) explorar falhas do sistema operacional para controlar o computador infectado.

c) permitir o acesso contínuo ao computador infectado.

d) propagar-se automaticamente pela rede enviando cópias para outros computadores.

e)  monitorar  as  atividades  de  um  sistema  e  enviar  as  informações  coletadas  para  o invasor.
_______________________ Comentários: conforme vimos em aula, ele monitora as atividades de um sistema e envia as informações coletadas para o invasor. A primeira opção trata do Keylogger, que é um tipo de Spyware, logo também poderia ser uma resposta. No entanto, a última opção é “mais correta”. Concurseiro tem que se acostumar com isso infelizmente (Letra E).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





32
128




2.6 – BACKDOOR
INCIDÊNCIA EM PROVA: ALTA 


Backdoor (em português, Porta dos Fundos) é um programa que permite o retorno de um invasor  a  um  computador  comprometido,  por  meio  da  inclusão  de  serviços  criados  ou modificados para este fim . Pode ser incluído pela ação de outros códigos maliciosos, que tenham previamente infectado o computador, ou por atacantes, que exploram vulnerabilidades existentes nos programas instalados no computador para invadi-lo.

Após  incluído,  ele  é  utilizado  para  assegurar  o  acesso  futuro  ao  computador  comprometido, permitindo  que  ele  seja  acessado  remotamente, sem  que  haja  necessidade  de  recorrer novamente aos métodos utilizados na realização da invasão ou infecção e, na maioria dos casos, sem que seja notado . Há casos, inclusive, de Backdoors incluídos propositalmente por fabricantes de programas, sob alegação de necessidades administrativas. Sinistro, não é?

Esses casos constituem uma séria ameaça à segurança de um computador que contenha um destes programas instalados, pois – além de comprometerem a privacidade do usuário – também podem ser usados por invasores para acessarem remotamente computadores.
Em suma: esse software malicioso  abre  as  Portas  TCP  para  que  seja  possível  que  o  invasor  acesse  o  computador remotamente.
Professor, qual é a diferença entre Backdoor e Bot? São muitas...

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





33
128






Backdoors  são  obtidos  somente  pela  inserção  por  um invasor  ou  pela  ação  de  outro  código malicioso – bots podem ser obtidos por diversas outras maneiras. Bots são instalados pela sua execução explícita; backdoors são instalados via execução de outro código malicioso.
Além disso,
backdoors não se propagam! Por fim, backdoors buscam possibilitar o retorno do invasor e procuram se manter escondidos; essas não são ações maliciosas comuns de um bot!

back = fundo; door = porta backdoor = porta dos fundos 
(COMPESA – 2018) Os códigos maliciosos fazem inúmeras vítimas e provocam os mais variados prejuízos. Quando esse código se instala na máquina da vítima para permitir conexões remotas, funcionando como um controle remoto, é classificado como:

a) Adware.
b) Spyware.
c) Keylogger.
d) Worm.
e) Backdoor.
_______________________ Comentários:  dentre  os  códigos  maliciosos  apresentados,  aquele que  permite  conexões  remotas  funcionando  como  um controle remoto é o backdoor (Letra E).

(IBGE – 2017) Curioso, um usuário baixou e instalou em seu computador um suposto jogo erótico que viu em um site desconhecido. O jogo era, na verdade, um software que passou a permitir remotamente o controle do computador do usuário. É possível concluir que esse comportamento é típico de um malware denominado:

a) vírus
b) keylogger
c) adware
d) worm
e) backdoor
_______________________ Comentários: conforme vimos em aula, esse comportamento é típico de um backdoor (Letra E).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





34
128




2.7 – ROOTKIT



Rootkit é um conjunto de programas e técnicas que permite esconder e assegurar a presença de um invasor ou de outro código malicioso em um computador comprometido. É muito importante ressaltar que o nome rootkit não indica que os programas e as técnicas que o compõem são usadas para obter acesso privilegiado a um computador, mas sim para mantê-lo . O conjunto de
programas e técnicas fornecido pelos rootkits pode ser usado para:

 Remover evidências em arquivos de logs (arquivos de registro de ações de um sistema);
 Instalar códigos maliciosos (ex: backdoors), para assegurar acesso futuro à máquina infectada;
 Esconder atividades/informações (Ex: arquivos, diretórios, processos, chave de registro, etc);
 Mapear potenciais vulnerabilidades em outros computadores, através de varreduras na rede;
 Capturar informações da rede do computador pela interceptação de tráfego.

Rootkits  inicialmente  eram  usados  por  atacantes  que,  após  invadirem  um  computador,  os instalavam para manter o acesso privilegiado, sem precisar recorrer novamente aos métodos utilizados na invasão, e para esconder suas atividades do responsável e/ou dos usuários do computador. Apesar de ainda serem bastante usados por atacantes, os rootkits atualmente têm sido também tem uma outra função.

Eles são utilizados e incorporados por outros códigos maliciosos para ficarem ocultos e não serem detectados pelo usuário e nem por mecanismos de proteção. Galera, os rootkits são um dos tipos de malware mais sofisticados que existem atualmente. Por anos, as soluções de segurança têm lutado contra a sua detecção e remoção, principalmente porque eles comprometem o sistema operacional. Como é, professor?

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





35
128




Sim, eles comprometem o sistema operacional em um nível tão profundo que podem camuflar sua presença tanto das soluções antimalware quanto do próprio sistema operacional. Ao contrário do malware  tradicional,  os rootkits  introduzem  uma  falha  fundamental  nos  computadores que infectam:
eles não comprometem arquivos ou pastas – em vez disso, eles alteram tudo o que o sistema operacional informa de acordo com as necessidades do criador.

Quando  algum  sistema  operacional  efetua  um  pedido  de  leitura  de  um  arquivo,  o  rootkit intercepta os dados que são requisitados e faz uma filtragem dessa informação, deixando o sistema  ler  apenas  arquivos  não  infectados. Desta  forma,  o  antivírus  ou  qualquer  outra ferramenta antimalware fica impossibilitada de encontrar o arquivo malicioso no computador – por essa razão, ele tão difícil de detectar.

Ao  utilizar  um  rootkit,  um  criminoso  tem  privilégios  totais  de  administrador  para  o  seu computador  e  softwares ,  convenientemente  acessando  logs,  monitorando  sua atividade, roubando informações e arquivos privados, e mexendo em suas configurações. Sem você saber, todas as suas senhas e informações poderão ser roubadas. É interessante enfatizar também que ele geralmente é formado por um conjunto de arquivos executáveis.



Alunos  sempre  me  perguntam  no  fórum  qual  é  a  diferença  entre  rootkit  e  backdoor.  Eles realmente são bastante parecidos em relação à obtenção, instalação e propagação. No entanto, os rootkit  são  bem  mais  avançados  e  complexos  –  trata-se  de  um  conjunto  de  funcionalidades maliciosas capaz de camuflar a presença do invasor, apagar evidências, remover logs e infectar o núcleo do sistema operacional, geralmente implicando a formatação da máquina do usuário.

Root
= Administrador (Linux) Rootkit = Kit do Administrador 
(IDAM - 2019) “A capacidade de se esconder permite que este tipo de malware permaneça no  sistema  da  vítima  por  meses,  às  vezes  até  anos, deixando  que  um  hacker  use  o computador para o que bem entender. Mesmo uma máquina que não contém informações valiosas, o que é pouco comum, pode ser útil para produzir bitcoins (moeda digital), enviar spam e participar de ataques DDoS.” Essa é uma definição do malware denominado:

a) adware    b) spyware   c) keylogger   d) rootkit _______________________ Comentários:  capacidade  de  se  esconder,  permitindo  que  o  hacker  use  o  computador  para  o  que  bem  entender  são características típicas de um rootkit (Correto).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





36
128




2.8 – TABELA COMPARATIVA 
RESUMO DE Códigos maliciosos 
VÍRUS

WORM

BOT

TROJAN

SPYWARE

BACKDOOR

ROOTKIT

FORMA DE OBTENÇÃO
Recebido automaticamente pela rede X X
Recebido por e-mail
X X X X X
Baixado de sites na Internet X X X X X
Compartilhamento de arquivos X X X X X
Uso de mídias removíveis infectadas X X X X X
Redes sociais
X X X X X
Mensagens instantâneas X X X X X
Inserido por um invasor X X X X X X
Ação de outro código malicioso X X X X X X
FORMA DE INSTALAÇÃO
Execução de um arquivo infectado X
Execução explícita do código malicioso X X X X
Via execução de outro código malicioso X X
Exploração de vulnerabilidades X X   X X
FORMA DE PROPAGAÇÃO
Insere cópia de si próprio em arquivos X
Envia cópia de si próprio automaticamente pela rede X X
Envia cópia de si próprio automaticamente por email X X
Não se propaga
X X X X
AÇÕES MALICIOSAS MAIS COMUNS Altera e/ou remove arquivos X   X   X
Consome grande quantidade de recursos X X
Furta informações sensíveis X X X
Instala outros códigos maliciosos X X X   X
Possibilita o retorno do invasor X X
Envia spam e phishing X
Desfere ataques na Internet X X
Procura se manter escondido X    X X X
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA ==12b2d8==






37
128




3 – OUTROS MALWARES
3.1 – RANSOMWARE
INCIDÊNCIA EM PROVA: ALTA 


Esse tem começado a cair com mais frequência recentemente em provas de concurso, mas é minha aposta nesses novos tempos de moedas digitais. O Ransomware é um tipo de código malicioso  que  torna  inacessíveis  os  dados  armazenados  em  um  equipamento,  geralmente utilizando criptografia, e que exige pagamento de um resgate (ransom, em inglês) para restabelecer o acesso ao usuário – trata-se de uma espécie de extorsão virtual.

Ele pode se propagar de diversas formas, embora as mais comuns sejam: através de correios eletrônicos com o código malicioso em anexo ou que induzam o usuário  a seguir um link; ou explorando vulnerabilidades em sistemas operacionais comprometidos que não tenham recebido as devidas atualizações de segurança. Atualmente, existem dois tipos básicos da praga virtual ransomware:

 Ransomware Locker: impede que você acesse o equipamento infectado.
 Ransomware Crypto: impede que você acesse dados no equipamento infectado.

Esse segundo tipo utiliza criptografia para impedir que o usuário tenha acesso aos dados. Além de infectar o equipamento, ele também costuma buscar outros dispositivos conectados, locais ou em rede, e criptografá-los também. Para se proteger, recomenda-se manter o sistema operacional e os programas instalados com todas as atualizações aplicadas; ter um antivírus instalado; e ser cuidadoso ao clicar em links ou abrir arquivos.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





38
128




Fazer  backups  regularmente  também  é  essencial  para proteger  os  seus  dados,  pois  –  se  seu equipamento for infectado – a única garantia de que você conseguirá acessá-los novamente é possuir backups atualizados.
Em geral, o pagamento é feito utilizando moedas digitais (Ex:
Bitcoin), de modo que se torne não-rastreável, e infelizmente não garante o restabelecimento do acesso aos dados.

ransom = resgate
ransomware = software de resgate 
(SERES/PE – 2017) Praga virtual que informa, por meio de mensagem, que o usuário está impossibilitado de acessar arquivos de determinado equipamento porque tais arquivos foram  criptografados  e  somente  poderão  ser  recuperados  mediante  pagamento  de resgate denomina-se:

a) ransomware.
b) trojan.
c) spyware.
d) backdoor.
e) vírus.
_______________________ Comentários: conforme vimos em aula, trata-se do ransomware (Letra A).

(PC/BA – 2018) Uma das formas de atuação do ransomware, um dos códigos maliciosos mais difundidos atualmente, é:

a) capturar as senhas digitadas no computador e enviar para o hacker.
b) criptografar os dados do disco rígido e solicitar o pagamento de resgate.
c) enviar várias cópias de uma mensagem de e-mail utilizando os seus contatos.
d) instalar diversos arquivos de imagens para lotar o disco rígido.
e) mostrar uma mensagem com propaganda no navegador Internet.
_______________________ Comentários: conforme vimos em aula, ele criptografa os dados do disco rígido e solicita o pagamento de resgate (Letra B).

(Polícia Federal – 2018) Formatos comuns de arquivos, como, por exemplo, .docx ou .xlsx,  são  utilizados  como  vetor  de  infecção  por  ransomware,  um  tipo  de  software malicioso que encripta os dados do usuário e solicita resgate.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





39
128




3.2 – KEYLOGGERS
INCIDÊNCIA EM PROVA: média 


Galera, vocês se lembram que nós vimos os spywares? Pois é, keylogger é um tipo de spyware capaz de capturar e armazenar as teclas digitadas pelo usuário no teclado do computador e enviá-las a um invasor
. Imaginem que tudo que vocês digitam no teclado é armazenado pelo software malicioso  e  enviado  para  o  atacante,  que  pode  eventualmente  capturar  senhas  ou  outras informações relevantes.

Criado inicialmente com a intenção de ser utilizado para auxiliar o suporte técnico e fiscalização, ele
adquire  uma  característica  maliciosa  quando  é  integrado  a  malwares  e  usado  para coletar informações pessoais. O uso ilícito tem o objetivo de coletar dados como nomes de usuário e senhas de contas de e-mail, sites de relacionamento, mensageiros instantâneos e qualquer outro serviço que precise de senha para se conectar, inclusive dados de acesso às contas bancárias.

Sua ativação, em muitos casos, é condicionada a uma ação prévia do usuário, como o acesso a um site específico de comércio eletrônico ou de Internet Banking.
Para aumentar a proteção dos seus clientes, alguns bancos online utilizam a tecnologia do teclado virtual, com recursos  que  reduzem  a  probabilidade  de  sucesso  desses softwares
. A ideia é que caracteres não sejam digitados pelo teclado físico e, sim, clicados com o auxílio do mouse em um teclado virtual que aparece na tela do computador.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





40
128




key = tecla; logger = registrador keylogger = registrador de tecla 
(CAU/MG – 2019) Qual é o software malicioso criado para gravar informações digitadas por  um  determinado  usuário  no  teclado  de  um  computador,  a  fim  de  obter  dados sigilosos?

a) Keylogger
b) Spam
c) Firewall
d) Scan
_______________________ Comentários: conforme vimos em aula, trata-se do Keylogger (Letra A).

(TRT/10 – 2019) “Programa que armazena todas as informações que um usuário digitou em um micro infectado por esse tipo de programa”. A afirmativa se refere a:

a) Adware.
b) Spyware.
c) Keylogger.
d) Screenlogger.
_______________________ Comentários: conforme vimos em aula, trata-se do Keylogger (Letra C).

(TRT-BA – 2013) Um site de segurança publicou uma notícia informando sobre um tipo de  e-mail  falso  que  vem  atacando  as  redes  sociais. Trata-  se  de  um  falso  aviso  de segurança  informando  que  a  conta  será  bloqueada  caso  não  seja  atualizada.  Com aparência semelhante à do Facebook, este tipo de e-mail oferece um link para que a pessoa acesse uma página da rede social para iniciar o processo de atualização dos dados. Na verdade, o que ocorre ao clicar no link é a instalação de um spyware, capaz de capturar e armazenar as teclas digitadas pelo usuário no teclado do computador. O spyware capaz de realizar o que está sublinhado no texto, de acordo com a cartilha de segurança para internet do CERT.BR, é denominado:

a) Adware.
b) Keylogger.
c) Rootkit.
d) Bot.
e) Trojan.
_______________________ Comentários: conforme vimos em aula, trata-se de um Keylogger (Letra B).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





41
128




3.3 – SCREENLOGGERS
INCIDÊNCIA EM PROVA: média 


Trata-se também de um spyware – similar ao keylogger – capaz de armazenar a posição do cursor e a tela apresentada no monitor nos momentos em que o mouse é clicado, ou a região que circunda a posição onde o mouse é clicado. Vocês se lembram que uma das soluções contra os keyloggers foi a utilização de teclados virtuais? Pois é, o screenlogger foi criado principalmente para capturar as teclas digitadas pelos usuários nesses teclados virtuais .

Professor, como ele faz isso?
Ele permite capturar uma foto instantânea da tela (print screen) e assim observar uma sequência de cliques. Ele era bastante utilizado por atacantes para capturar as teclas digitadas pelos usuários em teclados virtuais, disponíveis principalmente em sites de internet Banking. Por que era utilizado? Porque, hoje em dia, é mais raro utilizar teclados virtuais e porque atualmente há diversas maneiras de impedir esse tipo de praga virtual.

screen
= tela; logger = registrador screenlogger = registrador de tela 
(TRT/AMAZONAS  –  2017) Spyware  é  um  programa  projetado  para  monitorar  as atividades de um sistema e enviar as informações coletadas para terceiros. Existem tipos específicos deste programa, como o que é capaz de armazenar a posição do cursor e a tela apresentada no monitor, nos momentos em que o mouse é clicado, ou a região que circunda a posição onde o mouse é clicado. Este tipo de spyware é denominado de:

a) KeyLogger
b) Mouselogger
c) Adware
d)  Screenlogger
_______________________ Comentários: conforme vimos em aula, trata-se do Screenlogger (Letra D).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





42
128




3.4 – ADWARES
INCIDÊNCIA EM PROVA: ALTA 


Trata-se de um spyware projetado especificamente para apresentar propagandas. Pode ser usado para fins legítimos, quando incorporado a programas e serviços, como forma de patrocínio ou retorno financeiro para quem desenvolve programas livres ou presta serviços gratuitos. Também pode ser usado para fins maliciosos, quando as propagandas são direcionadas de acordo com a navegação do usuário sem que este saiba que tal monitoramento está sendo feito.

É  um
programa  executado  de  forma automática  e  geralmente  instalado  sem  o consentimento  do  usuário   durante  a instalação de outro software . É utilizado para
divulgação de links publicitários, muitas vezes através de pop-ups.

Quem nunca fez download de um software, não prestou atenção nas instruções de instalação e acabou  instalando  algum  outro  software  de propaganda que não gostaria de ter instalado?
Prestem muita atenção na instalação, como na imagem ao lado!

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





43
128




Em  suma: consiste  em  um  programa  projetado  para  exibir  propagandas  e  anúncios normalmente sem a autorização do usuário, tornando o computador mais lento e a navegação mais incômoda. Geralmente vêm em formato de diversos pop-ups e notificações inseridas em outro programa  (em  geral,  um  navegador)  e  pode  ser  considerado  um  malware  na  hipótese  de  sua propaganda variar de acordo com hábitos de navegação do usuário.

ad (
advertisement) = propaganda ou anúncio adware = software de propaganda 
(DETRAN/MA – 2018) Após acessar um website para o download de músicas da internet foi notado que o navegador internet passou a mostrar janelas pop-up com propagandas de forma infinita, ou seja, após o fechamento de uma janela, outra é apresentada em seguida de forma contínua. Esse efeito é característico do ataque do malware conhecido como:

a) adware.
b) spyware.
c) botnet.
d) worm.
e) rootkit.
_______________________ Comentários: janelas de pop-up com propagandas de forma infinita e apresentada de forma contínua é uma característica típica de um adware (Letra A).

(INPI  –  2013) A  principal  atividade  de  programas  com  códigos  maliciosos  e  que funcionam  na  função  de  keylogger  é  apresentar  propagandas  não  solicitadas  pelo usuário, direcionando-o a sítios maliciosos.
_______________________ Comentários: conforme vimos em aula, a questão trata de adwares e, não, keyloggers (Errado).










Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





44
128




3.5 – SNIFFER
INCIDÊNCIA EM PROVA: baixa 


Por  padrão,  computadores  em  uma  mesma  rede  “farejam”  e  respondem  somente  pacotes endereçados a eles. No entanto, é possível utilizar um analisador de pacotes de dados chamado sniffer capaz de monitorar, interceptar e registrar tráfego de dados em segmentos de rede de computadores.
Esse software pode ser utilizado de forma legítima ou pode ser utilizado de forma maliciosa. Diego, você pode explicar melhor? Claro...

Ele é utilizado de forma legítima por administradores de redes, para detectar problemas, analisar desempenho  e  monitorar  atividades  maliciosas  relativas  aos  computadores  ou  redes  por  eles administrados.
Ele  também  pode  ser  utilizado  por  atacantes,  para  capturar  informações sensíveis, como senhas, números de cartão de crédito e o conteúdo de arquivos confidenciais que estejam trafegando por meio de conexões inseguras, ou seja, sem criptografia.

Nesse  último  caso,  dizemos  que  ele  está  configurado  em  modo  promíscuo. Notem  que  as informações capturadas por este software malicioso são armazenadas na forma como trafegam, ou seja, informações que trafegam criptografadas apenas serão úteis ao atacante se ele conseguir decodificá-las. Os hackers costumam colocar sniffers em locais que ofereçam redes wi-fi inseguras, como cafeterias, hotéis e aeroportos.

Um sniffer é programa que age monitorando o tráfego na rede, através da captura de pacotes de dados, em busca de informações sensíveis como o endereço dos sites acessados, senhas de acesso, e-mails, etc. No entanto, é bom enfatizar que eles não são necessariamente maliciosos.
Este tipo de software é usado com frequência para monitorar e analisar o tráfego de rede para detectar problemas e manter um fluxo eficiente.

Por outro lado, se utilizados de má-fé, eles podem capturar tudo o que passa por eles, inclusive senhas e nomes de usuários não criptografados. Além disso, um sniffer pode ser instalado em qualquer computador conectado a uma rede local. Ele não precisa ser instalado no próprio aparelho que se deseja monitorar. Em outras palavras, ele pode permanecer oculto durante a conexão em um outro computador conectado à rede local.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





45
128





sniff = farejar
sniffer = farejador

(TCE/SP – 2015 ) Os Sniffers, utilizados para monitorar o tráfego da rede por meio da interceptação de dados por ela transmitidos, não podem ser utilizados por empresas porque violam as políticas de segurança da informação.
_______________________ Comentários: eles não só podem como geralmente são utilizados assim desde que com boa-fé (Errado).

(CRF/PR – 2019) Os  programas  que  são considerados  como muito  parecidos  com  os spywares  e  que  têm  como  função  principal  interceptar e registrar dados trafegados na rede são os:

a) hijackers.
b) vírus time bomb.
c) sniffers.
d) spams.
e) de engenharia social.
_______________________ Comentários: conforme vimos em aula, o programa responsável por interceptar e registrar dados trafegados é o sniffer (Letra C).

(BANESTES – 2015) Um SNIFFER de rede é um programa que:

a)  Põe  em  risco  as  informações  que  trefegam  em  rede,  pois  captura  pacotes  desse ambiente.

b) Não põe em risco as informações que trefegam em rede, pois protege os pacotes desse ambiente.

c) Não põe em risco as informações que trefegam em rede, pois criptografa em IPSEC os pacotes desse ambiente.

d) Põe em risco as informações que trefegam em rede, apesar de criptografar em HTTPS os pacotes desse ambiente.

e) Não pode ser utilizado em protocolos TCP/IP.
_______________________ Comentários: (a) Correto, ele pode por as informações em risco por capturar pacotes de dados; (b) Errado, ele compromete pacotes de dados; (c) Errado, ele não criptografa pacotes de dados; (d) Errado, ele não criptografa pacotes de dados; (e) Errado, ele pode – sim – ser utilizado com protocolos da arquitetura TCP/IP (Letra A).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





46
128




3.6 – BOMBAS LÓGICAS INCIDÊNCIA EM PROVA: baixa 


Trata-se de um software malicioso normalmente instalado por um usuário autorizado, como um administrador da rede, que o mantém no sistema deixando-o programado para causar danos
(como excluir arquivos importantes) em um determinado evento, como – por exemplo – um código que monitora o sistema de pagamentos de uma empresa e deleta arquivos críticos para a organização caso um determinado funcionário seja demitido.

Imaginem um camarada que tenha sido demitido por qualquer que seja a razão e, insatisfeito, decide criar uma bomba lógica que apagará arquivos importantes caso ele seja excluído da base de dados da empresa (significando a sua demissão) – de forma que ninguém desconfie que ele foi o responsável pelos danos causados pelo software malicioso.
Esse é geralmente o tipo de situação em que esse malware aparece. Hora de praticar...

(CRQ/SP – 2011) O programador escreve uma parte do código e o insere secretamente no  sistema  operacional  para  utilizá-lo  em  represália  a  um  possível  afastamento involuntário  do  ambiente  de  trabalho.  Dessa  forma, a  execução  bem-sucedida  do programa  depende  desse  programador  alimentá-lo  diariamente,  por  meio  de  uma senha.

O tipo de ataque descrito acima é conhecido por:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





47
128





a) alçapão.
b) conexão impostora.
c) transbordo do buffer.
d) código móvel.
e) bomba lógica.
_______________________ Comentários: como a execução bem-sucedida do programa depende de o programador alimentá-lo diariamente, existe uma dependência lógica, logo se trata de uma bomba lógica (Letra E).

(CRO/AC  –  2019) A  bomba  lógica  tem  como  característica  principal  enviar  várias requisições de informação para um sistema de computação, com o objetivo de paralisá- lo.
_______________________ Comentários: na verdade, essa é a característica principal de um ataque chamado DDoS (Errado).

(CONRERP/2R – 2019) A bomba lógica é um tipo de código malicioso embutido no malware que consegue fazer com que o computador trave ou se torne muito lento, de forma a interromper o trabalho do usuário. Contudo, esse tipo de praga virtual não consegue eliminar dados ou arquivos.
_______________________ Comentários: conforme vimos em aula, essa é uma característica de um worm e, não, de uma bomba lógica (Errado).



















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





48
128




3.7 – EXPLOITS
INCIDÊNCIA EM PROVA: baixíssima 


Trata-se  de  uma  ferramenta  criada  por  hackers  para permitir  explorar  vulnerabilidades  ou brechas de segurança conhecidas de sistemas e assim permitir que atacantes possam praticar ações  de  invasões  sem  conhecimentos  avançados.
Eles  geralmente  causam  instabilidade  no sistema para diminuir temporariamente a sua segurança, passando então a executar ordens para roubar informações, invadir acessos bloqueados ou propagar vírus.

Outra coisa interessante é que eles podem explorar de vulnerabilidades zero-day. Zero o que, Diego?
Zero-day! No contexto de segurança da informação, trata-se de uma vulnerabilidade desconhecida por administradores de um sistema que pode ser explorada por hackers.
O termo zero-day (ou dia zero) é o dia em que o administrador de um sistema descobre essa vulnerabilidade e começa a tomar ações para mitigá-la.

exploit
= explorar
em nosso contexto, utilizar algo tirar vantagens 
(UFAL  –  2016) Exploit  é  um  software  malicioso  projetado  para  explorar  uma vulnerabilidade existente em um software de computador.
_______________________ Comentários: conforme vimos em aula, ele realmente é projetado para explorar vulnerabilidades de um software ou sistema computacional (Correto).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





49
128




3.8 – HIJACKER
INCIDÊNCIA EM PROVA: média 


O Browser Hijacker é um software malicioso que modifica o registro do sistema operacional, alterando o funcionamento do navegador, modificando sua página inicial, abrindo páginas automaticamente  ou  inserindo  botões  inadvertidamente.
Como  muitos  sites  patrocinam  o acesso a seu conteúdo, remunerando por cliques em links, o desenvolvedor do Hijacker costuma receber quantias financeiras sempre que estas páginas são abertas.



Em outras palavras, trata-se de uma praga virtual que assume o controle do navegador e muda a forma como seu conteúdo é exibido quando você está navegando na web. Quem nunca instalou sem querer o HAO123? Gente, esse maldito malware se instala, bagunça seu navegador inteiro e é terrível para desinstalar (eu odeio essa @#&*&# desse software). Eu já tive que formatar meu computador várias vezes por conta de hijackers.

hijack = sequestrar
hijacker = sequestrador 
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





50
128




(Prefeitura  de  Rurópolis/PA  –  2019) Os  programas  que  alteram  a  página  inicial  do navegador e também são capazes de redirecionar qualquer página visitada para outra, escolhida pelo criador da praga, são denominados de:

a) sniffers.
b) snappers.
c) hijackers.
d) screenloggers.
_______________________ Comentários: conforme vimos em aula, alterar página inicial do navegador e redirecionar páginas visitadas são ações maliciosas típicas de um Hijacker (Letra C).

(TRE/MA  -  2015) Alcebíades  queria  instalar  um  software  em  seu  computador rapidamente  para  modificar  umas  fotos.  Procurou  na internet  e  achou  um  software freeware.  Baixou  e  instalou,  sem  perceber  que  alguns  softwares  adicionais  foram instalados também. Como a prioridade era a rapidez e não a segurança, ele pagou o preço.  Sua  página  inicial  do  browser  foi  alterada, sua  página  de  procura  principal  e redirecionamentos de páginas. Qual destas pragas virtuais ele instalou?

a) Browser Hijacker.
b) Trojans.
c) Spyware.
d) Worms.
_______________________ Comentários: conforme vimos em aula, trata-se do Browser Hijacker (Letra A).

(TRT/MA – 2014) Após a instalação de um programa obtido na internet, o navegador Internet  Explorer  utilizado  por  Luis  apresenta  uma página  inicial  diferente  da configurada por ele, além de exibir pop-up indesejável. A partir dessas informações, pode-se concluir que o tipo de malware que atacou o computador do Luis é:

a) Hijacker.
b) Rootkit.
c) Worm.
d) Bootnet.
e) Keylogger.
_______________________ Comentários: apresentar página inicial diferente e exibir pop-up indesejável são ações maliciosas típicas de um Hijacker (Letra A).


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





51
128




4 – ATAQUES E GOLPES 4.1 – ENGENHARIA SOCIAL INCIDÊNCIA EM PROVA: média 


Galera, quando eu tinha uns 14 anos, eu já era fissurado com computadores e ficava encantado com todas as histórias de hackers que invadiam computadores, etc. À época, eu fiquei sabendo de um livro que contava a história do maior hacker de todos os tempos: Kevin Mitnick.
Eu comprei e fui
logo ler a história desse cara que hackeou computadores e sistemas de diversas empresas de tecnologia e provedores de internet na década de noventa.

Ele era tão ousado que – para mostrar como ele era competente – ele invadiu o computador pessoal de um dos maiores especialistas em segurança computacional do mundo: Tsutomu Shimomura.
Esse cara evidentemente não deixou barato e, no ano seguinte, conseguiu capturá-lo e prendê-lo com a ajuda do FBI. Ele ficou cinco anos preso e depois mais três anos sem poder chegar perto de um computador, celular ou internet.

Essa história é contada no filme chamado Take Down (Caçada Virtual)! Eu –  ávido  por  entender  como  esse  hacker  conseguiu  fazer  tudo  isso  – comprei  o  livro  pensando  que  descobriria  técnicas  mirabolantes  sobre como hackear computadores e sistemas. No entanto, em determinado momento do livro, Mitnick surpreende e diz:

Mitnick: Vocês sabem qual é a melhor técnica para descobrir uma senha?

Mitnick: Perguntando!

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





52
128





Galera, leiam o subtítulo do livro na página anterior. Ele diz:
“Ataques de Hackers: controlando o fator humano na Segurança da  Informação”.  É  claro  que  existem  técnicas  para  invadir sistemas, mas tantas outras envolvem mais o fator humano do que  o  fator  computacional! A  Engenharia  Social  é  uma técnica  por  meio  da  qual  uma  pessoa  procura  persuadir outra a executar determinadas ações por má-fé . Trata-se de
uma  técnica  utilizada  por  golpistas  para  tentar  explorar  a confiança, ingenuidade, ganância, vaidade ou boa-fé de outras pessoas,  a  fim  de  aplicar  golpes,  ludibriar  ou  obter informações sigilosas e importantes.

Ela é utilizada para obter informações importantes do usuário, através de sua ingenuidade ou da confiança. Quem está mal-intencionado geralmente utiliza telefone, e-mails ou salas de bate- papo para obter as informações que necessita. Por exemplo: algum desconhecido liga para a sua casa e se diz do suporte técnico do seu provedor de internet. Nessa ligação, ele te convence de que sua conexão está com problemas e pede sua senha para corrigir.

Duvide desse tipo de abordagem e contate o provedor caso algum técnico ligue para sua casa pedindo  dados  confidenciais  a  seu  respeito  (senhas,  números  de  cartões,  etc.)  avisando-o  do ocorrido.
Em suma: engenharia social é um conjunto de práticas utilizadas para obter acesso a informações importantes ou sigilosas em organizações/sistemas, através da persuasão e se aproveitando da ingenuidade ou confiança das pessoas . Um exemplo comum é o Phishing.

(BB – 2013) Analise o diálogo apresentado a seguir.

– Sr. José, bom dia: Aqui fala o suporte técnico do seu provedor de Internet. O senhor está feliz com o nosso atendimento?
– Sim, bastante.
– Sr. José, constatamos uma ligeira redução na velocidade da sua conexão e por isso gostaríamos de confirmar alguns dados para poder estar melhorando o serviço que lhe prestamos. É possível?
– Pois não!
– O seu endereço é rua do Bastião, 37?
– Sim.
– O seu e-mail é jose.arrose@empresa.com.br?
– Sim.
– Muito obrigado, Sr. José, seus dados foram confirmados e podemos continuar nossa entrevista. O seu histórico de cliente bom pagador gerou um benefício. A sua velocidade de conexão será aumentada sem qualquer acréscimo na sua mensalidade. Bons clientes, melhores serviços. O senhor aceita esse prêmio por bom relacionamento?
– Sim.
– Sr. José, podemos fazer isso imediatamente, nossos recursos de acesso remoto incorporaram novas funcionalidades que permitem que eu mesmo, com um simples comando no meu computador, modifique a configuração do seu modem e troque essa velocidade. O senhor autoriza essa manobra? São 10 M em lugar do seus 2 M atuais.
– Sim.
– O senhor, então, pode ditar sua senha de acesso, por favor?
– 4 5 2 8 4 7 9 3.
– Muito obrigado, Sr. José. Aguarde uns 30 min e verifique como estarão mais rápidos os seus acessos. O seu provedor agradece.

Esse diálogo caracteriza um ataque à segurança da informação conhecido por:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





53
128





a) port scanner
b) cavalo de troia
c) spyware
d) técnica de entrevista e) engenharia social _______________________ Comentários: conforme vimos em aula, trata-se claramente de engenharia social – inclusive como o exemplo de um provedor de internet que demos na teoria (Letra E).

(ANP  –  2016) Uma hacker  ameaçou divulgar na Web informações sigilosas de uma empresa após ter conseguido acesso a seus sistemas de informação. Para conseguir o acesso, ela telefonou para uma das secretárias da diretoria, passando-se por esposa de um dos diretores. Em seguida, ela disse à secretária que seu marido tinha sofrido um acidente e estava hospitalizado. Porém, antes de ficar inconsciente, o diretor lhe havia pedido que entrasse em contato com a empresa a fim de que uma de suas secretárias solicitasse a mudança do seu login e da sua senha, pois ele havia perdido sua agenda no acidente e temia que alguém pudesse invadir os sistemas da empresa, uma vez que esses dados, por descuido seu, estavam anotados na agenda perdida. Em seguida, a suposta esposa forneceu os novos login e senha à secretária.

Esse tipo de ataque para obtenção de informações é chamado de:

a) informações livres b) engenharia social c) varredura de vulnerabilidades d) dumpster diving
e) ataque físico
_______________________ Comentários: (a) Errado. Informações Livres é uma técnica de análise de informações que podem ser obtidas livremente na internet sem a necessidade de ações intrusivas; (b) Correto. Engenharia Social é uma técnica de obtenção de informações explorando vulnerabilidades humanas e sociais dos funcionários de uma organização; (c) Errado. Varredura de Vulnerabilidades é  uma  técnica  de envio  de  tipos  de  pacotes com  o  objetivo  de  obter informações  relevantes para um ataque  sobre  um computador ou uma rede; (d) Errado. Dumpster Diving é uma técnica de vasculhar o lixo (sim, lixo mesmo) de empresas e pessoas com o objetivo de encontrar algo de valor; (e) Errado. Ataque Físico é basicamente o roubo de equipamentos ou dispositivos de armazenamento realizado diretamente em uma organização (Letra B).

(CFO/DF – 2017) Não revelar informações confidenciais para outra pessoa, via telefone, sem confirmar sua legitimidade é uma das formas de evitar a engenharia social.
_______________________ Comentários: conforme vimos em aula, é uma forma clássica de engenharia social (Correto).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





54
128




4.2 – FORÇA BRUTA
INCIDÊNCIA EM PROVA: baixa 
Galera, deixa eu contar uma historinha para vocês! Era uma vez, um professor de informática que estava viajando para curtir  as  férias.  No  fim  da  viagem,  antes  de  ir  para  o aeroporto, ele fechou sua mala e – bastante inteligente que é – trancou seus documentos dentro. Na hora do check-in, ele lembrou que os documentos estavam dentro da mala, mas esqueceu a maldita da senha desse cadeado embutido que vem em algumas malas. O que ele teve que fazer? Testar todas as  possibilidades  de  combinação  desses  três  números  até descobrir  a  senha  correta  que  abrir  a  mala.
Esse  é  um
exemplo de força bruta e eu sou o professor mané (Isso aconteceu de verdade!).

Um Ataque de Força Bruta (Brute Force) consiste em adivinhar, por tentativa e erro, um nome de usuário e senha e, assim, executar processos e acessar sites, computadores e serviços em nome e com os mesmos privilégios deste usuário.
Qualquer computador, equipamento de rede ou serviço que seja acessível via Internet, com um nome de usuário e uma senha, pode ser alvo de um ataque de força bruta.

Mesmo que o atacante não consiga descobrir a sua senha, você pode ter problemas ao acessar a sua conta caso ela tenha sofrido um ataque de força bruta, pois muitos sistemas bloqueiam as contas quando há várias tentativas de acesso sem sucesso.
Apesar dos ataques de força bruta poderem ser realizados manualmente, em geral eles são realizados com o uso de ferramentas facilmente obtidas na Internet.
As tentativas de adivinhação são baseadas em:

 dicionários de diferentes idiomas e que podem ser facilmente obtidos na Internet;
 listas de palavras comumente usadas (Ex: personagens de filmes, nomes de times, etc);
 substituições óbvias de caracteres, como trocar "a" por "@" e "o" por "0"';
 sequências numéricas e de teclado, como "123456", "qwert" e "1qaz2wsx";
 informações pessoais (Ex: nome, sobrenome, datas e números de documentos).

Um ataque de força bruta, dependendo de como é realizado, pode resultar em um ataque de negação  de  serviço,  devido  à  sobrecarga  produzida  pela  grande  quantidade  de  tentativas realizadas em um pequeno período de tempo. Vamos ver exatamente o que é um ataque de negação de serviço no próximo tópico, mas é basicamente um ataque massivo que resulta na interrupção de um serviço. Bacana? Praticar...

(CODEBA – 2016) Um grupo de hackers chamado DarkSide tem como objetivo executar processos e acessar sites, computadores e serviços em nome e com os privilégios de um Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





55
128




usuário da rede. Para isso, os integrantes do DarkSide tentam adivinhar, por tentativa e erro, um nome de usuário da rede e sua respectiva senha.

De acordo com a Cartilha de Segurança para Internet do Centro de Estudos, Resposta e Tratamento  de  Incidentes  de  Segurança  no  Brasil  (cert.br),  a  técnica  utilizada  pelos integrantes da DarkSide é:

a) varredura em redes, ou scan.
b) interceptação de tráfego, ou sniffing.
c) ataque de força bruta, ou brute force.
d) falsificação de e-mail, ou e-mail spoofing.
e) negação de serviço, ou DoS (Denial of Service).
_______________________ Comentários: conforme vimos em aula, tentar adivinhar – por tentativa e erro – um nome de usuário da rede e sua respectiva senha é um exemplo típico de ataque de força bruta (Letra C).

(Câmara  de  Ponte  Nova/MG  –  2018) A  maioria  dos  computadores,  tanto  pessoais quanto  coorporativos,  hoje  em  dia,  trabalha  conectada  à  internet.  Por  isso,  eles  se tornam vulneráveis a vários tipos de ataques. Um desses ataques consiste em adivinhar, por tentativa e erro, um nome de usuário e senha e, assim, executar processos e acessar sites, computadores e serviços em nome e com os mesmos privilégios desse usuário.

O ataque que contém essa técnica, conforme o <cert.br>, é chamado de:

a) defacement.
b) sniffing.
c) força bruta.
d) e-mail spoofing.
_______________________ Comentários: conforme vimos em aula, adivinhar – por tentativa e erro – um nome de usuário e senha para executar processos e acessar sites, computadores e serviços em nome de um usuário é um ataque de força bruta (Letra C).

(UFBA – 2017) Um exemplo de ataque por força bruta (brute force) seria adivinhar, por tentativa e erro, um nome de usuário e senha, por exemplo, e, assim, executar processos e acessar sites, computadores e serviços em nome e com os mesmos privilégios desse usuário.
_______________________ Comentários: conforme vimos em aula, é mais uma vez a mesma descrição do mesmo ataque de força bruta (Correto).




Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





56
128




4.3 – DENIAL OF SERVICE (DOS) INCIDÊNCIA EM PROVA: média 


Negação de serviço (Denial of Service – DoS) é uma técnica pela qual um atacante busca retirar de operação um serviço, um computador ou uma rede conectada à Internet. Quando usada de forma coordenada e distribuída, ou seja, quando um conjunto de equipamentos é utilizado no ataque, recebe o nome de Ataque Distribuído de Negação de Serviço (Distributed Denial of Service – DDoS).

O objetivo destes ataques não é invadir nem coletar informações, mas – sim – exaurir recursos e  causar  indisponibilidades.  Nesse  caso,  todas  as  pessoas  que  dependem  do  serviço  são prejudicadas, visto que ficam impossibilitadas de acessar ou realizar as operações desejadas. Em geral, os alvos ficaram impedidos de oferecer serviços durante o ataque, mas voltam a operar normalmente ao final sem vazamento de informações ou comprometimento de sistemas.

Uma pessoa pode voluntariamente usar ferramentas e fazer com que seu computador seja utilizado em ataques.
No entanto, a grande maioria dos computadores participa dos ataques sem sequer ter conhecimento.
Por vezes, eu computador pode estar infectado (por exemplo, com worms) ou fazendo  parte  de  botnets. Ataques  de  negação  de  serviço  podem  ser  realizados de  diversas maneiras, tais como:

 Pelo  envio  de  grande  quantidade  de  requisições  para  um  serviço,  consumindo  os  recursos necessários ao seu funcionamento (processamento, número de conexões simultâneas, memória e espaço em disco, por exemplo) e impedindo que as requisições dos demais usuários sejam atendidas;

 Pela geração de grande tráfego de dados para uma rede, ocupando toda a banda disponível e tornando  indisponível  qualquer  acesso  a  computadores  ou  serviços  desta  rede;  ou  pela exploração  de  vulnerabilidades  existentes  em  programas,  que  podem  fazer  com  que  um determinado serviço fique inacessível.

(IF/MG  –  2016) A  respeito  da  segurança  de  redes,  o  ataque  conhecido  por  tornar inacessíveis  os  serviços  providos  pela  vítima  e  usuários  legítimos,  e  normalmente Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





57
128




nenhum  tipo  de  informação  é  roubado  ou  alterado  e  nem  é  feito  um  acesso  não autorizado à vítima é o:

a) Sniffer.
b) Wepattack.
c) Man-in-the-middle.
d) Endereçamento MAC.
e) DoS (Denial of Service).
_______________________ Comentários: conforme vimos em aula, ataque conhecido por tornar inacessíveis os serviços providos pela vítima e usuários legítimos é a descrição típica de um ataque de negação de serviço ou denial of service (Letra E).

(SEGEP/MA  –  2016) Um  cracker  passou  a  controlar  diversos  computadores remotamente após infectá-los com um tipo de programa malicioso chamado bot. Por meio desse programa, ele enviou instruções para desferir ataques maciços para tirar de operação serviços, computadores e redes conectadas à internet. Assim, conseguiu enviar grande quantidade de requisições para um serviço, tirando-o de operação. Conseguiu também  gerar  grande  tráfego  de  dados  para  uma  rede,  ocupando  toda  a  banda disponível, até conseguir sua queda. Esse tipo de ataque é conhecido como:

a) Ping of Death.
b) Sniffing.
c) Spoofing.
d) Defacement.
e) DoS.
_______________________ Comentários: conforme vimos em aula, desferir maciços ataques para tirar serviços, computadores ou redes de operação é um exemplo típico de um ataque de negação de serviço ou denial of service – DoS (Letra E).

(FUNAI – 2016) Há ataques que consistem em sobrecarregar um servidor com uma quantidade  excessiva  de solicitações  de  serviços.  Há  muitas  variantes  desse  tipo  de ataque.  Em  uma  delas  o  agressor  invade  muitos  computadores  e  instala  neles  um software  zumbi.  Quando  recebem  a  ordem  para  iniciar  o  ataque,  os  zumbis bombardeiam o servidor-alvo, tirando-o do ar. Esse tipo de ataque é conhecido como:

a) NGSV.
b) DDoS.
c) ServBlock.
d) Worm.
e) Cavalo de Tróia.
_______________________ Comentários:  conforme  vimos  em  aula,  bombardear  um  servidor  alvo  por  meio  de  um  ataque  de  zumbis  de  vários computadores, tirando-o do ar, é uma característica de um ataque distribuído de negação de serviço – DDoS (Letra B).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





58
128




4.4 – IP SPOOFING
INCIDÊNCIA EM PROVA: baixa 
O IP Spoofing (Falsificação/Mascaramento de IP) é uma técnica de invasão comumente empregada quando o mecanismo de autenticação de uma rede é baseado em endereços IP, isto é, quando a identificação de um usuário é realizada baseado em seu número de endereço IP.
Nesse caso, um
atacante pode clonar o IP de um usuário legítimo, mascarando-se e fazendo-se passar pelo usuário autorizado, podendo ganhar acessos não autorizados na rede.

COMUNICAÇÃO PADRÃO



TÉCNICA DE SPOOFING


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





59
128





(DPE/RJ  -  2014) Muitos  ataques  utilizam  uma  técnica  chamada  IP  spoofing,  tanto individualmente para  conseguir  acesso  a  outros  hosts  bem  como  em  conjunto  com outras ferramentas de ataque. Basicamente, IP spoofing gera pacotes?

a) para o endereço de broadcast da rede destino.
b) com o endereço IP de origem forjado.
c) para o endereço de destino de loopback.
d) com cabeçalhos inválidos ou corrompidos.
e) para endereços multicast.
_______________________ Comentários: conforme vimos em aula, gera pacotes com o Endereço IP de origem forjado (Letra B).

(EBSERH – 2015) Ataque  que objetiva mascarar pacotes IP utilizando endereços de remetentes falsos. Esse tipo de ataque é definido como:

a) Honeypot.
b) IP Flooding.
c) SYN Flooding.
d) IP Spoofing.
e) DNS Spoofing.
_______________________ Comentários: conforme vimos em aula, mascarar pacotes utilizando remetentes falsos é um típico ataque de IP Spoofing (Letra D).

(FUNASG  –  2015) Uma  rede  de  computadores  foi  atacada  com  um  vírus  que  cria endereços de rede falsos e permite que um usuário interno cause dano à rede sem ser descoberto com facilidade. Esse tipo de ameaça é denominado:

a) combolist.
b) bruteforce.
c) keylogger.
d) sniffer.
e) spoofing.
_______________________ Comentários: conforme vimos em aula, vírus que cria endereços de rede– também chamados de IP – falsos, permitindo que um usuário interno cause danos à rede sem ser descoberto com facilidade é basicamente um de IP Spoofing (Letra E).





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





60
128




4.5 – E-MAIL SPOOFING INCIDÊNCIA EM PROVA: ALTA 


E-Mail Spoofing (Falsificação/Mascaramento de E-Mail) é uma técnica que consiste em alterar campos  do  cabeçalho  de  um  e-mail,  de  forma  a  aparentar  que  ele  foi  enviado  de  uma determinada origem quando, na verdade, foi enviado de outra . Essa técnica é possível devido a características do protocolo SMTP (Simple Mail Transfer Protocol) que permitem que campos do cabeçalho sejam falsificados.

Ataques deste tipo são bastante usados para propagação de códigos maliciosos, envio de spam e em golpes de phishing. Atacantes utilizam-se de endereços de e-mail coletados de computadores infectados para enviar mensagens e tentar fazer com que os seus destinatários acreditem que elas partiram  de  pessoas  conhecidas.  Exemplos  de  e-mails  com  campos  falsificados  são  aqueles recebidos como sendo:

 de alguém conhecido, solicitando que você clique algum link ou execute algum arquivo em anexo;

 do seu banco, solicitando que você siga um link fornecido na própria mensagem e informe dados da sua conta bancária;

 do administrador do serviço de e-mail que você utiliza, solicitando informações pessoais e ameaçando bloquear a sua conta caso você não as envie.

Você também pode já ter observado situações em que o seu próprio endereço de e-mail foi indevidamente utilizado . Alguns indícios são, por exemplo, quando você recebe respostas de e- mails que você nunca enviou; quando recebe e-mails aparentemente enviados por você mesmo, Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





61
128




sem que você tenha feito isto; ou quando recebe mensagens de devolução de e-mails que você nunca enviou, reportando erros como usuário desconhecido e caixa de entrada lotada.

(Câmara de Boa Vista - 2014) A respeito de ataques na internet, pode-se afirmar que e- mail spoofing:

a)  é  o  termo  usado  para  se  referir  aos  e-mails  não solicitados,  que  geralmente  são enviados para um grande número de pessoas.

b) é uma técnica que consiste em espionar os dados de emails trafegados em redes de computadores, por meio do uso de programas específicos chamados de sniffers.

c) é uma técnica pela qual um atacante utiliza um computador para tirar de operação um serviço, um computador ou uma rede conectada à internet.

d) é uma técnica que consiste em alterar campos do cabeçalho de um e-mail, de forma a aparentar  que  ele  foi  enviado  de  uma  determinada  origem  quando,  na  verdade,  foi enviado de outra.
_______________________ Comentários: (a) Errado, o item trata de spam; (b) Errado, o item trata de sniffing; (c) Errado, o item trata de negação de serviço;
(d) Correto, essa é a definição correta de e-mail spoofing (Letra D).

(Câmara de Boa Vista - 2014) Qual é o nome da técnica que consiste em alterar campos do  cabeçalho  de  um  e-mail,  de  forma  a  aparentar  que  ele  foi  enviado  de  uma determinada origem quando na verdade, foi enviado de outra?

a) Spoofing
b) Sniffing
c) Brute Force
d) Defacement
_______________________ Comentários: conforme vimos em aula, a técnica que altera cabeçalhos de um e-mail para fasificá-lo é o Spoofing – mais precisamente, E-mail Spoofing (Letra A).










Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





62
128




4.6 – PHISHING SCAM
INCIDÊNCIA EM PROVA: Altíssima 


O Phishing Scam é uma fraude em que o golpista tenta enganar um usuário para obtenção de dados  pessoais  e  financeiros que  permitam  a  aplicação  de  um  golpe,  combinando  técnicas computacionais e de engenharia social. Um exemplo de phishing é um e-mail que possa induzir o usuário a clicar em um link falso levando-o para uma página clonada ou para um arquivo malicioso.
O Phishing ocorre por meio do envio de mensagens eletrônicas que:

 Tentam se passar pela comunicação oficial de uma instituição conhecida, como um banco, uma empresa ou um site popular; ou que procuram atrair a atenção do usuário, seja por curiosidade, por caridade ou pela possibilidade de obter alguma vantagem financeira;

 Informam  que  a  não  execução  dos  procedimentos  descritos  pode  acarretar  sérias consequências, como a inscrição em serviços de proteção de crédito e o cancelamento de um cadastro, de uma conta bancária ou de um cartão de crédito;

 Tentam induzir o usuário a fornecer dados pessoais e financeiros, por meio do acesso a páginas falsas, que tentam se passar pela página oficial da instituição; da instalação de malwares; e do preenchimento de formulários contidos na mensagem ou em páginas Web.

Para  atrair  a  atenção  do  usuário,  as  mensagens  apresentam  diferentes  tópicos  e  temas, normalmente  explorando  campanhas  de  publicidade,  serviços,  a  imagem  de  pessoas  e assuntos em destaque no momento . Galera, todos vocês já devem ter sido alvos de algum tipo de phishing alguma vez na vida – eu mesmo vou mostrar alguns casos que aconteceram comigo. Por enquanto, vamos ver alguns exemplos de situações envolvendo esse golpe:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





63
128





 Páginas falsas de comércio eletrônico ou Internet Banking: você recebe um e-mail em nome de um site de comércio eletrônico ou de uma instituição financeira, que tenta induzi-lo a clicar em um link. Ao fazer isto, você é direcionado para uma página falsa, semelhante ao site que você realmente deseja acessar, onde são solicitados dados pessoais e financeiros.

 Páginas  falsas  de  redes  sociais  ou  de  companhias  aéreas:  você  recebe  uma  mensagem contendo um link para o site da rede social ou da companhia aérea que você utiliza. Ao clicar, você é direcionado para uma página falsa em que são solicitados o seu nome de usuário e a sua senha que, ao serem fornecidos, serão enviados aos golpistas.

 Mensagens contendo formulários: você recebe uma mensagem contendo um formulário com campos  para  a  digitação  de  dados  pessoais  e  financeiros.  A  mensagem  solicita  que  você preencha  o  formulário  e  apresenta  um  botão  para  confirmar  o  envio  das  informações.  Ao preencher os campos e confirmar o envio, seus dados são transmitidos para os golpistas.

 Mensagens contendo links para códigos maliciosos: você recebe um e-mail que tenta induzi- lo a clicar em um link, para baixar e abrir/executar um arquivo. Ao clicar, é apresentada uma mensagem de erro ou uma janela pedindo que você salve o arquivo. Após salvo, quando você o abrir ou o executar, será instalado um código malicioso em seu computador.

 Solicitação de recadastramento: você recebe uma mensagem, supostamente enviada pelo grupo  de  suporte  da  instituição  de  ensino que  frequenta  ou  da  empresa  em  que  trabalha, informando  que  o  serviço  de  e-mail  está  passando  por  manutenção  e  que  é  necessário  o recadastramento. Para isto, é preciso que você forneça dados como nome de usuário e senha.

Professor, estou assustado. Como eu faço para me prevenir de cair em golpes semelhantes a esses apresentados anteriormente? Vejamos as formas de prevenção:

PREVENÇÃO
Fique  atento  a  mensagens,  recebidas  em  nome  de  alguma  instituição,  que  tentem  induzi-lo  a  fornecer informações, instalar/executar programas ou clicar em links.

Questione-se porquê instituições com as quais você não tem contato estão lhe enviando mensagens, como se houvesse  alguma  relação  prévia  entre  vocês  (Ex:  se você  não  tem  conta  em  um  banco,  não  há  porque recadastrar dados ou atualizar módulos de segurança).
Fique atento a mensagens que apelem demasiadamente pela sua atenção e que, de alguma forma, o ameacem caso você não execute os procedimentos descritos.

Não considere que uma mensagem é confiável com base na confiança que você deposita em seu remetente, pois ela pode ter sido enviada de contas invadidas, de perfis falsos ou pode ter sido forjada.

Seja cuidadoso ao acessar links. Procure digitar o endereço diretamente no navegador web.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





64
128




Verifique o link apresentado na mensagem. Golpistas costumam usar técnicas para ofuscar o link real para o phishing. Ao posicionar o mouse sobre o link, muitas vezes é possível ver o endereço real da página falsa ou código malicioso.
Utilize mecanismos de segurança, como programas antimalware, firewall pessoal e filtros antiphishing.


Verifique se a página utiliza conexão segura. Sites de comércio eletrônico ou Internet Banking confiáveis sempre utilizam conexões seguras quando dados sensíveis são solicitados.

Verifique  as  informações  mostradas  no  certificado. Caso  a  página  falsa  utilize  conexão  segura,  um  novo certificado será apresentado e, possivelmente, o endereço mostrado no navegador web será diferente do endereço correspondente ao site verdadeiro.
Acesse a página da instituição que supostamente enviou a mensagem e procure por informações (você vai observar que não faz parte da política da maioria das empresas o envio de mensagens, de forma indiscriminada, para os seus usuários).

Galera, eu recebi um e-mail um dia desses do Bradesco! Eu achei estranho e fui ver o que era porque eu realmente tenho conta no Bradesco. Vejam só a imagem abaixo:



Notem que o título já é estranho, porque “você” está escrito com erro! Outra coisa importante de observar é o endereço do remetente: banco.bradesco@netmail2.bradesco.com.br. Galera,  isso parece ser um e-mail real do Bradesco? Não, está esquisito! O banco não envia e-mails aos clientes sem autorização prévia. Eu entrei no site do banco e procurei pela seção de segurança. Logo, ficou claro que se tratava de uma tentativa de phishing...

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





65
128






(Prefeitura de Jardim de Piranhas/RN – 2019) O nome da técnica de fraude online que é utilizada por criminosos, os quais utilizam armadilhas virtuais como e-mails falsos, websites  ou,  até  mesmo,  mensagens,  para  roubar  senhas  de  banco  e  demais informações pessoais, usando-as de maneira fraudulenta, é o:

a) Worm.
b) Keylogger.
c) Ransomware.
d) Phishing.
_______________________ Comentários: conforme vimos em aula, fraude online que utiliza armadilhas virtuais como e-mails falsos, websites ou até mesmo mensagens para roubar senhas de banco e informações pessoais é típico de Phishing (Letra D).

(UFRN  –  2019) Maria,  do  setor  de  Contabilidade  da  Security10,  relatou  que recentemente recebeu uma mensagem eletrônica sobre um seguro de vida que ela não solicitou, mas a mensagem provém do banco no qual ela tem conta. O conteúdo da mensagem  trazia  um  link  para  o  contrato do  seguro  com  as  informações  gerais  da apólice e um outro link para a geração do boleto a ser pago. Ao clicar em qualquer um dos links, era exibida uma página do banco requisitando os dados da conta, incluindo a senha para operações online. Tudo parecia legítimo, mas ao tentar prosseguir, sempre dava uma mensagem para tentar novamente. Nesse caso, Maria foi vítima de um ataque de:

a) Phishing.
b) SPAM.
c) Malware.
d) Adware.
_______________________ Comentários: conforme vimos em aula, se ela recebeu um e-mail não solicitado com um link para um contrato com um boleto para pagamento e exigindo dados da conta e senha, trata-se claramente de um phishing (Letra A).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





66
128




(SEFAZ/BA – 2019) Um Auditor recebeu uma mensagem de e-mail, aparentemente de seu banco, com um link para verificar a existência de uma dívida de cartão de crédito não paga. Preocupado com a situação, clicou no link e forneceu os dados de seu cartão de crédito para pagar a suposta conta. Dias depois percebeu na fatura do seu cartão que foram feitas diversas compras online em sites de comércio eletrônico na Internet. A situação descrita permite concluir que esse Auditor foi vítima de:

a) rot.
b) backdoor.
c) worm.
d) phishing.
e) ransomware.
_______________________ Comentários: conforme vimos em aula, link solicitando fornecimento de dados de cartão é típico de phishing (Letra D).

(Prefeitura de Valinhos/SP – 2019) Frequentemente, os usuários de Correio Eletrônico recebem mensagens contendo frases como “atualize seus dados bancários” ou, então, “parabéns, você é o novo milionário”, cujo objetivo é capturar informações como senhas de banco e demais informações pessoais para utilizá-las de maneira fraudulenta. Esse tipo de crime, que cresce em ritmo acelerado, é chamado:

a) Accounting.
b) Backdoor.
c) Download.
d) Phishing.
e) Redirecting.
_______________________ Comentários: conforme vimos em aula, golpe para capturar dados pessoais ou financeiros é o tal do phishing (Letra D).

(FPMA/PR – 2019) Você recebe um e-mail, supostamente enviado pelo grupo de suporte da empresa em que trabalha, informando que sua caixa postal está cheia e que será necessário o recadastramento. Para isso, é preciso que você atualize seus dados pessoais clicando no link fornecido. Esse tipo de golpe é conhecido como:

a) Ransomware.
b) Rootkit.
c) Phishing.
d) Cavalo de troia.
e) NCE.
_______________________ Comentários: conforme vimos em aula, e-mail solicitando recadastramento e fornecimento de dados pessoais clicando em um link fornecido pelo e-mail é típico de phishing (Letra C).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





67
128




4.7 – PHARMING
INCIDÊNCIA EM PROVA: ALTA 


Para entender a mecânica de um ataque de Pharming e como eles são realizados, precisamos explorar como os servidores DNS (Domain Name Service) funcionam. A tarefa do DNS é converter nomes de domínio em endereços IP, o que representa a localização real do site, permitindo que o navegador da Internet se conecte ao servidor em que o site está hospedado.
O método mais
comum de executar esse ataque é por meio do envenenamento de cache.


Quando você digita o endereço de um site, seu navegador cria um cache (memória rápida) de DNS para que você não precise retornar ao servidor toda vez que quiser revisitar um site. O pharming é um tipo de phishing que "envenena" a tabela de cache do Servidor DNS, corrompendo o  servidor  por  meio  da  alteração  de  IPs  e  redirecionando  o  tráfego  da  Internet  para  sites fraudulentos para capturar informações e permitir a ação de golpistas.

Neste caso, quando você tenta acessar um site legítimo, o seu navegador é redirecionado para uma página falsa de forma transparente, isto é, sem que você esteja ciente. Logo, você digita no navegador www.bb.com.br, por exemplo. No entanto, você é redirecionado para uma página cujo  endereço  é www.bb.net.br  e  sequer  percebe.  Galera,  existem  tipos  diferentes  de redirecionamento. Vejamos...

TIPOS DE REDIRECIONAMENTO Por meio do comprometimento do servidor de DNS do provedor que você utiliza;

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





68
128




Pela  ação  de  códigos  maliciosos  projetados  para  alterar  o  comportamento  do  serviço  de  DNS  do  seu computador;
Pela ação direta de um invasor, que venha a ter acesso às configurações do serviço de DNS do seu computador ou modem de banda larga.

prevenção
Desconfie se, ao digitar uma URL, for redirecionado para outro site, o qual tenta realizar alguma ação suspeita, como abrir um arquivo ou tentar instalar um programa;

Desconfie imediatamente caso o site de comércio eletrônico ou Internet Banking que você está acessando não utilize conexão segura. Sites confiáveis de comércio eletrônico e Internet Banking sempre usam conexões seguras quando dados pessoais e financeiros são solicitados;
Observe se o certificado apresentado corresponde ao do site verdadeiro.



Em suma: pharming é um ataque que possui como estratégia corromper o DNS e direcionar o endereço de um sítio para um servidor diferente do original . É um tipo específico de phishing que envolve o redirecionamento da navegação do usuário para sites falsos, por meio de alterações no serviço de DNS. Nesse caso, quando o usuário tenta acessar um site legítimo, o seu navegador web é redirecionado, de forma transparente, para uma página falsa.

(HCPA – 2016) Assinale a alternativa que apresenta um método utilizado como base para o ataque de segurança chamado de pharming:

a) Envenenamento de cache de DNS.
b) Negação de serviço distribuída.
c) Código malicioso escondido em arquivos.
d) Troca de endereços nos cabeçalhos IP das mensagens.
e) Troca de portas nos cabeçalhos TCP das mensagens.
_______________________ Comentários: conforme vimos em aula, pharming envenena o cache (memória) do serviço de DNS – nenhum dos outros itens faz qualquer sentido (Letra A).

(TJ/AC – 2012) Pharming é um ataque que possui como estratégia corromper o DNS e direcionar o endereço de um sítio para um servidor diferente do original.
_______________________ Comentários: conforme vimos em aula, esse ataque realmente busca corromper o DNS e redirecionar o usuário para uma página de um servidor diferente do original (Correto).

(TRF/1 – 2011) O golpe de Pharming é um ataque que consiste em:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





69
128




a) corromper o DNS, fazendo com que a URL de um site passe a apontar para um servidor diferente do original.

b) alterar as tabelas de roteamento para que o roteador desvie os pacotes para um falso servidor.

c)  impedir  que  o  servidor  DNS  converta  o  endereço  em  um  número  IP  e  assim congestionar a rede.

d) instalar um programa cliente no servidor de destino para capturar senhas e endereços de sites.

e) travar um servidor de páginas através do envio de pacotes IP inválidos.
_______________________ Comentários: (a) Correto, ele corrompe o DNS permitindo um redirecionamento de endereços; (b) Errado, ele não altera tabelas de roteamento de roteadores, ele altera a tabela de cache do DNS; (c) Errado, ele não impede a conversão, ele só altera os endereços; (d) Errado, ele não instala nenhum programa; (e) Errado, ele não trava servidores de páginas (Letra A).

(FINEP - 2011) O ataque a uma rede de computadores que corrompe o DNS (Domain Name  System),  fazendo  com  que  a  URL  (Uniform  Resource  Locator)  de  um  site redirecione o cliente para um servidor diferente do original, é denominado:

a) backdoor
b) pharming
c) sharing
d) spam
e) worm
_______________________ Comentários: conforme vimos em aula, corromper o DNS alterando redirecionamentos é típico de Pharming (Letra B).














Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





70
128




4.8 – HOAX
INCIDÊNCIA EM PROVA: média 


O Hoax (Boato) é uma mensagem que possui conteúdo alarmante ou falso e que, geralmente, tem como remetente, ou aponta como autora, alguma instituição, empresa importante ou órgão  governamental .  Por  meio  de  uma  leitura  minuciosa  de  seu  conteúdo,  normalmente,  é possível identificar informações sem sentido e tentativas de golpes, como correntes e pirâmides.

CONTEÚDO DE HOAX
Conter códigos maliciosos, espalhar desinformação pela internet ou ocupar – desnecessariamente – espaço nas caixas de e-mails dos usuários.
Comprometer a credibilidade e a reputação de pessoas ou entidades referenciadas na mensagem.

Comprometer a credibilidade e a reputação da pessoa que o repassa, pois, ao fazer isto, esta pessoa estará supostamente endossando ou concordando com o conteúdo da mensagem.
Aumentar excessivamente a carga de servidores de e-mail e o consumo de banda de rede, necessários para a transmissão e o processamento das mensagens.
Indicar, no conteúdo da mensagem, ações a serem realizadas e que, se forem efetivadas, podem resultar em sérios danos.

Em geral, boatos se propagam pela boa vontade e solidariedade de quem os recebe, pois há uma grande tendência das pessoas em confiar no remetente, não verificar a procedência e não conferir a veracidade do conteúdo da mensagem . Para que você possa evitar a distribuição de Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





71
128




boatos  é  muito  importante  conferir  a  procedência  dos  e-mails  e,  mesmo  que  tenham  como remetente alguém conhecido, é preciso certificar-se de que a mensagem não é um boato.

(CRBM/6  –  2018) A principal característica do vírus Hoax é que ele é utilizado para “pescar” senhas e(ou) dados financeiros dos usuários, como, por exemplo, do cartão de crédito.
_______________________ Comentários: conforme vimos em aula, a questão trata de phishing e, não, hoax (Errado).

(IF/BA  -  2014) A  Internet  propicia  muitas  facilidades  e  tornou-se indispensável  na atualidade.  Ela  expõe,  porém,  seus  usuários  a  muitas  ameaças.  Uma  das  principais ameaças dos usuários da Internet são os vírus, que existem em diversas categorias. A categoria de vírus que visa a difundir histórias enganosas ou boatos é o:

a) Backdoor.
b) Cavalo de Troia.
c) Hoax.
d) Phishing.
e) Spyware.
_______________________ Comentários: conforme vimos em aula, a questão trata de hoax – eles podem ser espalhados por meio de vírus (Letra C).

(TRT/24  –  2011) O  usuário  do  computador  recebe  uma  mensagem  não  solicitada, geralmente  de conteúdo  alarmista,  a  fim  de  assustá-lo  e  convencê-lo  a  continuar  a corrente interminável de e-mails para gerar congestionamento na rede. Trata-se de um ataque denominado:

a) Hoax.
b) Worms.
c) Trojans.
d) Spam.
e) Backdoors.
_______________________ Comentários: conforme vimos em aula, mensagem não solicitada no e-mail com conteúdo alarmista a fim de assustar ou convencer sobre algo é típico de hoax (Letra A).







Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





72
128




4.9 – MAN IN THE MIDDLE INCIDÊNCIA EM PROVA: baixa 


O Man in the Middle é um ataque em que os dados trocados entre duas partes (Ex: você e o seu banco)  são  de  alguma  forma  interceptados,  registrados  e  possivelmente  alterados  pelo atacante sem que as vítimas percebam.
Durante o ataque, a comunicação é interceptada pelo atacante e retransmitida. O atacante pode decidir retransmitir entre os legítimos participantes os dados inalterados, com alterações ou bloquear partes da informação.

(BANPARÁ– 2018 – Item II) O ataque do homem-do-meio refere-se à forma de ataque em  que  uma  comunicação  entre  duas  pessoas  é  interceptada  por  uma  terceira.  O atacante simplesmente recebe e, opcionalmente, repassa as informações do transmissor para o receptor, sem que ambos percebam que a comunicação não está sendo, de fato, direta.
_______________________ Comentários: conforme vimos em aula, essa é a definição impecável do ataque Man in The Middle (Correto).

(TRF4 – 2019) Em redes de computadores, é o tipo de ataque em que o espião intercepta a comunicação entre dois usuários, de forma que o usuário A comunique-se com ele mesmo pensando ser o usuário B, e o usuário B também o faz, pensando ser o usuário A.
Trata-se de:

a) SYN Flooding.
b) Pharming.
c) Man-in-The-Middle.
d) DoS.
e) Spoofing.
_______________________ Comentários: conforme vimos em aula, trata-se do Man-in-the-Middle (Letra C).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





73
128




4.10 – DEFACEMENT
INCIDÊNCIA EM PROVA: baixíssima 


Desfiguração de página (Defacement ou Pichação) é uma técnica que consiste em alterar o conteúdo da página web . Para ganhar mais visibilidade, chamar mais atenção e atingir maior número de visitantes, geralmente os atacantes alteram a página principal do site, porém páginas internas também podem ser alteradas. As principais formas que um atacante, neste caso também chamado de Defacer, pode utilizar para desfigurar uma página web são:

 explorar  vulnerabilidades  da  linguagem  de  programação  ou  dos  pacotes  utilizados  no desenvolvimento da aplicação Web;

 invadir o servidor onde a aplicação Web está hospedada e alterar diretamente os arquivos que compõem o site;

 explorar erros da aplicação Web ou vulnerabilidades do servidor de aplicação web; ou furtar senhas de acesso à interface Web usada para administração remota.

(TRE/RJ – 2012) É possível executar um ataque de desfiguração (defacement) — que consiste  em  alterar  o  conteúdo  da  página  web  de  um sítio  —  aproveitando-se  da vulnerabilidade  da  linguagem  de  programação  ou  dos pacotes  utilizados  no desenvolvimento de aplicação web.
_______________________ Comentários: conforme vimos em aula, o defacement realmente consiste em alterar o conteúdo da página web de um sítio (Correto).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





74
128




RESUMO

DEFINIÇÃO de malware Códigos maliciosos (Malwares, do inglês Malicious Softwares) são programas especificamente desenvolvidos para executar ações danosas e atividades maliciosas em um computador.

FORMAS comuns DE INFECÇÃO DE MALWARES Pela  exploração  de  vulnerabilidades  existentes  nos programas  instalados  ou  pela  auto-execução  de  mídias removíveis infectadas, como pen-drives;
Pelo acesso a páginas maliciosas, utilizando navegadores vulneráveis ou pela ação direta de atacantes que, após invadirem o computador, incluem arquivos contendo códigos maliciosos;
Pela execução de arquivos previamente infectados, obtidos em anexos de mensagens eletrônicas, via mídias removíveis, em páginas web ou de outros computadores.



DEFINIÇÃO de vírus
Programa ou parte de um programa, normalmente malicioso, que se propaga infectando, inserindo cópias de si mesmo, anexando-se ou hospedando-se em arquivos ou programas existentes na máquina.

TIPOs de vírus DESCRIÇÃO VÍRUS DE SCRIPT
Escrito em linguagem de script, como VBScript e JavaScript, e recebido ao acessar uma página web ou por e-mail, como um arquivo anexo ou como parte do próprio e-mail escrito em formato HTML.

VÍRUS DE MACRO
Tipo específico de vírus de script normalmente recebido ao acessar páginas web ou por e-mail e que tenta infectar arquivos  manipulados  por  aplicativos  que  utilizam  essas  linguagens  mencionadas  anteriormente  como  os arquivos que compõe o Microsoft Office.
VÍRUS DE BOOT
Também conhecido como Vírus de Setor de Carga ou Vírus de Setor de Inicialização, ele é ativado quando o computador é ligado e é carregado na memória antes do sistema operacional.

VÍRUS DE ARQUIVO
Também conhecido como Vírus de Programa ou Parasitário, trata-se do vírus mais tradicional e comum. Ele infecta e causa danos ao se conectarem a arquivos executáveis (.exe, .com, .dll, etc), sobrescrevendo o código original e causando danos quase sempre irreparáveis.
VÍRUS POLIMÓRFICO
Também conhecido como Vírus Mutante, é capaz de assumir múltiplas formas a cada infecção com o intuito de burlar o software de antivírus.

VÍRUS METAMÓRFICO
Trata-se de um vírus que se transforma a cada infecção, mas que – diferentemente do polimórfico – se reescreve completamente a cada infecção, podendo mudar seu tamanho e comportamento, aumentando a dificuldade de detecção.
VÍRUS STEALTH
Projetados  explicitamente  para  não  serem  detectados  pelo antivírus  e  têm  a capacidade  de  se remover  da memória temporariamente para evitar que o antivírus o detecte.

VÍRUS TIMEBOMB
Conhecido como Vírus Bomba Relógio, trata-se de um vírus que – após infectar a máquina – permanece latente (oculto), apenas  se  replicando,  e  seu  código malicioso  é  programado  para  ser  ativado  em  um  determinado momento específico, executando sua carga útil.
PRINCIPAIS CATEGORIAS DE MALWARES VÍRUSWORMBOTTROJANSPYWAREBACKDOORROOTKIT Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





75
128




TIPOs de malwares DESCRIÇÃO WORM
Worm (ou Verme) é um programa capaz de se replicar automaticamente, enviando cópias de si mesmo. Diferente dos vírus, ele não se propaga por meio da inclusão de cópias de si mesmo em outros programas ou arquivos através da rede, mas – sim – pela exploração automática de vulnerabilidades existentes em programas instalados em computadores ou pela execução direta de suas cópias.
BOT
Bot é um programa que dispõe de mecanismos de comunicação com o invasor que permitem que ele seja controlado remotamente. Possui processo de infecção e propagação similar ao do Worm, ou seja, é capaz de se propagar automaticamente, explorando vulnerabilidades existentes em programas instalados em computadores.
BOTNET
Rede formada por centenas ou milhares de computadores zumbis e que permitem potencializar as ações danosas executadas pelos bots.


CAVALO DE TROIA
O Trojan é um programa que age utilizando o princípio do Cavalo de Troia, em um arquivo é enviado se fazendo passar  por  um  aplicativo  útil,  como  um  “presente  de  grego”,  mas  que  na  verdade  possui  funcionalidades maliciosas escondidas. Muitas vezes, o trojan abre portas de comunicação para que através da Internet a máquina possa ser invadida ou monitorada.
RANSOMWARE
Trata-se de um tipo de código malicioso que torna inacessíveis os dados armazenados em um equipamento, geralmente utilizando criptografia, e que exige pagamento de um resgate (Ransom, em inglês) para restabelecer o acesso ao usuário – trata-se de uma espécie de extorsão virtual.

SPYWARE
Software espião, capaz de violar a privacidade das informações de usuários, coletando dados da máquina ou da rede e disponibilizando-as a terceiros. Pode ser usado tanto de forma legítima quanto maliciosa, dependendo de como é instalado, das ações realizadas, do tipo de informação monitorada e do uso que é feito por quem recebe as informações coletadas.
KEYLOGGER
Trata-se de um spyware capaz de capturar e armazenar as teclas digitadas pelo usuário no teclado do computador e enviá-las a um invasor.


SCREENLOGGER
Trata-se de um spyware – similar ao keylogger – capaz de armazenar a posição do cursor e a tela apresentada no monitor nos momentos em que o mouse é clicado, ou a região que circunda a posição onde o mouse é clicado.

ADWARE
Trata-se de um spyware projetado especificamente para apresentar propagandas. Pode ser usado para fins legítimos, quando incorporado a programas e serviços, como forma de patrocínio ou retorno financeiro para quem desenvolve programas livres ou presta serviços gratuitos. Também pode ser usado para fins maliciosos quando as propagandas são direcionadas.
SNIFFER
Um Sniffer é programa que age monitorando o tráfego na rede, através da captura de pacotes de dados, em busca de informações sensíveis como o endereço dos sites acessados, senhas de acesso, e-mails, etc.


BACKDOOR
Um programa que permite o retorno de um invasor a um computador comprometido, por meio da inclusão de serviços criados ou modificados para este fim.


ROOTKIT
Conjunto de programas e técnicas que permite esconder e assegurar a presença de um invasor ou de outro código malicioso em um computador comprometido.


BOMBAS LÓGICAS
Trata-se de um software malicioso normalmente instalado por um usuário autorizado, como um administrador da  rede,  que  o  mantém  no  sistema  deixando-o  programado  para  causar  danos  (como  excluir  arquivos importantes) em um determinado evento, como por exemplo o caso de ficar mais de 30 dias sem efetuar login.
EXPLOITS
Trata-se de uma ferramenta criada por hackers para permitir explorar vulnerabilidades conhecidas de sistemas e assim permitir que iniciantes (Script Kiddies) possam praticar ações de invasões sem conhecimentos avançados.

HIJACKER
O Hijacker (sequestro, em inglês) é um software malicioso que modifica o registro do sistema operacional, alterando o funcionamento do navegador, modificando sua página inicial, abrindo páginas automaticamente, inserindo botões inadvertidamente.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





76
128




TIPOs de ataques DESCRIÇÃO ENGENHARIA SOCIAL
Trata-se de uma técnica muito utilizada por golpistas para tentar explorar a ganância, a vaidade e a boa-fé ou abusar da ingenuidade e da confiança de outras pessoas, a fim de aplicar golpes, ludibriar ou obter informações sigilosas e importantes. O termo é utilizado para os métodos de obtenção de informações importantes do usuário, através de sua ingenuidade ou da confiança.
FORÇA BRUTA
Consiste em adivinhar, por tentativa e erro, um nome de usuário e senha e, assim, executar processos e acessar sites, computadores e serviços em nome e com os mesmos privilégios deste usuário. Qualquer computador, equipamento de rede ou serviço que seja acessível via Internet, com um nome de usuário e uma senha, pode ser alvo de um ataque de força bruta.
NEGAÇÃO DE SERVIÇO
Negação de serviço (Denial of Service – DoS) é uma técnica pela qual um atacante busca retirar de operação um serviço, um computador ou uma rede conectada à Internet. Quando usada de forma coordenada e distribuída, ou seja, quando um conjunto de equipamentos é utilizado no ataque, recebe o nome de Ataque Distribuído de Negação de Serviço (Distributed Denial of Service – DDoS).
IP SPOOFING
O IP Spoofing (Falsificação/Mascaramento de IP) é uma técnica de invasão comumente empregada quando o mecanismo de autenticação de uma rede é baseado em endereços IP, isto é, quando a identificação de um usuário é realizada baseado em seu número de endereço IP.

E-MAIL SPOOFING
Técnica que consiste em alterar campos do cabeçalho de um e-mail, de forma a aparentar que ele foi enviado de uma  determinada  origem  quando,  na  verdade,  foi  enviado  de  outra.  Essa  técnica  é  possível  devido  a características do protocolo SMTP (Simple Mail Transfer Protocol) que permitem que campos do cabeçalho sejam falsificados.
PHISHING SCAM
Fraude em que o golpista tenta enganar um usuário para obtenção de dados pessoais e financeiros que permitam a aplicação de um golpe, combinando técnicas computacionais e de engenharia social. Um exemplo de phishing é um e-mail que possa induzir o usuário a clicar em um link falso levando-o para uma página clonada ou um arquivo malicioso.
PHARMING
Ataque que possui como estratégia corromper o DNS e direcionar o endereço de um sítio para um servidor diferente do original. É um tipo específico de phishing que envolve o redirecionamento da navegação do usuário para sites falsos, por meio de alterações no serviço de DNS. Nesse caso, quando o usuário tenta acessar um site legítimo, o navegador web é redirecionado, de forma transparente, para uma página falsa.
HOAX
Trata-se de uma mensagem que possui conteúdo alarmante ou falso e que, geralmente, tem como remetente, ou aponta como autora, alguma instituição, empresa importante ou órgão governamental.


MAN IN THE MIDDLE
Trata-se  de  um  ataque  em  que  os  dados  trocados  entre  duas  partes  são  de  alguma  forma  interceptados, registrados  e  possivelmente  alterados  pelo  atacante  sem  que  as  vítimas  percebam.  Durante  o  ataque,  a comunicação  é  interceptada  pelo  atacante  e  retransmitida.  O  atacante  pode  decidir  retransmitir  entre  os legítimos participantes os dados inalterados, com alterações ou bloquear partes da informação.
DEFACEMENT
Trata-se de uma técnica que consiste em alterar o conteúdo da página web. Para ganhar mais visibilidade, chamar mais atenção e atingir maior número de visitantes, geralmente os atacantes alteram a página principal do site, porém páginas internas também podem ser alteradas.













Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





77
128




RESUMO DE Códigos maliciosos 
VÍRUS

WORM

BOT

TROJAN

SPYWARE

BACKDOOR

ROOTKIT

FORMA DE OBTENÇÃO
Recebido automaticamente pela rede X X
Recebido por e-mail
X X X X X
Baixado de sites na Internet X X X X X
Compartilhamento de arquivos X X X X X
Uso de mídias removíveis infectadas X X X X X
Redes sociais
X X X X X
Mensagens instantâneas X X X X X
Inserido por um invasor X X X X X X
Ação de outro código malicioso X X X X X X
FORMA DE INSTALAÇÃO
Execução de um arquivo infectado X
Execução explícita do código malicioso X X X X
Via execução de outro código malicioso X X
Exploração de vulnerabilidades X X   X X
FORMA DE PROPAGAÇÃO
Insere cópia de si próprio em arquivos X
Envia cópia de si próprio automaticamente pela rede X X
Envia cópia de si próprio automaticamente por email X X
Não se propaga
X X X X
AÇÕES MALICIOSAS MAIS COMUNS Altera e/ou remove arquivos X   X   X
Consome grande quantidade de recursos X X
Furta informações sensíveis X X X
Instala outros códigos maliciosos X X X   X
Possibilita o retorno do invasor X X
Envia spam e phishing X
Desfere ataques na Internet X X
Procura se manter escondido X    X X X


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





78
128




MAPA MENTAL

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





79
128





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





80
128






Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





81
128







Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





82
128






Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





83
128




QUESTÕES COMENTADAS - FCC 
1. (FCC / TRT 6 - SEGURANÇA - 2018) Ao utilizar um computador, mesmo com aplicativos de segurança instalados, é necessário tomar cuidado, uma vez que novas pragas virtuais podem ser criadas  rapidamente.  Desabilitar  a  autoexecução  de mídias  removíveis  e  não  abrir  ou  não executar arquivos duvidosos pode ajudar a prevenir a infecção e a propagação da praga virtual (malware) do tipo:

a) Worm
b) Bot
c) Backdoor
d) Vírus
e) Rootkit

Comentários:

Backdoor e Rootkit não são obtidos por meio de mídias removíveis infectadas. Já o Worm não é instalado pela execução de um arquivo infectado, de forma que desabilitar a autoexecução de mídias removíveis é uma providência importante para evitar a ação de vírus.

Gabarito: Letra D

2. (FCC  /  METRO  –  SP  -  2018) O usuário de um computador deu um duplo clique sobre um programa recebido por e-mail, executando-o, e seu computador foi infectado por um malware que se propaga inserindo cópias de si mesmo e se tornando parte de outros programas e/ou arquivos. Tais características permitem concluir que o computador foi infectado por um:

a) worm.
b) vírus.
c) rootkit.
d) botnet.
e) backdoor.

Comentários:

O usuário clicou e executou o programa recebido por e-mail e seu computador foi infectado por um malware  que inseriu cópias de si mesmo, logo trata-se de um vírus. Worms não precisam ser executados e nem precisam de arquivos/programas hospedeiros; Rootkits não são recebidos por e- mail; botnets são redes e, não, malwares em si; e backdoor não se propaga.

Gabarito: Letra B

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





84
128




3. (FCC / AGED - MA - 2018) Não importa se um usuário utiliza Microsoft, MacOS, Android ou outro tipo de sistema operacional, pois ao se conectar na internet com um deles, já fica vulnerável a uma infinidade de ataques digitais e pode sofrer com um tipo de malware cuja invasão é realizada com o intuito de causar algum dano ou roubar informações.

(Adaptado de: http://tecnologia.ig.com.br/2017-04-04/malware-cimes-ciberneticos.html) 
O malware referenciado no texto é um programa que, além de executar as funções para as quais foi aparentemente projetado, também executa outras funções maliciosas sem o conhecimento do usuário. Ataca através de programas que necessitam ser explicitamente executados para que sejam  instalados,  mas  também  pode  ser  instalado  por  atacantes  que,  após  invadirem  o computador, alteram programas já existentes para que também executem ações maliciosas.
Este malware é denominado:

a) worm.
b) rootkit.
c) trojan.
d) wanna cry.
e) ransomware

Comentários:

O malware que, além de executar as funções para as quais foi aparentemente projetado, também executa outras funções maliciosas é o Trojan. Ele é um programa que age utilizando o princípio do Cavalo de Troia, em um arquivo é enviado se fazendo passar por um aplicativo útil, como um “presente de grego”, mas que na verdade possui funcionalidades maliciosas escondidas.

Gabarito: Letra C

4. (FCC / AGED - MA - 2018) Ataques cibernéticos causaram prejuízo de US$ 280 bilhões às corporações

A extorsão virtual, quando servidores de empresas são bloqueados e seus gestores só recebem acesso novamente mediante pagamento para os criminosos, também é um dos maiores problemas na América Latina, 28,1%, ficando atrás apenas do bloco de países Asiáticos, 35,1%. Os setores mais  suscetíveis  a  essa  modalidade  de  ataques  cibernéticos  são  serviços  financeiros  (45,8%);
cuidados da saúde (23,7%); energia (23,3%); bens de consumo (22,4%); educação (22,1%); viagem, turismo  e  lazer  (19,8%);  agricultura  (17,9%);  setor  produtivo  (16,3%);  tecnologia,  meios  de comunicação e telecomunicações (13,0%); transporte (11,3%); imobiliário e construção (6,2%) e serviços profissionais (4,8%).

(Disponível em: http://www.convergenciadigital.com.br) 
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





85
128




O texto se refere à “extorsão virtual, quando servidores de empresas são bloqueados e seus gestores só recebem acesso novamente mediante pagamento para os criminosos” e quase 18% deste tipo de ataque atinge o setor de agricultura. A denominação deste tipo de ataque é:

a) bot.
b) spyware.
c) backdoor.
d) ransomware.
e) rootkit.

Comentários:

Extorsão virtual que bloqueia acesso a dados mediante pagamento de recompensa é característica típica de ransomware.

Gabarito: Letra D

5. (FCC / SABESP - 2018) Um Estagiário estava navegando em um site de comércio eletrônico para verificar  os  preços  de  alguns  dispositivos  de  hardware  e  um  malware  passou  a  capturar  e armazenar as teclas digitadas por ele no teclado do computador. Isso ocorreu porque o:

a) estagiário digitou apenas o nome do site, esquecendo-se de digitar SMTPS:\\, para ter acesso a ele. Isso deixou o site vulnerável ao malware.

b) computador estava conectado a uma rede do tipo Wi-Fi com VPN.

c) computador não estava equipado com um firewall, um hardware que bloqueia o acesso de malwares aos dados digitados.

d) computador estava infectado com um spyware do tipo keylogger.

e) computador estava infectado com um malware do tipo bootnet.

Comentários:

Na verdade, o coitado do estagiário não teve culpa. Se um malware passou a capturar e armazenar as teclas digitadas por ele no teclado, é porque seu computador estava infectado por um keylogger – que é um tipo de spyware.

Gabarito: Letra D

6. (FCC / TRT 2 – 2018) Um Analista descobriu que seu computador estava infectado por bots maliciosos. A primeira ação que o Analista deve realizar para proteger os dados deve ser:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





86
128





a) Instalar um antivírus e examinar o computador com seus recursos após a sua instalação.
b) Instalar um antibot, que é uma variação de antivírus específica para proteger o computador contra bots e botnets.
c) Reiniciar o computador para que o bot seja eliminado da memória.
d) Abrir uma ordem de serviço para que o suporte técnico examine o computador.
e) Desconectar o computador da rede o mais rápido possível.

Comentários:

A  recomendação  adequada  para  proteger  dados  diante de  um  ataque  de  bots  maliciosas  – chamados de zumbis – é desconectar o computador da rede o mais rápido possível.

Gabarito: Letra E

7. (FCC / SEGEP-MA - 2018) Em uma situação hipotética, um funcionário da Secretaria de Estado da Gestão e Assistência dos Servidores (SEGEP) verificou que um tipo de código malicioso (malware) havia invadido e tornado inacessíveis os dados armazenados em seu equipamento porque tudo havia sido criptografado. O invasor exigiu pagamento de resgate para restabelecer o acesso. Essa situação mostra a ocorrência do ataque cibernético de um malware conhecido por:

a) Spam.
b) Ransomware.
c) Trojan Spy.
d) Cookie.
e) Worm.

Comentários:

Dados inacessíveis e criptografados cuja liberação se dá sob o pagamento de um resgate é típico de um ransomware.

Gabarito: Letra B

8. (FCC / TRT 24 – 2017) É um conjunto de programas e técnicas que permite esconder e assegurar a presença de um invasor ou de outro código malicioso em um computador comprometido.
Pode  ser  usado  para:  remover  evidências  em  arquivos  de  logs;  instalar  outros  códigos maliciosos, como backdoors, para assegurar o acesso futuro ao computador infectado; esconder atividades e informações, como arquivos, diretórios, processos, chaves de registro, conexões de rede etc.; mapear potenciais vulnerabilidades em outros computadores, por meio de varreduras na rede; capturar informações da rede onde o computador comprometido está localizado, pela interceptação de tráfego; dentre outras possibilidades. No entanto, seu nome não indica que os Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





87
128




programas  e  as  técnicas  que  o  compõem  são  usadas  para  obter  acesso  privilegiado  a  um computador, mas sim para manter o acesso privilegiado.
(Disponível em: http://cartilha.cert.br/malware/) 
O texto descreve um tipo de ameaça à segurança das informações conhecido como:

a) rootkit.
b) engenharia social.
c) wardriving.
d) worm.
e) bot.

Comentários:

Conjunto  de  programas  e  técnicas?  Já  dá  para  desconfiar  que  se  trata  de  um  Rootkit. Permite esconder e assegurar a presença de um invasor ou de outro código malicioso em um computador comprometido? Sim,  é  definitivamente  um  Rootkit.  Engenharia  Social  é  um  golpe  e,  não,  um malware; Wardriving não tem relação com o enunciado; Worm não é um conjunto de programas e técnicas e nem busca esconder a presença de um invasor ou código malicioso; e bot também não é um conjunto de programas e técnicas.

Gabarito: Letra A

9. (FCC / TRE-PR – 2017) Considere a notícia abaixo.

“Um tipo sofisticado de ......... (programa automático de computador projetado para monitorar as atividades  de  um  sistema  e  enviar  as  informações  coletadas  para  terceiros)  vem  infectando sigilosamente centenas de computadores de governos por toda a Europa e nos Estados Unidos, em um dos mais complexos programas de espionagem cibernética descobertos até hoje. Vários pesquisadores em  segurança  e  funcionários  da  área  de  inteligência  ocidentais  dizem  acreditar  que  o  malware, conhecido como ‘Turla’, é um programa espião que está sendo vinculado a uma enorme operação previamente conhecida de espionagem cibernética mundial, apelidada de Outubro Vermelho, e cujo alvo eram redes de pesquisa nuclear, diplomática e militar. Essas constatações se baseiam na análise das táticas empregadas pelos hackers, bem como nos indicadores técnicos e em relatos das vítimas que eram seu alvo.”
(Adaptado de: http://g1.globo.com/tecnologia/noticia/2014/03/) 
Com base nas características descritas do malware, a lacuna do texto é corretamente preenchida por:

a) ransomware.
b) trojan DoS.
c) spyware.
d) addware.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





88
128




e) bootnetspy.

Comentários:

Programa automático de computador projetado para monitorar as atividades de um sistema e enviar as informações coletadas para terceiros é típico de spyware.

Gabarito: Letra C

10. (FCC / DPE/RS – 2017) Cada tipo de código malicioso possui características próprias que o define e o diferencia dos demais tipos. Com relação as ações mais comuns do Backdoor e Rootkit, pode-se afirmar que eles:

a) vem por e-mail e enviam spam e phishing.
b) vem mídias removíveis infectadas e consomem grandes quantidades de recursos.
c) furtam informações sensíveis e enviam cópia de si próprio automaticamente por e-mail.
d) são baixados de sites na internet e desferem ataques na internet.
e) possibilitam os retornos dos invasores, não se propagam e ficam escondidos.

Comentários:

Backdoor e Rootkit não são recebidos por e-mail, não enviam spam nem phishing, não são obtidos por  mídias  removíveis  infectadas,  não  consomem  grande  quantidade  de  recursos,  não  furtam informações sensíveis, não enviam cópias de si próprios automaticamente por e-mail, não são baixados de sites na Internet e não desferem ataques na Internet. Por outro lado, eles possibilitam os retornos dos invasores, não se propagam e ficam escondidos.

Gabarito: Letra E

11. (FCC / AL-MS - 2016) Após o recebimento e a leitura de um email com anexo, o usuário percebeu que o computador foi infectado por algum tipo de malware. Fazendo uma pesquisa na internet, o usuário identificou que o malware que infectou o computador é do tipo worm, pois:

a) arquivos desconhecidos foram instalados no Desktop do computador.
b) arquivos de documentos de texto foram deletados da pasta Documentos.
c) o computador realiza atividades como se estivesse sendo controlado remotamente.
d) o computador enviou várias mensagens de email com propaganda indevidamente.
e) o computador ficou lento indicando grande consumo de recursos.

Comentários:

Apenas  a  última  opção  apresenta  uma  ação  maliciosa típica  de  um  worm,  que  é  deixar  o computador ou rede lenta devido ao alto consumo de recursos.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





89
128





Gabarito: Letra E

12. (FCC / SANASA - 2016) Em uma situação hipotética, ao analisar as características de alguns malwares  que  haviam  invadido  alguns  computadores  da  SANASA,  um  Assistente Administrativo teve que informar o suporte técnico. Para tanto, ele pesquisou na internet e comparou as características pesquisadas com as ocorrências observadas nos computadores. No caso de algumas invasões, por exemplo, ele descobriu que a característica da categoria do malware e a ação de um de seus tipos eram:

−   Característica da Categoria: monitorar as atividades de um sistema e enviar as informações coletadas para terceiros.

−   Ação de um de seus tipos: capturar e armazenar as teclas digitadas pelo usuário no teclado do computador. Sua ativação, em muitos casos, é condicionada a uma ação prévia do usuário, como o acesso a um site específico de comércio eletrônico ou de Internet Banking.

Pela característica da categoria e pela ação de um de seus tipos, respectivamente, tratam-se de:

a) Spyware e Keylogger.
b) Scanner e Spyware.
c) Phishing e Worm.
d) Worm e Screenlogger.
e) Spyware e Spam.

Comentários:

Monitorar as atividades de um sistema e enviar as informações coletadas para terceiros é uma ação maliciosa típica de um Spyware; já capturar e armazenar as teclas digitadas pelo usuário no teclado do computador é uma ação típica de um keylogger.

Gabarito: Letra A

13. (FCC / TRE-AP - 2015) Um usuário de computador observou que, ao conectar um pendrive no computador,  os  arquivos  do  pendrive  foram  transformados  em  atalhos,  não  conseguindo acessar os arquivos originalmente armazenados. Esse sintoma é característico de um malware do tipo:

a) Spyware.
b) Keylogger.
c) Worm.
d) Vírus.
e) Adware.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





90
128





Comentários:

Spywares,  Keyloggers,  Worms  e  Adwares  geralmente  não  transformam  arquivos  de  mídias removíveis em atalhos – essa é uma característica muito comum de vírus. Lembrando que as mídias removíveis são atualmente uma grande fonte de propagação de malwares.

Gabarito: Letra D

14. (FCC / TRE-PB - 2015) Atualmente, a forma mais utilizada para a disseminação de vírus é por meio  de  mensagens  de  e-mails  com  anexos  recebidos  pela  internet.  Para  que  o  vírus  seja ativado:

a) é necessária a transferência do anexo para a Área de trabalho do computador.
b) é necessário que o anexo contaminado seja aberto ou executado.
c) basta realizar a abertura da mensagem para a sua leitura.
d) é suficiente o download da mensagem do servidor de e-mail para o computador.
e) é necessário que, uma vez aberta a mensagem, haja uma conexão com a internet.

Comentários:

(a) Errado, basta que ele seja executado; (b) Correto, o anexo contaminado é um programa e, se ele for executado ou aberto, o computador será contaminado; (c) Errado, apenas abrir a mensagem não executa o anexo – você precisa fazer o download e abri-lo; (d) Errado, apenas fazer o download não executa o anexo – é necessário abri-lo; (e) Errado, não é necessário estar conectado à internet.

Gabarito: Letra B

15. (FCC / DPE-SP – 2013) Analise os exemplos abaixo.

Exemplo  1:  algum  desconhecido  liga  para  a  sua  casa e  diz  ser  do  suporte  técnico  do  seu provedor.  Nesta  ligação  ele  diz  que  sua  conexão  com  a  internet  está  apresentando  algum problema e pede sua senha para corrigi-lo. Caso você entregue sua senha, este suposto técnico poderá realizar atividades maliciosas, utilizando a sua conta de acesso à internet, relacionando tais atividades ao seu nome.

Exemplo 2: você recebe uma mensagem de e-mail, dizendo que seu computador está infectado por um vírus. A mensagem sugere que você instale uma ferramenta disponível em um site da internet para eliminar o vírus de seu computador. A real função desta ferramenta não é eliminar um vírus, mas permitir que alguém tenha acesso ao seu computador e a todos os dados nele armazenados.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





91
128




Exemplo  3:  você  recebe  uma  mensagem  de  e-mail  em  que  o  remetente  é o  gerente  ou  o departamento de suporte do seu banco. Na mensagem é dito que o serviço de Internet Banking está apresentando algum problema e que tal problema pode ser corrigido se você executar o aplicativo  que  está  anexado  à  mensagem. A  execução deste  aplicativo  apresenta  uma  tela análoga àquela que você utiliza para ter acesso à sua conta bancária, aguardando que você digite sua senha. Na verdade, este aplicativo está preparado para furtar sua senha de acesso à conta bancária e enviá-la para o atacante.

Estes casos mostram ataques típicos de:

a) Keylogger.
b) Cavalo de Troia.
c) Botnet.
d) Cookies.
e) Engenharia Social.

Comentários:

Todos os exemplos são típicos casos de engenharia social, em que são utilizados métodos de obtenção de informações importantes do usuário, através de sua ingenuidade ou da confiança.

Gabarito:
Letra E

16. (FCC / TRT-RS – 2011) É uma forma de fraude eletrônica, caracterizada por tentativas de roubo de identidade. Ocorre de várias maneiras, principalmente por e-mail, mensagem instantânea, SMS, dentre outros, e, geralmente, começa com uma mensagem de e-mail semelhante a um aviso oficial de uma fonte confiável, como um banco, uma empresa de cartão de crédito ou um site de comércio eletrônico. Trata-se de:

a) Hijackers.
b) Phishing.
c) Trojans.
d) Wabbit.
e) Exploits.

Comentários:

Fraude eletrônica caracterizada por tentativas de roubo de identidade? Trata-se de uma característica típica do Phishing Scam, isto é, uma fraude em que o golpista tenta enganar um usuário para obtenção de dados pessoais e financeiros que permitam a aplicação de um golpe, combinando técnicas computacionais e de engenharia social.

Gabarito:
Letra B
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





92
128





17. (FCC / TRE-SP – 2017) Considere o texto abaixo.

Com efeito, nesse tipo específico de delito, o agente obtém, para ele ou outrem, vantagem ilícita (numerário  subtraído  de  conta  bancária),  em  prejuízo  de  alguém  (a  vítima,  cliente  de  banco) mediante  o  emprego  do  artifício  da  construção  de  uma  página  eletrônica  falsa  ou  envio  de mensagem  eletrônica  (e-mail)  de  conteúdo  fraudulento.  Não  haveria,  como  se  disse,  qualquer dificuldade de enquadramento do praticante do “ato ilícito” no art. 171 do CPC, impondo-lhe as sanções previstas nesse dispositivo (reclusão, de um a cinco anos, e multa). Além do mais, quando o criminoso implementa o último estágio da execução ilícita, que é a subtração não autorizada dos fundos existentes na conta da vítima, a jurisprudência tem entendido que aí está caracterizado o crime de furto qualificado, previsto no art. 155, § 4° , II.

(Adaptado de: REINALDO FILHO, Democrito. Disponível em: http://www.teleco.com.br/pdfs/tutorialintbank.pdf) 
Hipoteticamente,  um  Analista  Judiciário  do  TRE-SP  identificou,  corretamente,  o  ato  ilícito referido entre aspas no texto como um tipo de fraude por meio da qual um golpista tenta obter dados pessoais e financeiros de um usuário, pela utilização combinada de meios técnicos e engenharia social. Comumente realizado por meio da internet, esse golpe é caracterizado como:

a) identity theft.
b) fielding.
c) phishing.
d) hacker.
e) worming.


Comentários:


Fraude por meio da qual um golpista tenta obter dados pessoais e financeiros de um usuário, pela utilização  combinada  de  meios  técnicos  e engenharia  social? Ora, descrição clássica de Phishing Scam.

Gabarito:
Letra C

18. (FCC / ALE-SE – 2018) Considere o trecho a seguir, retirado do Relatório de Crimes Cibernéticos da empresa Norton:

Vírus de computador e ataques de malware são os tipos mais comuns de crime cibernético que as pessoas sofrem, com 51% dos adultos sentindo os efeitos desses crimes mundialmente. Na Nova Zelândia, Brasil e China é ainda pior, com mais de 6 em 10 computadores infectados (61%, 62% e 65%, respectivamente). Os adultos em todo o mundo também são alvos de golpes (scams) online, ataques de phishing, roubo de perfis de redes sociais e fraude de cartão de crédito. 7% dos adultos até mesmo se depararam com predadores sexuais online.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





93
128




(Disponível em: http://www.symantec.com/content/en/us/home_homeoffice/media/pdf/cybercrime_report/Norton_Portuguese-Hu man%20Impact-A4_Aug18.pdf) 
O phishing, mencionado no texto, é um tipo de golpe por meio do qual um golpista:

a) faz varreduras na rede do usuário, com o intuito de identificar quais computadores estão ativos e quais serviços estão sendo disponibilizados por eles.

b) tenta obter dados pessoais e financeiros de um usuário, pela utilização combinada de meios técnicos e engenharia social.

c) armazena tudo o que o usuário digita pelo teclado do computador e depois obtém estes dados remotamente.

d) altera campos do cabeçalho de um e-mail, de forma a aparentar que ele foi enviado de uma determinada origem quando, na verdade, foi enviado de outra.

e)  utiliza  um  computador  ou  dispositivo  móvel  para tirar  de  operação  um  serviço,  um computador ou uma rede conectada à Internet.


Comentários:


O phishing, mencionado no texto, é um tipo de golpe por meio do qual um golpista tenta obter dados  pessoais  e  financeiros  de  um  usuário,  pela  utilização  combinada  de  meios  técnicos  e engenharia social – nenhum dos outros itens faz qualquer sentido.

Gabarito: Letra B










LISTA DE QUESTÕES - FCC 
1. (FCC / TRT 6 - SEGURANÇA - 2018) Ao utilizar um computador, mesmo com aplicativos de segurança instalados, é necessário tomar cuidado, uma vez que novas pragas virtuais podem ser criadas  rapidamente.  Desabilitar  a  autoexecução  de mídias  removíveis  e  não  abrir  ou  não executar arquivos duvidosos pode ajudar a prevenir a infecção e a propagação da praga virtual (malware) do tipo:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





94
128





a) Worm
b) Bot
c) Backdoor
d) Vírus
e) Rootkit

2. (FCC  /  METRO  –  SP  -  2018) O usuário de um computador deu um duplo clique sobre um programa recebido por e-mail, executando-o, e seu computador foi infectado por um malware que se propaga inserindo cópias de si mesmo e se tornando parte de outros programas e/ou arquivos. Tais características permitem concluir que o computador foi infectado por um:

a) worm.
b) vírus.
c) rootkit.
d) botnet.
e) backdoor.

3. (FCC / AGED - MA - 2018) Não importa se um usuário utiliza Microsoft, MacOS, Android ou outro tipo de sistema operacional, pois ao se conectar na internet com um deles, já fica vulnerável a uma infinidade de ataques digitais e pode sofrer com um tipo de malware cuja invasão é realizada com o intuito de causar algum dano ou roubar informações.

(Adaptado de: http://tecnologia.ig.com.br/2017-04-04/malware-cimes-ciberneticos.html) 
O malware referenciado no texto é um programa que, além de executar as funções para as quais foi aparentemente projetado, também executa outras funções maliciosas sem o conhecimento do usuário. Ataca através de programas que necessitam ser explicitamente executados para que sejam  instalados,  mas  também  pode  ser  instalado  por  atacantes  que,  após  invadirem  o computador, alteram programas já existentes para que também executem ações maliciosas.
Este malware é denominado:

a) worm.
b) rootkit.
c) trojan.
d) wanna cry.
e) ransomware

4. (FCC / AGED - MA - 2018) Ataques cibernéticos causaram prejuízo de US$ 280 bilhões às corporações

A extorsão virtual, quando servidores de empresas são bloqueados e seus gestores só recebem acesso novamente mediante pagamento para os criminosos, também é um dos maiores problemas na América Latina, 28,1%, ficando atrás apenas do bloco de países Asiáticos, 35,1%. Os setores Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





95
128




mais  suscetíveis  a  essa  modalidade  de  ataques  cibernéticos  são  serviços  financeiros  (45,8%);
cuidados da saúde (23,7%); energia (23,3%); bens de consumo (22,4%); educação (22,1%); viagem, turismo  e  lazer  (19,8%);  agricultura  (17,9%);  setor  produtivo  (16,3%);  tecnologia,  meios  de comunicação e telecomunicações (13,0%); transporte (11,3%); imobiliário e construção (6,2%) e serviços profissionais (4,8%).

(Disponível em: http://www.convergenciadigital.com.br) 
O texto se refere à “extorsão virtual, quando servidores de empresas são bloqueados e seus gestores só recebem acesso novamente mediante pagamento para os criminosos” e quase 18% deste tipo de ataque atinge o setor de agricultura. A denominação deste tipo de ataque é:

a) bot.
b) spyware.
c) backdoor.
d) ransomware.
e) rootkit.

5. (FCC / SABESP - 2018) Um Estagiário estava navegando em um site de comércio eletrônico para verificar  os  preços  de  alguns  dispositivos  de  hardware  e  um  malware  passou  a  capturar  e armazenar as teclas digitadas por ele no teclado do computador. Isso ocorreu porque o:

a) estagiário digitou apenas o nome do site, esquecendo-se de digitar SMTPS:\\, para ter acesso a ele. Isso deixou o site vulnerável ao malware.

b) computador estava conectado a uma rede do tipo Wi-Fi com VPN.

c) computador não estava equipado com um firewall, um hardware que bloqueia o acesso de malwares aos dados digitados.

d) computador estava infectado com um spyware do tipo keylogger.

e) computador estava infectado com um malware do tipo bootnet.

6. (FCC / TRT 2 – 2018) Um Analista descobriu que seu computador estava infectado por bots maliciosos. A primeira ação que o Analista deve realizar para proteger os dados deve ser:

a) Instalar um antivírus e examinar o computador com seus recursos após a sua instalação.
b) Instalar um antibot, que é uma variação de antivírus específica para proteger o computador contra bots e botnets.
c) Reiniciar o computador para que o bot seja eliminado da memória.
d) Abrir uma ordem de serviço para que o suporte técnico examine o computador.
e) Desconectar o computador da rede o mais rápido possível.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





96
128




7. (FCC / SEGEP-MA - 2018) Em uma situação hipotética, um funcionário da Secretaria de Estado da Gestão e Assistência dos Servidores (SEGEP) verificou que um tipo de código malicioso (malware) havia invadido e tornado inacessíveis os dados armazenados em seu equipamento porque tudo havia sido criptografado. O invasor exigiu pagamento de resgate para restabelecer o acesso. Essa situação mostra a ocorrência do ataque cibernético de um malware conhecido por:

a) Spam.
b) Ransomware.
c) Trojan Spy.
d) Cookie.
e) Worm.

8. (FCC / TRT 24 – 2017) É um conjunto de programas e técnicas que permite esconder e assegurar a presença de um invasor ou de outro código malicioso em um computador comprometido.
Pode  ser  usado  para:  remover  evidências  em  arquivos  de  logs;  instalar  outros  códigos maliciosos, como backdoors, para assegurar o acesso futuro ao computador infectado; esconder atividades e informações, como arquivos, diretórios, processos, chaves de registro, conexões de rede etc.; mapear potenciais vulnerabilidades em outros computadores, por meio de varreduras na rede; capturar informações da rede onde o computador comprometido está localizado, pela interceptação de tráfego; dentre outras possibilidades. No entanto, seu nome não indica que os programas  e  as  técnicas  que  o  compõem  são  usadas  para  obter  acesso  privilegiado  a  um computador, mas sim para manter o acesso privilegiado.
(Disponível em: http://cartilha.cert.br/malware/) 
O texto descreve um tipo de ameaça à segurança das informações conhecido como:

a) rootkit.
b) engenharia social.
c) wardriving.
d) worm.
e) bot.

9. (FCC / TRE-PR – 2017) Considere a notícia abaixo.

“Um tipo sofisticado de ......... (programa automático de computador projetado para monitorar as atividades  de  um  sistema  e  enviar  as  informações  coletadas  para  terceiros)  vem  infectando sigilosamente centenas de computadores de governos por toda a Europa e nos Estados Unidos, em um dos mais complexos programas de espionagem cibernética descobertos até hoje. Vários pesquisadores em  segurança  e  funcionários  da  área  de  inteligência  ocidentais  dizem  acreditar  que  o  malware, conhecido como ‘Turla’, é um programa espião que está sendo vinculado a uma enorme operação previamente conhecida de espionagem cibernética mundial, apelidada de Outubro Vermelho, e cujo alvo eram redes de pesquisa nuclear, diplomática e militar. Essas constatações se baseiam na análise Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





97
128




das táticas empregadas pelos hackers, bem como nos indicadores técnicos e em relatos das vítimas que eram seu alvo.”
(Adaptado de: http://g1.globo.com/tecnologia/noticia/2014/03/) 
Com base nas características descritas do malware, a lacuna do texto é corretamente preenchida por:

a) ransomware.
b) trojan DoS.
c) spyware.
d) addware.
e) bootnetspy.

10. (FCC / DPE/RS – 2017) Cada tipo de código malicioso possui características próprias que o define e o diferencia dos demais tipos. Com relação as ações mais comuns do Backdoor e Rootkit, pode-se afirmar que eles:

a) vem por e-mail e enviam spam e phishing.
b) vem mídias removíveis infectadas e consomem grandes quantidades de recursos.
c) furtam informações sensíveis e enviam cópia de si próprio automaticamente por e-mail.
d) são baixados de sites na internet e desferem ataques na internet.
e) possibilitam os retornos dos invasores, não se propagam e ficam escondidos.

11. (FCC / AL-MS - 2016) Após o recebimento e a leitura de um email com anexo, o usuário percebeu que o computador foi infectado por algum tipo de malware. Fazendo uma pesquisa na internet, o usuário identificou que o malware que infectou o computador é do tipo worm, pois:

a) arquivos desconhecidos foram instalados no Desktop do computador.
b) arquivos de documentos de texto foram deletados da pasta Documentos.
c) o computador realiza atividades como se estivesse sendo controlado remotamente.
d) o computador enviou várias mensagens de email com propaganda indevidamente.
e) o computador ficou lento indicando grande consumo de recursos.

12. (FCC / SANASA - 2016) Em uma situação hipotética, ao analisar as características de alguns malwares  que  haviam  invadido  alguns  computadores  da  SANASA,  um  Assistente Administrativo teve que informar o suporte técnico. Para tanto, ele pesquisou na internet e comparou as características pesquisadas com as ocorrências observadas nos computadores. No caso de algumas invasões, por exemplo, ele descobriu que a característica da categoria do malware e a ação de um de seus tipos eram:

−   Característica da Categoria: monitorar as atividades de um sistema e enviar as informações coletadas para terceiros.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





98
128




−   Ação de um de seus tipos: capturar e armazenar as teclas digitadas pelo usuário no teclado do computador. Sua ativação, em muitos casos, é condicionada a uma ação prévia do usuário, como o acesso a um site específico de comércio eletrônico ou de Internet Banking.

Pela característica da categoria e pela ação de um de seus tipos, respectivamente, tratam-se de:

a) Spyware e Keylogger.
b) Scanner e Spyware.
c) Phishing e Worm.
d) Worm e Screenlogger.
e) Spyware e Spam.

13. (FCC / TRE-AP - 2015) Um usuário de computador observou que, ao conectar um pendrive no computador,  os  arquivos  do  pendrive  foram  transformados  em  atalhos,  não  conseguindo acessar os arquivos originalmente armazenados. Esse sintoma é característico de um malware do tipo:

a) Spyware.
b) Keylogger.
c) Worm.
d) Vírus.
e) Adware.

14. (FCC / TRE-PB - 2015) Atualmente, a forma mais utilizada para a disseminação de vírus é por meio  de  mensagens  de  e-mails  com  anexos  recebidos  pela  internet.  Para  que  o  vírus  seja ativado:

a) é necessária a transferência do anexo para a Área de trabalho do computador.
b) é necessário que o anexo contaminado seja aberto ou executado.
c) basta realizar a abertura da mensagem para a sua leitura.
d) é suficiente o download da mensagem do servidor de e-mail para o computador.
e) é necessário que, uma vez aberta a mensagem, haja uma conexão com a internet.

15. (FCC / DPE-SP – 2013) Analise os exemplos abaixo.

Exemplo  1:  algum  desconhecido  liga  para  a  sua  casa e  diz  ser  do  suporte  técnico  do  seu provedor.  Nesta  ligação  ele  diz  que  sua  conexão  com  a  internet  está  apresentando  algum problema e pede sua senha para corrigi-lo. Caso você entregue sua senha, este suposto técnico poderá realizar atividades maliciosas, utilizando a sua conta de acesso à internet, relacionando tais atividades ao seu nome.

Exemplo 2: você recebe uma mensagem de e-mail, dizendo que seu computador está infectado por um vírus. A mensagem sugere que você instale uma ferramenta disponível em um site da internet para eliminar o vírus de seu computador. A real função desta ferramenta não é eliminar Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





99
128




um vírus, mas permitir que alguém tenha acesso ao seu computador e a todos os dados nele armazenados.

Exemplo  3:  você  recebe  uma  mensagem  de  e-mail  em  que  o  remetente  é o  gerente  ou  o departamento de suporte do seu banco. Na mensagem é dito que o serviço de Internet Banking está apresentando algum problema e que tal problema pode ser corrigido se você executar o aplicativo  que  está  anexado  à  mensagem. A  execução deste  aplicativo  apresenta  uma  tela análoga àquela que você utiliza para ter acesso à sua conta bancária, aguardando que você digite sua senha. Na verdade, este aplicativo está preparado para furtar sua senha de acesso à conta bancária e enviá-la para o atacante.

Estes casos mostram ataques típicos de:

a) Keylogger.
b) Cavalo de Troia.
c) Botnet.
d) Cookies.
e) Engenharia Social.

16. (FCC / TRT-RS – 2011) É uma forma de fraude eletrônica, caracterizada por tentativas de roubo de identidade. Ocorre de várias maneiras, principalmente por e-mail, mensagem instantânea, SMS, dentre outros, e, geralmente, começa com uma mensagem de e-mail semelhante a um aviso oficial de uma fonte confiável, como um banco, uma empresa de cartão de crédito ou um site de comércio eletrônico. Trata-se de:

a) Hijackers.
b) Phishing.
c) Trojans.
d) Wabbit.
e) Exploits.

17. (FCC / TRE-SP – 2017) Considere o texto abaixo.

Com efeito, nesse tipo específico de delito, o agente obtém, para ele ou outrem, vantagem ilícita (numerário  subtraído  de  conta  bancária),  em  prejuízo  de  alguém  (a  vítima,  cliente  de  banco) mediante  o  emprego  do  artifício  da  construção  de  uma  página  eletrônica  falsa  ou  envio  de mensagem  eletrônica  (e-mail)  de  conteúdo  fraudulento.  Não  haveria,  como  se  disse,  qualquer dificuldade de enquadramento do praticante do “ato ilícito” no art. 171 do CPC, impondo-lhe as sanções previstas nesse dispositivo (reclusão, de um a cinco anos, e multa). Além do mais, quando o criminoso implementa o último estágio da execução ilícita, que é a subtração não autorizada dos fundos existentes na conta da vítima, a jurisprudência tem entendido que aí está caracterizado o crime de furto qualificado, previsto no art. 155, § 4° , II.

(Adaptado de: REINALDO FILHO, Democrito. Disponível em: http://www.teleco.com.br/pdfs/tutorialintbank.pdf) Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





100
128





Hipoteticamente,  um  Analista  Judiciário  do  TRE-SP  identificou,  corretamente,  o  ato  ilícito referido entre aspas no texto como um tipo de fraude por meio da qual um golpista tenta obter dados pessoais e financeiros de um usuário, pela utilização combinada de meios técnicos e engenharia social. Comumente realizado por meio da internet, esse golpe é caracterizado como:

a) identity theft.
b) fielding.
c) phishing.
d) hacker.
e) worming.


18. (FCC / ALE-SE – 2018) Considere o trecho a seguir, retirado do Relatório de Crimes Cibernéticos da empresa Norton:

Vírus de computador e ataques de malware são os tipos mais comuns de crime cibernético que as pessoas sofrem, com 51% dos adultos sentindo os efeitos desses crimes mundialmente. Na Nova Zelândia, Brasil e China é ainda pior, com mais de 6 em 10 computadores infectados (61%, 62% e 65%, respectivamente). Os adultos em todo o mundo também são alvos de golpes (scams) online, ataques de phishing, roubo de perfis de redes sociais e fraude de cartão de crédito. 7% dos adultos até mesmo se depararam com predadores sexuais online.

(Disponível em: http://www.symantec.com/content/en/us/home_homeoffice/media/pdf/cybercrime_report/Norton_Portuguese-Hu man%20Impact-A4_Aug18.pdf) 
O phishing, mencionado no texto, é um tipo de golpe por meio do qual um golpista:

a) faz varreduras na rede do usuário, com o intuito de identificar quais computadores estão ativos e quais serviços estão sendo disponibilizados por eles.

b) tenta obter dados pessoais e financeiros de um usuário, pela utilização combinada de meios técnicos e engenharia social.

c) armazena tudo o que o usuário digita pelo teclado do computador e depois obtém estes dados remotamente.

d) altera campos do cabeçalho de um e-mail, de forma a aparentar que ele foi enviado de uma determinada origem quando, na verdade, foi enviado de outra.

e)  utiliza  um  computador  ou  dispositivo  móvel  para tirar  de  operação  um  serviço,  um computador ou uma rede conectada à Internet.





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





101
128




GABARITO
1. LETRA D
2. LETRA B
3. LETRA C
4. LETRA D
5. LETRA D
6. LETRA E
7. LETRA B
8. LETRA A
9. LETRA C
10. LETRA E
11. LETRA E
12. LETRA A
13. LETRA D
14. LETRA B
15. LETRA E
16. LETRA B
17. LETRA C
18. LETRA B





















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





102
128




QUESTÕES COMENTADAS – DIVERSAS BANCAS 
1. (CONSULPLAN  /  TJ-MG  –  2017)  Códigos  maliciosos  (malwares)  são  programas especificamente desenvolvidos para executar ações danosas e atividades maliciosas em um computador.  O  programa  que  permite  o  retorno  de  um invasor  a  um  computador comprometido,  por  meio  da  inclusão  de  serviços  criados  ou  modificados  para  este  fim  é conhecido como:

a) Backdoor.
b) Spyware.
c) Worm.
d) Rootkit.

Comentários:

Programa que permite o retorno de um invasor a um computador comprometido é típico de um backdoor. Professor, por que não poderia ser rootkit? Porque o rootkit é um conjunto de ferramentas e técnicas que também permite o retorno de um invasor.

Gabarito: Letra A

2. (CONSULPLAN / TRE-MG – 2015) Malware são programas especificamente desenvolvidos para executar ações danosas e atividades maliciosas no computador. O worm é um dos tipos de malware  que  se  propaga  automaticamente  pelas  redes,  enviando  cópias  de  si  mesmo  de computador  para  computador.  Quanto  a  um  ataque  desta  natureza,  assinale  a  alternativa INCORRETA.

a) Faz a inclusão de si mesmo em outros programas ou arquivos.
b) Necessita identificar os computadores-alvo para os quais tentará se copiar.
c) Na propagação pode afetar o desempenho de redes e uso dos computadores.
d) Explora vulnerabilidades existentes em programas instalados no computador-alvo.

Comentários:

(a) Errado, ele se propaga pela execução direta de suas cópias; (b) Correto, ele possui uma fase de identificação de computadores-alvo; (c) Correto, a sua propagação afeta o desempenho da rede e de computadores; (d) Correto, ele realmente explora vulnerabilidades existentes em programas instalados no computador-alvo.

Gabarito: Letra A

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





103
128




3. (COPESE / DPE-TO – 2015) Defacers são os pichadores virtuais especializados em desfigurar páginas de sites na Internet.

Comentários:

Defacers são realmente pichadores virtuais de páginas web. Eles utilizam uma técnica que consiste em alterar o conteúdo da página web. Para ganhar mais visibilidade, chamar mais atenção e atingir maior número de visitantes, geralmente os atacantes alteram a página principal do site, porém páginas internas também podem ser alteradas.

Gabarito: Correto

4. (UFPEL / UFPEL – 2013) Um software malicioso é um software intencionalmente incluído ou inserido em um sistema para um propósito prejudicial. Nesse contexto, analise as informações relacionadas aos vírus de computador.

I - Um vírus pode estar anexado a um programa de computador.

II  -  Uma  maneira  de  se  prevenir,  detectar  e  eliminar  um  vírus  é  através  de  um  programa denominado de WinZip.

III - A infecção de um vírus pode se propagar de um computador para outro, mesmo que ambos estejam desligados.

Está(ão) correta(s):

a) apenas I.
b) apenas II.
c) apenas III.
d) apenas I e II.
e) apenas II e III.

Comentários:

(I) Correto, um vírus frequentemente está anexado a algum programa de computador; (II) Errado, Winzip é apenas um compactador de arquivos – ele não é capaz de prevenir, detectar ou eliminar vírus; (III) Errado, caso eles estejam desligados, os vírus não podem se propagar.

Gabarito: Letra A

5. (OBJETIVA / Prefeitura de Terra de Areia/RS – 2016) Segundo a Cartilha de Segurança para Internet, alguns sistemas operacionais permitem que o usuário compartilhe com outros usuários Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





104
128




recursos do seu computador, como diretórios, discos e impressoras. Com base nisso, em relação às formas de prevenção, assinalar a alternativa INCORRETA:

a) Estabelecer senhas para os compartilhamentos.
b) Compartilhar os recursos pelo tempo mínimo necessário.
c) Ter um antimalware instalado no computador, mantê-lo atualizado e utilizá-lo para verificar qualquer arquivo compartilhado.
d)  Estabelecer  permissões  de  acesso  inadequadas,  permitindo  que  usuários  do compartilhamento tenham mais acessos que o necessário.
e) Manter o computador protegido, com as versões mais recentes e com todas as atualizações aplicadas.

Comentários:

(a) Correto, recomenda-se estabelecer senhas para compartilhamento; (b) Correto, recomenda-se compartilhar os recursos apenas pelo período necessário e nada mais; (c) Correto, essa é uma das melhores  recomendações:  ter  um  antimalware  atualizado  para  verificar  qualquer  arquivo compartilhados;  (d)  Errado,  recomenda-se  estabelecer  permissões  de  acesso  adequadas, permitindo que usuários do compartilhamento tenham acesso apenas ao que é necessário; (e) Errado, recomenda-se de fato manter o computador protegido, com as versões mais recentes e com todas as atualizações aplicadas.

Gabarito: Letra D

6. (OBJETIVA / Prefeitura de Porto Barreiro/PR – 2016) Em conformidade com a Cartilha de Segurança para Internet, sobre a segurança em conexões web, analisar os itens abaixo:

I - O protocolo HTTP, além de não oferecer criptografia, também não garante que os dados não possam ser interceptados, coletados, modificados ou retransmitidos, nem que o usuário esteja se comunicando exatamente com o site desejado. Por essas características, ele não é indicado para transmissões que envolvem informações sigilosas, como senhas, números de cartão de crédito e dados bancários, e deve ser substituído pelo HTTPS, que oferece conexões seguras.

II - O protocolo HTTPS utiliza certificados digitais para assegurar a identidade, tanto do site de destino quanto a sua própria, caso o usuário possua um. Também utiliza métodos criptográficos e outros protocolos, como o SSL (Secure Sockets Layer) e o TLS (Transport Layer Security), para assegurar a confidencialidade e a integridade das informações.

a) Os itens I e II estão corretos.
b) Somente o item I está correto.
c) Somente o item II está correto.
d) Os itens I e II estão incorretos.

Comentários:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





105
128





(I) Correto, item impecável – se você precisa de uma comunicação mais segura, deve utilizar HTTPS e, não, HTTP; (II) Correto, ele realmente utiliza certificados – esse protocolo utiliza métodos dos protocolos SSL e TLS.

Gabarito: Letra A

7. (OBJETIVA  /  Prefeitura  de  Tramandaí/RS  –  2015) Em  conformidade  com  a  Cartilha  de Segurança para Internet, em relação aos cuidados a serem tomados ao aceitar um certificado digital, marcar C para as afirmativas Certas, E para as Erradas e, após, assinalar a alternativa que apresenta a sequência CORRETA:

( ) Manter o sistema operacional e navegadores web atualizados (além disso contribuir para a segurança geral do computador, também serve para manter as cadeias de certificados sempre atualizadas).

(  )  Manter  o  computador  com  a  data  correta.  Além  de  outros  benefícios, isso impede que certificados válidos sejam considerados não confiáveis e, de forma contrária, que certificados não confiáveis sejam considerados válidos.

( ) Ao acessar um site web, observar os símbolos indicativos de conexão segura e ler com atenção eventuais alertas exibidos pelo navegador.

a) C - C - C.
b) C - E - C.
c) E - C - E.
d) E - E - E.

Comentários:

(I) Correto, é bastante recomendável manter o sistema operacional e navegadores web atualizados para melhorar a segurança; (II) Correto, isso parece besta, mas é importante manter a data correta para a validação dos certificados digitais; (III) Correto, é interessante observar o cadeado verde que existe na maioria dos navegadores, assim como os alertas.

Gabarito:
Letra A

8. (OBJETIVA / Prefeitura de Agudo/RS – 2015) Segundo a Cartilha de Segurança para Internet, falsificação de e-mail é uma técnica que consiste em alterar campos do cabeçalho de um e-mail, de forma a aparentar que ele foi enviado de uma determinada origem quando, na verdade, foi enviado de outra. Exemplos de e-mails com campos falsificados são aqueles recebidos como sendo:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





106
128




I - De alguém conhecido, solicitando que o usuário clique em um link ou execute um arquivo anexo.

II - Do banco do usuário, solicitando que ele siga um link fornecido na própria mensagem e informe dados da sua conta bancária.

III - Do administrador do serviço de e-mail que o usuário utiliza, solicitando informações pessoais e ameaçando bloquear a sua conta caso o usuário não as envie.

Estão CORRETOS:

a) Somente os itens I e II.
b) Somente os itens I e III.
c) Somente os itens II e III.
d) Todos os itens.

Comentários:

(I) Correto, não é recomendado executar arquivos nem de pessoas conhecidas porque o e-mail pode ter sido falsificado; (II) Correto, esse é um clássico – bancos não enviam e-mail sem autorização explícita do usuário. Fornecendo link e informando dados da conta bancária, pior ainda; (III) Correto, solicitar informações pessoais e ameaças de bloqueio são exemplos de possíveis falsificações de e- mail.

Gabarito: Letra D

9. (OBJETIVA / Prefeitura de Chapecó/SC – 2011) Assinalar a alternativa que preenche a lacuna abaixo CORRETAMENTE:

Os _______ são e-mails não solicitados, que geralmente são enviados para um grande número de  pessoas.  Quando  o  conteúdo  é  exclusivamente  comercial,  esse  tipo  de  mensagem  é denominado UCE (do inglês Unsolicited Commercial E-mail).

a) vírus
b) spams
c) Cavalos de Troia
d) trojans

Comentários:

Os spams são e-mails não solicitados, que geralmente são enviados para um grande número de pessoas. Quando o conteúdo é exclusivamente comercial, esse tipo de mensagem é denominado UCE (do inglês Unsolicited Commercial E-mail).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





107
128




Gabarito: Letra B

10. (PUC-PR / TJ-MS – 2015) A respeito de segurança da informação, é CORRETO afirmar que um Worm é:

a) um programa ou parte de um programa de computador que se propaga por meio de cópias de si mesmo, infectando outros programas e arquivos de computador. O Worm depende da execução do programa ou do hospedeiro para ser ativado.

b) um programa que procura dar a garantia de retorno a um computador invadido, sem utilizar novas técnicas de invasão, ou que retorna ao computador invadido sem ser notado.

c) um software espião que tem como objetivo monitorar atividades de um sistema e enviar as informações coletadas para terceiros.

d) um tipo de software projetado para apresentar propagandas, seja por meio de um navegador (browser), seja com algum outro programa instalado em um computador.

e) um programa capaz de se propagar automaticamente através de redes, enviando cópias de si mesmo de computador para computador. Difere do vírus por não embutir cópias de si mesmo em outros programas ou arquivos.

Comentários:

(a)  Errado,  worms  não  infectam  outros  programas  nem  depende  de  execução  do  programa hospedeiro; (b) Errado, esse item trata do Backdoor; (c) Errado, esse item trata do Spyware; (d) Errado,  esse  item  trata  do  Adware;  (e)  Correto.  Worms  realmente  são  capazes  de  propagar automaticamente através de redes, enviando cópias de si mesmo de computador para computador e diferem do vírus por não embutir cópias de si mesmo em outros programas ou arquivos.

Gabarito:
Letra E

11. (PUC-PR  /  TCE-MS  –  2013) De  modo  geral,  são  considerados  como  malware  softwares destinados a se infiltrar em um sistema de computador alheio de forma ilícita, com intuito de causar algum dano ou roubo de informação. Vírus de computador, worms, trojans e spywares são variações de malwares, cada qual com comportamentos e objetivos distintos. Um malware é classificado como worm quando possui a característica de:

a) apenas se propagar quando executado por um usuário, vindo de arquivo anexo em e-mail ou mensagens em redes sociais.

b) se propagar de computador para computador sozinho, sem ter que se anexar a algo ou alguma coisa.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





108
128





c) se esconder dentro de outros softwares, para ser acionado inadvertidamente pelo usuário.

d) inundar sites de internet com requisições de informação e solicitação de serviços, para que fiquem lentos ou caiam.

e) monitorar os dados que trafegam em uma rede, podendo capturar senhas e informações confidenciais.


Comentários:

(a) Errado, eles são capazes de propagar automaticamente; (b) Correto, worms podem ser propagar de computador para computador sozinho, sem ter que se anexar a algo ou alguma coisa; (c) Errado, worms não precisam de hospedeiros para se propagar; (d) Errado, a questão trata de um ataque de Ping Flood; (e) Errado, a questão de um programa chamado Sniffer.

Gabarito: Letra B

12. (IDIB / CRF-RJ – 2018) Acerca dos tipos de vírus, analise as seguintes afirmativas.

I. Os vírus de arquivos infectam arquivos de programas e arquivos criados por usuários.

II. Os vírus de macro são vírus que tem seu código fonte (linhas de comando) criptografado, ou seja, os caracteres da programação são alterados para outros caracteres.

III. Os vírus de boot infectam os arquivos de inicialização do sistema, escondendo-se no primeiro setor do disco e são carregados na memória antes do sistema operacional.

De acordo com as afirmativas acima, marque a alternativa correta.

a) Apenas a afirmativa I está correta.
b) Apenas as afirmativas I e II estão corretas.
c) Apenas as afirmativas I e III estão corretas.
d) Apenas as afirmativas II e III estão corretas.

Comentários:

I – Correto. Os vírus podem infectar tanto programas no computador, quanto arquivos criados pelo usuário, como imagens, documentos de texto e etc.

II – Errado. O vírus de macro é um tipo específico de vírus de script (escritos neste tipo de linguagem, como VBscript e JavaScript), normalmente recebido ao acessar páginas web ou por e-mail, e que tenta infectar arquivos manipulados por aplicativos que utilizam essas linguagens mencionadas Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





109
128




anteriormente como, por exemplo, os arquivos que compõe o Microsoft Office (Excel, Word e PowerPoint, entre outros).

III – Correto. O Vírus de Boot é um dos primeiros tipos de vírus conhecidos e infecta a parte de inicialização do sistema operacional, escondendo-se no primeiro setor da memória.

Gabarito:
Letra C

13. (IDIB / CRF RJ – 2018) Considerando que arquivos de computadores podem ser infectados por vírus ou serem portadores deles, marque a alternativa com o tipo de arquivo que NÃO pode ser infectado ou propagado por eles.

a) .doc
b) .docx
c) .txt
d) .xls

Comentários:

Todos os arquivos acima poderão ser infectados por vírus, com exceção do arquivo .txt que o formato de um texto simples. Geralmente, é o arquivo produzido pelo bloco de notas.

Gabarito: Letra C

14. (FADESP  /  BANPARÁ  –  2018) Sobre  os  conceitos  de  segurança,  vírus  e  ataques  a computadores, analise as seguintes afirmativas:

I.  A  criptografia  assimétrica  utiliza  uma  chave  única,  que  é  usada  para  cifrar  e  decifrar mensagens. Já a criptografia simétrica emprega um par de chaves, sendo uma privada e uma pública, que são usadas para cifrar e decifrar as mensagens, respectivamente.

II.  Engenharia  social  é  o  termo  usado  para  designar  práticas  utilizadas  a  fim  de  se  obter informações  sigilosas  ou  importantes  de  empresas,  usuários  e  sistemas  de  informação, explorando a confiança das pessoas para enganá-las.

III. São conhecidos como spammers os responsáveis pelo envio de diversas mensagens não solicitadas  para  muitos  usuários.  No  entanto,  o  termo spam  é  empregado  apenas  para  as mensagens  enviadas  por  meio  de  um  correio  eletrônico,  não  envolvendo,  portanto,  as mensagens veiculadas em outros meios como blogs, fóruns e redes sociais.

Está(ão) correto(s) o(s) item(ns):

a) II.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





110
128




b) III.
c) I e II.
d) II e III.
e) I, II e III.

Comentários:

(I) Errado. A questão inverteu os conceitos de criptografia simétrica e assimétrica; (II) Correto. A Engenharia Social é um método ou habilidade de extrair dados através da persuasão e manipulação psicológica de indivíduos. É um dos mais perigosos ataques, pois exige atenção e educação de seres humanos – item impecável; (III) Errado. O termo Spam é empregado para designar, no geral, todo tipo de lixo eletrônico, inclusive os que são vinculados por grandes sites e portais.

Gabarito:
Letra A

15. (FADESP / BANPARÁ – 2018) Sobre segurança no acesso à Internet, analise as afirmativas a seguir.

I. Phishing é uma prática utilizada para coletar informações pessoais, como senhas e número de contas bancárias. Uma tentativa de phishing pode acontecer através do contato do usuário com páginas Web construídas para imitar sites de bancos e outras instituições.

II. O ataque do homem–do–meio refere–se à forma de ataque em que uma comunicação entre duas  pessoas  é  interceptada  por  uma  terceira.  O  atacante  simplesmente  recebe  e, opcionalmente,  repassa  as  informações  do  transmissor  para  o  receptor,  sem  que  ambos percebam que a comunicação não está sendo, de fato, direta.

III. Ransomware é um software malicioso que bloqueia o acesso do usuário aos arquivos do computador. Os criminosos exigem alguma forma de recompensa mediante a promessa de que o acesso aos dados será restabelecido.

Com base na análise realizada, é correto afirmar que 
a) somente a afirmativa I é verdadeira.
b) somente a afirmativa II é verdadeira.
c) somente as afirmativas I e III são verdadeiras.
d) somente as afirmativas II e III são verdadeiras.
e) todas as afirmativas são verdadeiras.

Comentários:

(I) Correto. O Phishing é uma fraude em que o golpista tenta enganar um usuário para obtenção de dados  pessoais  e  financeiros  que  permitam  a  aplicação  de  um  golpe,  combinando  técnicas computacionais e de engenharia social;
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





111
128





(II) Correto. O Man in the Middle é um ataque em que os dados trocados entre duas partes (Ex: você e o seu banco) são de alguma forma interceptados, registrados e possivelmente alterados pelo atacante sem que as vítimas percebam;

(III)  Correto.  O  Ransomware  é  um  tipo  de  código  malicioso  que  torna  inacessíveis  os  dados armazenados em um equipamento, geralmente utilizando criptografia, e que exige pagamento de um resgate (ransom, em inglês) para restabelecer o acesso ao usuário – trata-se de uma espécie de extorsão virtual.

Gabarito: Letra E

16. (IBADE / PREVES – 2017) Em se tratando de vírus de computador, classificam-se as fases de execução de um vírus em 4 fases distintas. A fase em que o vírus está se replicando, infectando novos arquivos em outros sistemas é conhecida como a fase de:

a) ação.
b) carga.
c) ativação.
d) propagação.
e) dormência.

Comentários:

(a) Errado. Durante a ação, a função é executada! Ela pode ser inofensiva, como uma mensagem na tela, ou danosa, como a destruição de programas e arquivos de dados.

(b) Errado. Carga é um dos componentes de um vírus. Trata-se do que o vírus faz, além de se espalhar. A carga útil pode envolver algum dano ou atividade benigna, porém notável.

(c) Errado. Durante a Ativação, o vírus é ativado para executar a função pretendida. Como ocorre com a fase de dormência, a fase de ativação pode ser causada por uma variedade de eventos de sistema, incluindo a contagem do número de vezes que essa cópia de vírus fez uma cópia de si mesma.

(d) Correto. Durante a Propagação, o vírus instala uma cópia de si mesmo em outros programas ou em certas áreas do sistema no disco. A cópia pode não ser idêntica à versão de propagação; muitas vezes, os vírus mudam de forma para escapar à detecção. Agora, cada programa infectado conterá um clone do vírus, que também entrará em uma fase de propagação.

(e) Errado. Durante a Dormência, o vírus está ocioso. A certa altura, ele será ativado por algum evento, como uma data, a presença de outro programa ou arquivo, ou a ultrapassagem de algum limite de capacidade de disco. Nem todos os vírus têm esse estágio.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





112
128




Gabarito: Letra D

17. (IBADE / IPERON – 2017) Um usuário precisa instalar em seu microcomputador um software antivírus de mercado, para se prevenir de ataques. Um software dessa categoria é o:

a) Adware.
b) Broadsheet.
c) Kaspersky.
d) Media Player.
e) Switcher.

Comentários:

(a) Errado, Adware é um software malicioso;
(b) Errado. Broadsheet é um cartaz de jornal;
(c) Correto, Kaspersky é um antivírus de mercado;
(d) Errado, Media Player é um tocador de áudio/vídeo;
(e) Errado, Switcher é um interruptor.

Gabarito: Letra C

18. (IBADE / PM AC – 2017) Para manter um computador livre de vírus, o procedimento mais recomendado é:

a) desfragmentar o disco rígido semanalmente.
b) instalar e rodar um software de localização.
c) Instalar e rodar um antivírus.
d) varrer o disco removível antes de usá-lo.
e) fazer uma cópia física de segurança do disco removível.

Comentários:

O único dos procedimentos listados que permite manter o computador livre de vírus é instalar e rodar um antivírus.

Gabarito:
Letra C

19. (CETAP  /  Prefeitura  de  Ananindeua-PA  –  2019) Os  vírus  são  softwares  que  prejudicam  o computador, fazendo com que o mesmo fique lento ou até mesmo pare de funcionar. É exemplo de vírus:

a) Mcafee.
b) AVG.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





113
128




c) Norton.
d) Chameleon.

Comentários:

(a) Errado, esse é um exemplo de Antivírus; (b) Errado, esse é um exemplo de Antivírus; (c) Errado, esse  é  um  exemplo  de  Antivírus;  (d)  Correto,  esse  é  um  exemplo  de  vírus.  Lembrando  que Chameleon é um virus polimórfico da década de noventa que atinge arquivos .com.

Gabarito:
Letra D

20. (CETAP / Prefeitura de Ananindeua-PA – 2019) Firewall é uma solução de segurança baseada em hardware ou software (mais comum), onde sua função é:

a) separar os e-mails desejados dos indesejados (spams).
b) alertar o usuário quando há um problema no teclado.
c) alertar o usuário que há uma nova atualização do Word2010.
d) Controlar a movimentação de todos os dados do computador através da internet. Prevenir o vazamento de informações do computador para a internet, fazendo o bloqueio de acesso de softwares maliciosos que podem prejudicar o computador.

Comentários:

(a) Errado, essa é uma função do Antispam; (b) Errado, essa não é uma função do Firewall; (c) Errado, essa é uma função do Windows Update; (d) Correto, essa é uma função do Firewall.

Gabarito: Letra D

21. (CETAP / Prefeitura de Barcarena-PA – 2016) No contexto da segurança da informação, existe um sistema que é usado para prevenir o acesso não autorizado de usuários da Internet a uma rede  privada  (intranet).  Esse  sistema  pode  ser  implementado  em  hardware,  software  ou combinação de ambos. As mensagens que entram e saem da intranet devem passar por esse sistema que aplica suas políticas de segurança para permitir ou não a transmissão das mesmas.
Esse sistema é denominado:

a) Antispyware.
b) Firewall
c) Cavalo de tróia.
d) Antivírus.

e) Adware.

Comentários:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





114
128




Impedir  acesso  não  autorizado  a  uma  rede  privada?  Pode  ser  implementado  em  hardware  e/ou software? Mensagens passam por políticas de segurança? Só pode estar falando de Firewall!

Gabarito: Letra B

22. (CETAP / Prefeitura de São Miguel do Guamá/PA – 2016) A Segurança da Informação é a área da  Tecnologia  da  Informação  responsável  por  proteger  a  informação  contra  acessos  não autorizados, de modo a preservar seu valor. Analise as afirmativas seguintes sobre Segurança da Informação e assinale a alternativa correta:

I - Firewalls são programas de computador utilizados para prevenir, detectar e eliminar vírus de computador.

II - Spywares são programas maliciosos cujo objetivo é monitorar as atividades do usuário no computador e enviar as informações coletadas para terceiros através da Internet.

III - Vírus de computador são programas maliciosos capazes de infectar programas e arquivos do computador, podem fazer cópias de si mesmo e espalhar-se para outros computadores em rede.

IV - Cavalo de Tróia (Trojan Horse) são programas maliciosos que abrem portas no computador para possíveis ataques.

V - Anti-vírus são programas de computador que tem como objetivo proteger o computador ou uma rede de computadores, liberando ou bloqueando o tráfego de dados entre o computador e a rede externa de acordo com regras estabelecidas.

a) Todas as afirmativas estão corretas.
b) Somente as afirmativas I, II e III estão corretas.
c) Somente as afirmativas III e V estão corretas.
d) Somente as afirmativas II, III e IV estão corretas.
e) Somente as afirmativas I e V estão corretas.

Comentários:

(I) Errado, Firewalls controlam acessos a redes privadas – ele nada fazem contra vírus; (II) Correto, essa  é  a  definição  perfeita  de  spywares;  (III)  Correto,  trojans  são  capazes  de  abrir  portas  no computador para possíveis ataques futuros; (IV) Correto, antivírus de fato protegem computadores e redes. No entanto quem libera/bloqueia tráfego de dados entre computadores e rede externa são os Firewalls. Logo, apesar do gabarito definitivo correto, eu discordo!

Gabarito: Letra D

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





115
128




23. (CETAP  Prefeitura  de  Abaetetuba/PA  –  2016) No  contexto  de  segurança  da  informação, marque a alternativa que apresenta a definição correta de anti-spyware:

a)  Software  que  se  auto  instala  no  computador,  monitora  a  atividade  do  usuário  e, periodicamente, reporta suas atividades para outro computador na Internet.

b) É uma barreira de software ou hardware entre um ou mais computadores e a Internet.

c) Propaganda não desejada recebida por email.

d)  Software  que  executa  no  servidor  e  fica  posicionado  entre  as  estações  de  trabalho  dos usuários e a Internet. São usados nas organizações para prover mais controle administrativo, serviço de caching, monitoramente e registro das atividades da rede.


e) Software cuja finalidade é encontrar (através de varreduras) e remover spywares.

Comentários:

(a) Errado, ele precisa ser explicitamente executado para ser instalado; (b) Errado, essa é a definição de Firewall; (c) Errado, essa é a definição de Spam; (d) Errado, essa é a definição de Sniffer; (e) Correto, spywares realmente são softwares cuja finalidade é fazer varreduras e encontrar e remover spywares.

Gabarito:
Letra E

24. (CETAP / Prefeitura de São João de Pirabas/PA – 2016) Marque a alternativa ERRADA sobre os conceitos de vírus e ameaças virtuais:

a) um email recebido com um arquivo com extensão EXE anexado, que seja executado, é uma forma comum de contrair um vírus, exceto quando recebido de uma pessoa conhecida.

b) um anti-virus é um programa de proteção de computador que encontra e elimina os vírus (programas maliciosos) nele instalados.

c)  adwares  são  programas  maliciosos  que  espionam  os  dados  do  computador  infectado  e exibem propagandas indesejadas.

d)  spywares  são  programas  maliciosos  que  capturam  e  transmitem  dados  do  computador infectado.


e) um anti-spyware é um programa de proteção que detecta e elimina do computador spywares e adwares. Ele também previne que o computador seja infectado.

Comentários:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





116
128





(a) Errado, trata-se de uma forma comum de contrair um vírus mesmo quando recebido de pessoas conhecidas; (b) Correto, ele realmente elimina vírus instalados; (c) Correto, adwares realmente espionam  os  dados  do computador infectado  e  exibem propagandas indesejadas;  (d)  Correto, spywares realmente capturam e transmitem dados do computador infectado; (e) Correto, anti- spyware realmente detecta e elimina do computador spywares e adwares, além de previnir que o computador seja infectado.

Gabarito: Letra A

25. (CETAP / MPCM – 2015) Qual tipo de virus (ou praga eletrônica) pode contaminar os arquivos criados por processadores de texto e planilhas eletrônicas?

a) De arquivos executaveis.
b) De macro
c) Vermes.
d) Keyloggers.

e) Mutante.

Comentários:

O  tipo  de  vírus  capaz  de  infectar  arquivos  criados por  processadores  e  de  texto  e  planilhas eletrônicas são os Vírus de Macro.

Gabarito: Letra B

26. (CETAP / AL-RR – 2010) Atualmente, milhões de cidadãos têm usado a Internet para realização de operações bancárias, compras, dentre outras. Nesse contexto, a segurança da informação na Internet torna-se uma preocupação imprescindível para todos que usam esse meio. Analise os itens seguintes e assinale a alternativa CORRETA com relação aos procedimentos e conceitos de segurança.

I - A realização de operações na Web que envolvem dados sigilosos, como operações bancárias e compras, só devem ser realizadas em sites confiáveis que não necessitam utilizar criptografia de dados;

II - Os vírus são programas de computador maliciosos que podem multiplicar-se copiando a si próprio. Os anti-vírus são softwares importantes que protegem o computador dos ataques dos vírus;

III - Um firewall de uso pessoal é um programa de computador que controla o tráfego de entrada e saída de dados de um computador permitindo ou negando o acesso de acordo com políticas de segurança;
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





117
128





IV - Spywares são programas de computador que coletam informações de um computador sem permissão. Alguns tipos de vírus utilizam spywares para roubar informações confidenciais;

V  -  Os  anexos  de  emails  recebidos  podem  estar  infectados  por  vírus.  Entretanto,  caso  o remetente seja alguém confiável pode-se abrir os anexos sem maiores preocupações.

a) Somente a alternativa I está correta.
b) Somente as alternativas I e IV estão corretas.
c) Somente as alternativas I, II e IV estão corretas.
d) Somente as alternativas II, III e IV estão corretas.

e) Todas as afirmativas estão corretas.

Comentários:

(I) Errado. Na verdade, é ideal que utilize a criptografia de dados; (II) Correto. Vírus realmente podem  se  autocopiar  e  podem  ser  combatidos  por  antivírus;  (III)  Correto.  Firewall  Pessoal realmente  controla  tráfego  de  entrada/saída  de  dados  permitindo/negando  de  acordo  com  a política de segurança da organização; (IV) Correto. Spywares realmente coletam informações sem permissão. Além disso, alguns tipos de vírus podem utilizar spywares para roubar informações confidenciais; (V) Errado. Deve haver preocupação inclusive com e-mails recebidos de pessoas confiáveis (essa pessoa pode ter sido infectada com algum software malicioso).

Gabarito:
Letra D

















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





118
128




LISTA DE QUESTÕES – DIVERSAS BANCAS 
1. (CONSULPLAN  /  TJ-MG  –  2017)  Códigos  maliciosos  (malwares)  são  programas especificamente desenvolvidos para executar ações danosas e atividades maliciosas em um computador.  O  programa  que  permite  o  retorno  de  um invasor  a  um  computador comprometido,  por  meio  da  inclusão  de  serviços  criados  ou  modificados  para  este  fim  é conhecido como:

a) Backdoor.
b) Spyware.
c) Worm.
d) Rootkit.

2. (CONSULPLAN / TRE-MG – 2015) Malware são programas especificamente desenvolvidos para executar ações danosas e atividades maliciosas no computador. O worm é um dos tipos de malware  que  se  propaga  automaticamente  pelas  redes,  enviando  cópias  de  si  mesmo  de computador  para  computador.  Quanto  a  um  ataque  desta  natureza,  assinale  a  alternativa INCORRETA.

a) Faz a inclusão de si mesmo em outros programas ou arquivos.
b) Necessita identificar os computadores-alvo para os quais tentará se copiar.
c) Na propagação pode afetar o desempenho de redes e uso dos computadores.
d) Explora vulnerabilidades existentes em programas instalados no computador-alvo.

3. (COPESE / DPE-TO – 2015) Defacers são os pichadores virtuais especializados em desfigurar páginas de sites na Internet.

4. (UFPEL / UFPEL – 2013) Um software malicioso é um software intencionalmente incluído ou inserido em um sistema para um propósito prejudicial. Nesse contexto, analise as informações relacionadas aos vírus de computador.

I - Um vírus pode estar anexado a um programa de computador.

II  -  Uma  maneira  de  se  prevenir,  detectar  e  eliminar  um  vírus  é  através  de  um  programa denominado de WinZip.

III - A infecção de um vírus pode se propagar de um computador para outro, mesmo que ambos estejam desligados.

Está(ão) correta(s):

a) apenas I.
b) apenas II.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





119
128




c) apenas III.
d) apenas I e II.
e) apenas II e III.

5. (OBJETIVA / Prefeitura de Terra de Areia/RS – 2016) Segundo a Cartilha de Segurança para Internet, alguns sistemas operacionais permitem que o usuário compartilhe com outros usuários recursos do seu computador, como diretórios, discos e impressoras. Com base nisso, em relação às formas de prevenção, assinalar a alternativa INCORRETA:

a) Estabelecer senhas para os compartilhamentos.
b) Compartilhar os recursos pelo tempo mínimo necessário.
c) Ter um antimalware instalado no computador, mantê-lo atualizado e utilizá-lo para verificar qualquer arquivo compartilhado.
d)  Estabelecer  permissões  de  acesso  inadequadas,  permitindo  que  usuários  do compartilhamento tenham mais acessos que o necessário.
e) Manter o computador protegido, com as versões mais recentes e com todas as atualizações aplicadas.

6. (OBJETIVA / Prefeitura de Porto Barreiro/PR – 2016) Em conformidade com a Cartilha de Segurança para Internet, sobre a segurança em conexões web, analisar os itens abaixo:

I - O protocolo HTTP, além de não oferecer criptografia, também não garante que os dados não possam ser interceptados, coletados, modificados ou retransmitidos, nem que o usuário esteja se comunicando exatamente com o site desejado. Por essas características, ele não é indicado para transmissões que envolvem informações sigilosas, como senhas, números de cartão de crédito e dados bancários, e deve ser substituído pelo HTTPS, que oferece conexões seguras.

II - O protocolo HTTPS utiliza certificados digitais para assegurar a identidade, tanto do site de destino quanto a sua própria, caso o usuário possua um. Também utiliza métodos criptográficos e outros protocolos, como o SSL (Secure Sockets Layer) e o TLS (Transport Layer Security), para assegurar a confidencialidade e a integridade das informações.

a) Os itens I e II estão corretos.
b) Somente o item I está correto.
c) Somente o item II está correto.
d) Os itens I e II estão incorretos.

7. (OBJETIVA  /  Prefeitura  de  Tramandaí/RS  –  2015) Em  conformidade  com  a  Cartilha  de Segurança para Internet, em relação aos cuidados a serem tomados ao aceitar um certificado digital, marcar C para as afirmativas Certas, E para as Erradas e, após, assinalar a alternativa que apresenta a sequência CORRETA:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





120
128




( ) Manter o sistema operacional e navegadores web atualizados (além disso contribuir para a segurança geral do computador, também serve para manter as cadeias de certificados sempre atualizadas).

(  )  Manter  o  computador  com  a  data  correta.  Além  de  outros  benefícios, isso impede que certificados válidos sejam considerados não confiáveis e, de forma contrária, que certificados não confiáveis sejam considerados válidos.

( ) Ao acessar um site web, observar os símbolos indicativos de conexão segura e ler com atenção eventuais alertas exibidos pelo navegador.

a) C - C - C.
b) C - E - C.
c) E - C - E.
d) E - E - E.

8. (OBJETIVA / Prefeitura de Agudo/RS – 2015) Segundo a Cartilha de Segurança para Internet, falsificação de e-mail é uma técnica que consiste em alterar campos do cabeçalho de um e-mail, de forma a aparentar que ele foi enviado de uma determinada origem quando, na verdade, foi enviado de outra. Exemplos de e-mails com campos falsificados são aqueles recebidos como sendo:

I - De alguém conhecido, solicitando que o usuário clique em um link ou execute um arquivo anexo.

II - Do banco do usuário, solicitando que ele siga um link fornecido na própria mensagem e informe dados da sua conta bancária.

III - Do administrador do serviço de e-mail que o usuário utiliza, solicitando informações pessoais e ameaçando bloquear a sua conta caso o usuário não as envie.

Estão CORRETOS:

a) Somente os itens I e II.
b) Somente os itens I e III.
c) Somente os itens II e III.
d) Todos os itens.

9. (OBJETIVA / Prefeitura de Chapecó/SC – 2011) Assinalar a alternativa que preenche a lacuna abaixo CORRETAMENTE:

Os _______ são e-mails não solicitados, que geralmente são enviados para um grande número de  pessoas.  Quando  o  conteúdo  é  exclusivamente  comercial,  esse  tipo  de  mensagem  é denominado UCE (do inglês Unsolicited Commercial E-mail).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





121
128





a) vírus
b) spams
c) Cavalos de Troia
d) trojans

10. (PUC-PR / TJ-MS – 2015) A respeito de segurança da informação, é CORRETO afirmar que um Worm é:

a) um programa ou parte de um programa de computador que se propaga por meio de cópias de si mesmo, infectando outros programas e arquivos de computador. O Worm depende da execução do programa ou do hospedeiro para ser ativado.

b) um programa que procura dar a garantia de retorno a um computador invadido, sem utilizar novas técnicas de invasão, ou que retorna ao computador invadido sem ser notado.

c) um software espião que tem como objetivo monitorar atividades de um sistema e enviar as informações coletadas para terceiros.

d) um tipo de software projetado para apresentar propagandas, seja por meio de um navegador (browser), seja com algum outro programa instalado em um computador.

e) um programa capaz de se propagar automaticamente através de redes, enviando cópias de si mesmo de computador para computador. Difere do vírus por não embutir cópias de si mesmo em outros programas ou arquivos.

11. (PUC-PR  /  TCE-MS  –  2013) De  modo  geral,  são  considerados  como  malware  softwares destinados a se infiltrar em um sistema de computador alheio de forma ilícita, com intuito de causar algum dano ou roubo de informação. Vírus de computador, worms, trojans e spywares são variações de malwares, cada qual com comportamentos e objetivos distintos. Um malware é classificado como worm quando possui a característica de:

a) apenas se propagar quando executado por um usuário, vindo de arquivo anexo em e-mail ou mensagens em redes sociais.

b) se propagar de computador para computador sozinho, sem ter que se anexar a algo ou alguma coisa.

c) se esconder dentro de outros softwares, para ser acionado inadvertidamente pelo usuário.

d) inundar sites de internet com requisições de informação e solicitação de serviços, para que fiquem lentos ou caiam.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





122
128




e) monitorar os dados que trafegam em uma rede, podendo capturar senhas e informações confidenciais.

12. (IDIB / CRF-RJ – 2018) Acerca dos tipos de vírus, analise as seguintes afirmativas.

I. Os vírus de arquivos infectam arquivos de programas e arquivos criados por usuários.

II. Os vírus de macro são vírus que tem seu código fonte (linhas de comando) criptografado, ou seja, os caracteres da programação são alterados para outros caracteres.

III. Os vírus de boot infectam os arquivos de inicialização do sistema, escondendo-se no primeiro setor do disco e são carregados na memória antes do sistema operacional.

De acordo com as afirmativas acima, marque a alternativa correta.

a) Apenas a afirmativa I está correta.
b) Apenas as afirmativas I e II estão corretas.
c) Apenas as afirmativas I e III estão corretas.
d) Apenas as afirmativas II e III estão corretas.

13. (IDIB / CRF RJ – 2018) Considerando que arquivos de computadores podem ser infectados por vírus ou serem portadores deles, marque a alternativa com o tipo de arquivo que NÃO pode ser infectado ou propagado por eles.

a) .doc
b) .docx
c) .txt
d) .xls

14. (FADESP  /  BANPARÁ  –  2018) Sobre  os  conceitos  de  segurança,  vírus  e  ataques  a computadores, analise as seguintes afirmativas:

I.  A  criptografia  assimétrica  utiliza  uma  chave  única,  que  é  usada  para  cifrar  e  decifrar mensagens. Já a criptografia simétrica emprega um par de chaves, sendo uma privada e uma pública, que são usadas para cifrar e decifrar as mensagens, respectivamente.

II.  Engenharia  social  é  o  termo  usado  para  designar  práticas  utilizadas  a  fim  de  se  obter informações  sigilosas  ou  importantes  de  empresas,  usuários  e  sistemas  de  informação, explorando a confiança das pessoas para enganá-las.

III. São conhecidos como spammers os responsáveis pelo envio de diversas mensagens não solicitadas  para  muitos  usuários.  No  entanto,  o  termo spam  é  empregado  apenas  para  as mensagens  enviadas  por  meio  de  um  correio  eletrônico,  não  envolvendo,  portanto,  as mensagens veiculadas em outros meios como blogs, fóruns e redes sociais.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





123
128





Está(ão) correto(s) o(s) item(ns):

a) II.
b) III.
c) I e II.
d) II e III.
e) I, II e III.

15. (FADESP / BANPARÁ – 2018) Sobre segurança no acesso à Internet, analise as afirmativas a seguir.

I. Phishing é uma prática utilizada para coletar informações pessoais, como senhas e número de contas bancárias. Uma tentativa de phishing pode acontecer através do contato do usuário com páginas Web construídas para imitar sites de bancos e outras instituições.

II. O ataque do homem–do–meio refere–se à forma de ataque em que uma comunicação entre duas  pessoas  é  interceptada  por  uma  terceira.  O  atacante  simplesmente  recebe  e, opcionalmente,  repassa  as  informações  do  transmissor  para  o  receptor,  sem  que  ambos percebam que a comunicação não está sendo, de fato, direta.

III. Ransomware é um software malicioso que bloqueia o acesso do usuário aos arquivos do computador. Os criminosos exigem alguma forma de recompensa mediante a promessa de que o acesso aos dados será restabelecido.

Com base na análise realizada, é correto afirmar que 
a) somente a afirmativa I é verdadeira.
b) somente a afirmativa II é verdadeira.
c) somente as afirmativas I e III são verdadeiras.
d) somente as afirmativas II e III são verdadeiras.
e) todas as afirmativas são verdadeiras.

16. (IBADE / PREVES – 2017) Em se tratando de vírus de computador, classificam-se as fases de execução de um vírus em 4 fases distintas. A fase em que o vírus está se replicando, infectando novos arquivos em outros sistemas é conhecida como a fase de:

a) ação.
b) carga.
c) ativação.
d) propagação.
e) dormência.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





124
128




17. (IBADE / IPERON – 2017) Um usuário precisa instalar em seu microcomputador um software antivírus de mercado, para se prevenir de ataques. Um software dessa categoria é o:

a) Adware.
b) Broadsheet.
c) Kaspersky.
d) Media Player.
e) Switcher.

18. (IBADE / PM AC – 2017) Para manter um computador livre de vírus, o procedimento mais recomendado é:

a) desfragmentar o disco rígido semanalmente.
b) instalar e rodar um software de localização.
c) Instalar e rodar um antivírus.
d) varrer o disco removível antes de usá-lo.
e) fazer uma cópia física de segurança do disco removível.

19. (CETAP  /  Prefeitura  de  Ananindeua-PA  –  2019) Os  vírus  são  softwares  que  prejudicam  o computador, fazendo com que o mesmo fique lento ou até mesmo pare de funcionar. É exemplo de vírus:

a) Mcafee.
b) AVG.
c) Norton.
d) Chameleon.

20. (CETAP / Prefeitura de Ananindeua-PA – 2019) Firewall é uma solução de segurança baseada em hardware ou software (mais comum), onde sua função é:

a) separar os e-mails desejados dos indesejados (spams).
b) alertar o usuário quando há um problema no teclado.
c) alertar o usuário que há uma nova atualização do Word2010.
d) Controlar a movimentação de todos os dados do computador através da internet. Prevenir o vazamento de informações do computador para a internet, fazendo o bloqueio de acesso de softwares maliciosos que podem prejudicar o computador.

21. (CETAP / Prefeitura de Barcarena-PA – 2016) No contexto da segurança da informação, existe um sistema que é usado para prevenir o acesso não autorizado de usuários da Internet a uma rede  privada  (intranet).  Esse  sistema  pode  ser  implementado  em  hardware,  software  ou combinação de ambos. As mensagens que entram e saem da intranet devem passar por esse sistema que aplica suas políticas de segurança para permitir ou não a transmissão das mesmas.
Esse sistema é denominado:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





125
128




a) Antispyware.
b) Firewall
c) Cavalo de tróia.
d) Antivírus.

e) Adware.

22. (CETAP / Prefeitura de São Miguel do Guamá/PA – 2016) A Segurança da Informação é a área da  Tecnologia  da  Informação  responsável  por  proteger  a  informação  contra  acessos  não autorizados, de modo a preservar seu valor. Analise as afirmativas seguintes sobre Segurança da Informação e assinale a alternativa correta:

I - Firewalls são programas de computador utilizados para prevenir, detectar e eliminar vírus de computador.

II - Spywares são programas maliciosos cujo objetivo é monitorar as atividades do usuário no computador e enviar as informações coletadas para terceiros através da Internet.

III - Vírus de computador são programas maliciosos capazes de infectar programas e arquivos do computador, podem fazer cópias de si mesmo e espalhar-se para outros computadores em rede.

IV - Cavalo de Tróia (Trojan Horse) são programas maliciosos que abrem portas no computador para possíveis ataques.

V - Anti-vírus são programas de computador que tem como objetivo proteger o computador ou uma rede de computadores, liberando ou bloqueando o tráfego de dados entre o computador e a rede externa de acordo com regras estabelecidas.

a) Todas as afirmativas estão corretas.
b) Somente as afirmativas I, II e III estão corretas.
c) Somente as afirmativas III e V estão corretas.
d) Somente as afirmativas II, III e IV estão corretas.

e) Somente as afirmativas I e V estão corretas.

23. (CETAP  Prefeitura  de  Abaetetuba/PA  –  2016) No  contexto  de  segurança  da  informação, marque a alternativa que apresenta a definição correta de anti-spyware:

a)  Software  que  se  auto  instala  no  computador,  monitora  a  atividade  do  usuário  e, periodicamente, reporta suas atividades para outro computador na Internet.

b) É uma barreira de software ou hardware entre um ou mais computadores e a Internet.

c) Propaganda não desejada recebida por email.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





126
128




d)  Software  que  executa  no  servidor  e  fica  posicionado  entre  as  estações  de  trabalho  dos usuários e a Internet. São usados nas organizações para prover mais controle administrativo, serviço de caching, monitoramente e registro das atividades da rede.


e) Software cuja finalidade é encontrar (através de varreduras) e remover spywares.

24. (CETAP / Prefeitura de São João de Pirabas/PA – 2016) Marque a alternativa ERRADA sobre os conceitos de vírus e ameaças virtuais:

a) um email recebido com um arquivo com extensão EXE anexado, que seja executado, é uma forma comum de contrair um vírus, exceto quando recebido de uma pessoa conhecida.

b) um anti-virus é um programa de proteção de computador que encontra e elimina os vírus (programas maliciosos) nele instalados.

c)  adwares  são  programas  maliciosos  que  espionam  os  dados  do  computador  infectado  e exibem propagandas indesejadas.

d)  spywares  são  programas  maliciosos  que  capturam  e  transmitem  dados  do  computador infectado.


e) um anti-spyware é um programa de proteção que detecta e elimina do computador spywares e adwares. Ele também previne que o computador seja infectado.

25. (CETAP / MPCM – 2015) Qual tipo de virus (ou praga eletrônica) pode contaminar os arquivos criados por processadores de texto e planilhas eletrônicas?

a) De arquivos executaveis.
b) De macro
c) Vermes.
d) Keyloggers.

e) Mutante.

26. (CETAP / AL-RR – 2010) Atualmente, milhões de cidadãos têm usado a Internet para realização de operações bancárias, compras, dentre outras. Nesse contexto, a segurança da informação na Internet torna-se uma preocupação imprescindível para todos que usam esse meio. Analise os itens seguintes e assinale a alternativa CORRETA com relação aos procedimentos e conceitos de segurança.

I - A realização de operações na Web que envolvem dados sigilosos, como operações bancárias e compras, só devem ser realizadas em sites confiáveis que não necessitam utilizar criptografia de dados;

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





127
128




II - Os vírus são programas de computador maliciosos que podem multiplicar-se copiando a si próprio. Os anti-vírus são softwares importantes que protegem o computador dos ataques dos vírus;

III - Um firewall de uso pessoal é um programa de computador que controla o tráfego de entrada e saída de dados de um computador permitindo ou negando o acesso de acordo com políticas de segurança;

IV - Spywares são programas de computador que coletam informações de um computador sem permissão. Alguns tipos de vírus utilizam spywares para roubar informações confidenciais;

V  -  Os  anexos  de  emails  recebidos  podem  estar  infectados  por  vírus.  Entretanto,  caso  o remetente seja alguém confiável pode-se abrir os anexos sem maiores preocupações.

a) Somente a alternativa I está correta.
b) Somente as alternativas I e IV estão corretas.
c) Somente as alternativas I, II e IV estão corretas.
d) Somente as alternativas II, III e IV estão corretas.

e) Todas as afirmativas estão corretas.






















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





128
128




GABARITO
1. LETRA A
2. LETRA A
3. CORRETO
4. LETRA A
5. LETRA D
6. LETRA A
7. LETRA A
8. LETRA D
9. LETRA B
10. LETRA E
11. LETRA B
12. LETRA C
13. LETRA C
14. LETRA A
15. LETRA E
16. LETRA D
17. LETRA C
18. LETRA C
19. LETRA D
20. LETRA D
21. LETRA B
22. LETRA D
23. LETRA E
24. LETRA A
25. LETRA B
26. LETRA D











Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 06
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 