

Livro Eletrônico
Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti 06315057411 - EVA CELESTE DE SOUZA 






1
105
Sumário
Protocolos de Comunicação ..................................................................................................................... 3 1 – Conceitos Básicos ............................................................................................................................ 3 2 – Modelo OSI/ISO ............................................................................................................................... 5 3 - Arquitetura TCP/IP .......................................................................................................................... 13 4 – Principais Protocolos ...................................................................................................................... 15 4.1 – Protocolos da Camada de Rede ............................................................................................ 15 4.2 - Protocolos da Camada de Transporte ................................................................................... 27 4.3 – Protocolos da Camada de Aplicação .................................................................................... 33 Resumo ..................................................................................................................................................... 55 Mapa Mental ............................................................................................................................................ 58 Questões Comentadas – BANCAS DIVERSAS ..................................................................................... 60 Lista de Questões - BANCAS DIVERSAS ............................................................................................... 89 Gabarito - BANCAS DIVERSAS ............................................................................................................ 105 







Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






2
105
APRESENTAÇÃO DA AULA Fala, galera! O assunto da nossa aula de hoje é Protocolos de Comunicação! Pessoal, não há como se  falar  em  redes  de computadores como  a  internet  sem  falar  sobre  protocolos  de  comunicação.
Para utilizar a Internet, você precisará dos protocolos IP, TCP ou UDP; para utilizar um navegador, você precisará dos protocolos HTTP, HTTPS e DNS; para enviar/receber e-mail, você precisará dos protocolos SMTP, POP3 ou IMAP; e assim por diante...

PROFESSOR DIEGO CARVALHO - www.instagram.com/professordiegocarvalho 
Galera, todos os tópicos da aula possuem Faixas de Incidência, que indicam se o assunto cai muito ou pouco em prova. Diego, se cai pouco para que colocar em aula? Cair pouco não significa que não cairá justamente na sua prova! A ideia aqui é: se você está com pouco tempo e precisa ver somente aquilo que cai mais, você pode filtrar pelas incidências média, alta e altíssima; se você tem tempo sobrando e quer ver tudo, vejam também as incidências baixas e baixíssimas. Fechado?

INCIDÊNCIA EM PROVA: baixíssima 
INCIDÊNCIA EM PROVA: baixa 
INCIDÊNCIA EM PROVA: média 
INCIDÊNCIA EM PROVA: ALTA 
INCIDÊNCIA EM PROVA: Altíssima 

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






3
105
PROTOCOLOS DE COMUNICAÇÃO 1 – Conceitos Básicos INCIDÊNCIA EM PROVA: baixa 
Existe  um  renomado  autor  – chamado  Andrew  Tanenbaum  –  que  afirma  que  “um protocolo é um acordo entre as partes que se comunicam, estabelecendo como se dará a comunicação”. Outro grande autor  –  chamado  Behrouz  Forouzan  –  declara  que  um  “protocolo  é  um  conjunto  de  regras  que controlam a comunicação de dados”.
Já esse que vos escreve – chamado Diego Carvalho – gosta de pensar em protocolos simplesmente como um idioma.

Nós sabemos que um idioma é um conjunto de padrões que permitem a comunicação entre duas  ou  mais  pessoas!  Ora,  eu  falo  português  e  você  também,  logo  nós  nos  entendemos perfeitamente porque ambos usamos o mesmo protocolo de comunicação. Se você só fala russo, infelizmente  nós  não  vamos  nos  entender,  porque  nós  seguimos  protocolo,  regras,  normas diferentes de comunicação. No mundo dos computadores, isso também acontece!

Uma  máquina  só  consegue  se  comunicar  com  outra  máquina  se  ambas  utilizarem  o  mesmo protocolo de comunicação, ou seja, seguirem as mesmas regras ou normas pré-definidas. Então, a partir  de  agora  nós  já  podemos  definir  um  protocolo  de  comunicação  como um  conjunto  de padrões que permite a comunicação entre equipamentos de uma rede .  Da  mesma  forma  que existem centenas de idiomas no mundo, existem centenas de protocolos de comunicação.

Agora,  imaginem  comigo:  vocês  passaram  no  concurso público  que  vocês  tanto  sonhavam  e decidiram comemorar fazendo um mochilão por 10 países da Europa, sendo que cada um  desses países fala uma língua diferente (Ex: Espanhol, Francês, Holandês, Alemão, etc). Ora, você vai ter que aprender todos esses idiomas? Não! Hoje em dia, a língua mais universal que temos é o inglês.
Logo, se você souber falar inglês, você se vira em todos esses países.

“Os  computadores  e  os  seres  humanos  possuem  uma  característica  comum:  ambos  usam linguagens  complexas  para  se  comunicarem.  Quando  duas  pessoas  que  falam  idiomas diferentes (digamos, francês e japonês) precisam compartilhar informações, elas podem usar um intérprete para traduzir, ou uma terceira língua (como o inglês) que as duas podem entender” – Bill Eager

De  forma  similar,  ocorre  no  mundo  dos  computadores. Hoje  em  dia,  existe  um  conjunto  de protocolos padrão da internet chamado TCP/IP – ele é como o inglês das máquinas! Não importa se é um notebook, um tablet ou um computador, também não importa se utiliza Linux ou Windows ou  se  possui  arquitetura  x86 ou  x64.  Se estiver  conectado  à  Internet, ele  estará  necessariamente utilizando o TCP/IP – independentemente de seu hardware ou software.

Galera, um aluno certa vez me questionou: professor, e se eu quiser utilizar outro protocolo na rede da minha casa, eu não posso? Eu respondi que não havia problema  algum e que ele poderia fazer Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






4
105
isso  quando  quisesse! No  entanto, para  que  a  sua  rede  se  comunicasse  com  a  internet, ela necessariamente deveria utilizar o TCP/IP. Entendido?  Vamos  exemplificar  esses  conceitos  com algumas questões :)

(Governo do Maranhão – 2010) Em uma rede de computadores as regras e convenções utilizadas na “conversação” entre computadores são usualmente chamadas de:

a) Protocolos   b) Topologias c) Arquiteturas d) Drivers e) Links _______________________ Comentários: (a) Correto. vejam as palavras-chave da questão: regras, convenções, conversação entre computadores – só pode estar  falando  de  Protocolos!  (b)  Errado,  topologia é  o  layout,  o  desenho  da  rede;  (c)  Errado,  arquitetura  é  um  conjunto  de camadas  e  protocolos;  (d)  Errado,  drivers  são  softwares  para  instalação  de  equipamentos;  (e)  Errado,  links  são  ligações, conexões (Letra A).

(CISSUL/MG  –  2013) As  regras  e  convenções  usadas  na  comunicação  das  redes  de computadores são conhecidas como:

a) conectores.  b) idiomas.     c) protocolos. d) tradutores.
_______________________ Comentários: conforme  vimos  em  aula,  as  regras  e  convenções  utilizadas  na  comunicação  de  redes  de  computadores  são chamadas de protocolos (Letra C).

(Prefeitura de Belo Horizonte/MG – 2015) Um  _____________  define  as  regras  que  o remetente,  o  destinatário  e  todos  os  demais  dispositivos  devem  seguir  para  que  seja possível a comunicação em uma rede de computadores.

Assinale a alternativa que completa CORRETAMENTE a lacuna.

a) Comutador.  b) Demodulador.      c) Protocolo.  d) Roteador.
_______________________ Comentários: conforme  vimos  em  aula,  um  protocolo  define  as  regras  que  o  remetente,  o  destinatário  e  todos  os  demais dispositivos devem seguir para que seja possível a comunicação em uma rede de computadores (Letra C).

(PRODESP – 2014) Como são chamadas as regras da comunicação entre computadores em uma rede local?

a) Tipos. b) Limites.      c) Postagem.  d) Pilha. e) Protocolos.
_______________________ Comentários: conforme vimos  em aula, as  regras  de  comunicação  entre computadores  em  uma  rede  local  são chamadas  de Protocolos (Letra E).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






5
105
2 – Modelo OSI/ISO
INCIDÊNCIA EM PROVA: média 
Galera, nós já sabemos que uma rede é uma combinação de hardware e software que envia dados de uma localidade para outra. Para que dados possam trafegar de um ponto a outro, é necessário que tanto hardware quanto software realizem algumas tarefas.
Pessoal, vocês já se perguntaram como um e-mail enviado para um amigo que mora do outro lado do mundo consegue chegar até o computador dele? Tudo acontece tão rápido que até parece simples, mas não é!

Falando especificamente do contexto de softwares, a atividade de enviar um e-mail pode ser dividida  em  várias  tarefas,  cada  uma  das  quais  realizada  por  uma  camada  de  software diferente.
Professor,  não  estou  entendendo  bulhufas! Imagem  dois  amigos  se  comunicando  por cartas! O processo de enviar uma carta a um amigo seria complexo se não existisse nenhum serviço disponível das agências dos correios, concordam? Vejamos...



Note  que  temos  na  imagem  anterior  um  remetente,  um destinatário  e  um  transportador  – provavelmente um carteiro. Olhando apenas para o lado do remetente, nós temos três tarefas que podem  ser  divididas  em  camadas;  durante  o  transporte,  a  carta  se  encontra  a  caminho  de  seu destinatário (nesse momento, não nos interessa analisar as tarefas realizadas pelo transporte); por fim, ocorre de forma similar do lado direito, mas em ordem inversa.

De  acordo  com  nossa  análise,  há  três  tarefas  distintas  no  lado  do  remetente  e  outras  três  do destinatário, sendo que elas devem ser realizadas na sequência correta.
Note que cada camada no lado do remetente usa os serviços da camada imediatamente inferior. O remetente na camada mais  alta  utiliza  os  serviços  da  camada  intermediária;  a  camada  intermediária  usa  os  serviços  da camada mais baixa; e a camada mais baixa utiliza os serviços do transportador.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






6
105

Galera, dividir um problema em camadas com tarefas e serviços específicos é uma excelente estratégia para reduzir a complexidade de um problema.
Pois bem... e se eu dissesse para vocês que os engenheiros e cientistas pioneiros no estudo de redes de computadores decidiram utilizar essa mesma  ideia? A  ISO  (International  Standards  Organization)  criou um  modelo  conceitual  para auxiliar a compreender e projetar uma arquitetura de redes de computadores:

Modelo OSI
(Open Systems Interconnection) 

O Modelo OSI é basicamente um modelo de referência para conexão e projetos de sistemas de redes que se baseia em uma arquitetura em camadas. Esse modelo sugere um padrão comum de comunicação  entre  componentes  de  hardware  e  software  envolvidos  em  uma  comunicação.  Em outras palavras, ele diz como os componentes devem interagir para enviar e receber dados um para o outro por meio de uma rede de computadores.



Esse modelo é apenas uma abstração teórica – uma referência conceitual – usado pela comunidade acadêmica para representar o que seria um modelo perfeito de rede com suas respectivas descrições de camadas. Ele tem uma função mais didática do que pragmática.
Não  se  trata  de  da  arquitetura  utilizada  atualmente  em  redes  de  computadores  –  na prática, a arquitetura utilizada atualmente é o TCP/IP.

Nós sabemos que a comunicação entre dois computadores é extremamente complexa, logo esse modelo sugere dividir essa complexidade em uma estrutura de sete camadas distintas, porém relacionadas entre si, cada uma das quais definindo uma parte do processo de transferência de  informações  através  de  uma  rede.  Compreender  esses  conceitos  é  importante  para  entender posteriormente a função de cada protocolo. Vem comigo... é legal! Eu juro...

Na  tabela  seguinte,  nós  veremos  a  função  de  cada  uma  dessas camadas.  Entenda  que  esse  assunto  não  é  muito  relevante  para  a prova  em  si,  uma  vez  que  raramente  cai  alguma  questão.
No
entanto,   eu   considero   interessante   que   vocês   passem rapidamente por cada um desses pontos para que vocês entendam ao fim como cada camada dessas possui uma responsabilidade no envio  e  recebimento  de  dados  entre  um  remetente  e  um destinatário.
Além  disso,  é  possível  mapear  alguns  protocolos  que veremos mais à frente para cada uma dessas camadas apresentadas na imagem ao lado. É isso... Fechado? Então vamos lá...
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA ==12b2d8==







7
105

CAMADA Descrição protocolos APLICAÇÃO
Essa  camada  habilita  o  usuário,  seja  ele  humano  ou software,  a  estabelecer  a comunicação  entre  aplicações  e  a  acessar  a  rede.  Ela  fornece  interface  com  o usuário  e  suporte  a  serviços  como  e-mail,  acesso  e transferência  de  arquivos remotos,  gerenciamento  de  bancos  de  dados  compartilhados  e  outros  tipos  de serviços  de  informação  distribuídos.  Ela  funciona  como  um  portal  em  que  os processos de aplicações possam acessar uma rede.
HTTP, SMTP,
FTP, SSH,
TELNET, IRC,
SNMP, POP3,
IMAP, DNS.
APRESENTAÇÃO
Essa  camada  é  responsável  por  definir  o  formato  para  troca  de  dados  entre computadores,   como   se   fosse   um   tradutor. Como  assim,  professor?   Ela   é responsável  pela  formatação  e  tradução  de  protocolos,  pela  criptografia,  pela compressão  de  dados,  pela  conversão  de  caracteres  e  códigos,  entre  diversas tantas   funcionalidades.   Essa   camada   pega   um   texto   que   está   em   binário (010101101111) e converte para o alfabeto latino, por exemplo.
SSL,
TLS,
XDR.
SESSÃO
Essa  camada  é  responsável  por  permitir  que  duas  ou mais  aplicações  em computadores  diferentes  possam  abrir,  usar  e  fechar  uma  conexão,  chamada sessão.  Ela  gerencia  a  comunicação  para  que,  caso  haja  alguma  interrupção,  ela possa  ser  reiniciada  do  ponto  da  última  marcação  recebida.  Diz-se  que  essa camada controla o diálogo da rede – estabelecendo, mantendo e sincronizando a interação entre sistemas que se comunicam.
NETBIOS

TRANSPORTE
Essa  camada  é  responsável  por  organizar  os  dados  em  segmentos  e  que  eles cheguem  ao  destino  livre  de  erros  (sem  perdas,  sem duplicações  e  na  ordem correta), independentemente do tipo, topologia ou configuração de rede. Para tal, ela fornece uma comunicação fim-a-fim ou ponta-aponta confiável (isto é, o nó de origem   se   comunica   apenas   com   o   nó   de   destino,   sem reconhecer   nós intermediários).
TCP, UDP,
NETBEUI.
REDE
Essa camada é responsável pelo endereçamento, roteamento e entrega de pacotes individuais de dados desde sua origem até o seu destino, provavelmente através de várias redes. Embora a camada de enlace coordene a entrega do pacote entre dois  sistemas  na  mesma  rede,  a  camada  de  rede  garante  que  cada  pacote  seja transmitido de seu ponto de origem até seu destino final.

IP, ICMP, ARP
RARP, NAT.
ENLACE
Essa camada é responsável por organizar os dados em frames (ou quadros) e por estabelecer uma conexão nó a nó1 entre dois dispositivos físicos que compartilham o mesmo meio físico. Ela transforma a camada física, de um meio de transmissão bruto, em um link confiável, fazendo que a camada física pareça livre de erros para a  camada  superior  (camada  de  rede)  e  garantindo  assim  que  os  dados  sejam recebidos corretamente.
ETHERNET,
TOKEN RING,
BLUETOOTH,
WI-FI.
FÍSICA
Essa camada define as especificações elétricas e físicas da conexão de dados. Por exemplo: ela pode dizer como os pinos de um conector estarão posicionados, quais as  tensões  de  operação  de  um  cabo  elétrico,  as  especificações  do  cabo  de  fibra ótica,  a  frequência  dos  dispositivos  sem  fio,  entre  outros.  essa  camada  é totalmente orientada a hardware, não reconhecendo softwares.

USB, DSL.


1
Diferentemente da Camada de Transporte, a Camada de Enlace estabelece uma conexão nó a nó e, não, fim-a-fim.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






8
105
Nós  dissemos  anteriormente  que  o  modelo  divide  a  complexidade  da  comunicação  em  diversas camadas. Então vamos voltar para a nossa historinha de páginas atrás e consolidar tudo que vimos!
A  pergunta  inicial  era: como um e-mail enviado para um amigo que mora do outro lado do mundo consegue chegar até o computador dele? Bem,  no  momento  em  que  um  amigo  clica  no  botão  de enviar e-mail para seu outro amigo, inicia-se um complexo fluxo de dados.

Antes de prosseguir para entender o fluxo completo de dados por um meio de transmissão, vejam a imagem a seguir com um resumo das camadas:



A  primeira  camada  a  receber  o  comando  é  a  camada  de  aplicação.
Essa é a camada que serve como uma janela ou um portal para usuários ou processos acessarem serviços de rede.
Como
assim, professor? Vejam  só:  se  você  deseja  acessar  uma  página  web,  você  pode  usar  o  protocolo HTTP; se você deseja transferir um arquivo, você pode usar o protocolo FTP; e se você deseja enviar um e-mail, você pode usar o protocolo SMTP (esse é o nosso caso!).




Feito isso, os dados passam para a camada de apresentação, que será responsável por reconhecer o  formato  dos  dados  (verificar  se  se  trata  de  uma  mensagem,  uma  página  web,  uma  foto,  uma música, etc) e formatá-los, como uma espécie tradutor. Na prática, ela traduz a mensagem escrita no  alfabeto  latino  para  uma  linguagem  que  a  máquina  reconhece.  Além  disso,  ele  poderá encriptá-la para que ninguém a intercepte e a leia durante o caminho.

A partir daí, passamos para a camada de sessão, em que será estabelecida uma conexão entre a máquina de origem e a máquina de destino que permitirá que nós  troquemos  mensagens  entre  si.  A  Camada  de Sessão    também    será    responsável    guardar    várias informações relevantes para a comunicação (Logging).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






9
105

Beleza!   Agora   que   minha   informação   acessou   um serviço  de  rede  que  foi  reconhecido  na  camada  de apresentação   e   traduzido,   formatado,   encriptado   e passado  para  a  camada  de  sessão  abrir  uma  conexão entre  minha  máquina  e  a  máquina  destino, agora  eu
tenho  que  passar  por  uma  camada  que  cuide  da segurança e da validação da entrega dos dados .

Pessoal, adianta alguma coisa se eu perder metade dos dados no caminho? Não, porque meu amigo não  vai  entender nada  da  mensagem. Adianta eu enviar todos os dados, mas em uma ordem toda bagunçada? Também não, ele continuará sem entender nada da minha mensagem.
A responsável
por fazer uma varredura e garantir que o dado é confiável, íntegro e válido é a Camada de Transporte.

Além disso, notem uma coisa: nós não estamos mais era dos disquetes que cabiam 80kB! Hoje em dia, você pode   enviar   arquivos   enormes   por   e-mail,   por exemplo.  A  rede  não  suporta  dados  tão  grandes  de uma   vez,
portanto  é  necessário  dividi-los  em pequenos  segmentos.   Dados   que   estejam   com algum    tipo    de    problema    serão    destruídos    e retransmitidos pela camada de transporte.

Passamos então para a famosa camada de redes!
Aqui os segmentos serão encapsulados dentro de pacotes, que conterão o endereço lógico de origem e o endereço lógico de destino (também chamado de Endereço IP) . Essa camada também vai determinar a rota que será utilizada baseado nas condições atuais da rede e na prioridade de entrega, isto é, cada nó intermediário do caminho.



Em seguida, passamos para a Camada de Enlace de Dados, em que os pacotes são transformados em frames para redes específicas.
Ela estabelece também uma conexão entre dois nós sobre a Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






10
105
Camada Física, permitindo uma comunicação virtualmente livre de erros entre os nós. Além disso, ele adiciona o endereço físico do nó de origem e do nó de destino (Endereço MAC).



Por fim, chegamos à Camada Física, que transforma os frames em bits e finalmente os envia para a rede. Pode ser por meio daquele cabinho azul do computador, wi-fi, rádio, etc.



A partir daí, ficou fácil! Se  for  em  uma  rede  cabeada,  os  bits  passam  da  placa  de  rede  do  seu computador para o cabo azul, que passa para o seu roteador, que passa para o provedor de internet, que passa para o seu provedor de e-mail, que passa para o provedor de e-mail do seu amigo que passa para o roteador dele, que passa para o cabo azul dele, que passa para a placa de rede dele...
Ufa! Cansaram? 


E, finalmente, nós começamos todo esse processo, porém agora de forma invertida: iniciando na camada física da máquina de destino até chegar à camada de aplicação e o seu amigo clicar Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






11
105
para ler o e-mail que você enviou. Eu falei que ia ser legal, não falei? Galera, claro que eu fiz algumas simplificações nessa explicação, mas não se preocupem porque alguns desses detalhes não serão tema de prova.

Nós já vimos isso em aula, mas não custa repetir! Cada camada chama os dados que ela processo por um nome diferente. Quando estamos na camada física, tratamos de bits; quando estamos na camada de enlace, tratamos de frames ou quadros; quando estamos na camada de rede, tratamos de pacotes; quando estamos na camada de transporte, tratamos de segmentos; e quando estamos nas outras camadas, tratamos de dados. Vejam só:

CAMADA UNIDADE DE DADOS DO PROTOCOLO (DPU) FÍSICA BITS
ENLACE FRAMES/QUADROS REDE PACOTES
TRANSPOTE SEGMENTOS
SESSÃO
DADOS APRESENTAÇÃO
APLICAÇÃO


SWITCH
ACCESS POINT
ROTEADOR
BRIDGE
HUB
PLACA DE REDE
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






12
105
Por  fim,  nós  vimos  na  aula  anterior  os  principais  dispositivos  de  rede. Agora vejam na imagem abaixo  em  que  camada  trabalha  cada  um desses  dispositivos.  Placas  de  Rede  trabalham  na camada  física  (e  também  de  enlace);  Hubs  trabalham na  camada  física;  switches  trabalham  na camada de enlace; Bridges trabalham na camada de enlace; e o roteadores trabalham na camada de rede. Certinho? Para fechar, vamos ver alguns exercícios...
(PC/AL  –  2012) O  modelo  OSI  (Open  Systems  Interconnection),  um  conjunto  de protocolos destinados ao projeto de sistemas de redes, possibilita a comunicação entre todos os tipos de sistemas de computadores.
_______________________ Comentários: conforme vimos  em aula, Modelo OSI  é uma referência conceitual,  uma abstração  teórica  sobre  o  projeto de sistemas  de  redes.  Ele  não  é  um  conjunto  de  protocolos,  apesar  de  ser  possível  encontrar  os  protocolos  correspondentes  à função de cada camada (Errado).

(JUCEPAR/PR – 2016) Os protocolos HTTP, DNS, FTP e Telnet no modelo OSI operam na camada:

a) De Transporte
b) De Aplicação
c) De Link de Dados
d) De Rede
e) De Sessão
_______________________ Comentários: conforme vimos em aula, todos esses protocolos operam na Camada de Aplicação (Letra B).

(TJ/SP – 2012) As arquiteturas em camadas para rede de computadores, como o modelo OSI  (Open  System  Interconnection),  permitem  dividir  a  complexidade  do  sistema  de redes em camadas de atividades e serviços. No modelo OSI, a atividade de roteamento dos pacotes pelas redes é de responsabilidade da camada:

a) 1
b) 2
c) 3
d) 4
e) 5
_______________________ Comentários: conforme vimos em aula, roteamento de pacotes é atividade da camada de redes – 3 (Letra C).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






13
105
3 - Arquitetura TCP/IP INCIDÊNCIA EM PROVA: ALTA 
Nós  acabamos  de  ver  em  detalhes  o  Modelo  OSI  e  descobrimos  que  –  apesar  de  ser  um  modelo conceitual bastante interessante e de facilitar o entendimento da comunicação entre redes – ele é apenas  um  modelo  teórico  utilizado  didaticamente  para  mostrar  o  funcionamento  ideal  da comunicação  de  dados  em  uma  rede  de  computadores.
Ele  não  é  uma  tecnologia,  nem  um conjunto de protocolos, nem um software e, na prática, ele só tem utilidade pedagógica.

Na prática, o que é utilizado é a Arquitetura ou Pilha TCP/IP. Essa arquitetura foi desenvolvida – na verdade  –  antes  do  Modelo  OSI.  Dessa  forma,  as  camadas  que  nós  veremos  a  seguir  não correspondem exatamente àquelas do Modelo OSI. O que é essa Arquitetura TCP/IP, Diego?
Trata-
se de um conjunto de protocolos e camadas para conectar várias redes diferentes de maneira uniforme – é o conjunto padrão de protocolos da Internet.




A quantidade e nome das camadas apresentada acima para a Arquitetura TCP/IP foi baseada na documentação oficial (RFC 1122) . No entanto, alguns autores modelam essa arquitetura com três, quatro ou cinco camadas de nomes bastante diversos. Observem que ela condensa as camadas de  aplicação,  apresentação  e  sessão  na  camada  de  aplicação.  Ademais,  ela  condensa  a  camada física e de enlace na camada de enlace e chama a camada de rede de internet.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






14
105


Eventualmente,  quando  um  servidor  –  uma  máquina  especializada  –  fornece eminentemente os serviços de um protocolo, é comum chamar esse servidor pelo nome do protocolo que ele implementa. Logo, temos que:

 Um servidor que fornece serviços de apresentação de páginas web pode ser chamado de servidor HTTP;
 Um servidor que fornece serviços de envio de e-mails pode  ser chamado de servidor SMTP;
 Um servidor que fornece serviços de tradução de domínios pode ser chamado de servidor DNS;
 Um  servidor  que  fornece  serviços  de  transferência  de  arquivos  pode  ser chamado de servidor FTP.

(Polícia Federal – 2009) Na  tecnologia  TCP/IP,  usada  na  Internet,  um  arquivo,  ao  ser transferido, é transferido inteiro (sem ser dividido em vários pedaços), e transita sempre por uma única rota entre os computadores de origem e de destino, sempre que ocorre uma transmissão.
_______________________ Comentários: conforme  vimos  em  aula,  ele  é  fragmentado  em  pequenos  pacotes  e  transita  por  rotas  diversas  entre  os computadores de origem e destino (Errado).

(TJM/SP  –  2011) Assinale  a  alternativa  que  apresenta  um  protocolo  da  camada  de aplicação do modelo TCP/IP de protocolos de redes de computadores.

a) ARP   b) FTP  c) UDP d) IPSec e) ICMP _______________________ Comentários: (a) Errado. ARP – Rede; (b) Correto. FTP – Aplicação; (c) Errado. UDP – Transporte; (d) Errado. IPSec – Rede; (e) Errado. ICMP – Rede (Letra B).

(TJM/SP  –  2011) Redes  de  computadores  modernas  utilizam  a  pilha  de protocolos TCP/IP para acesso à Internet. Assinale a opção em que os protocolos apresentados são todos da camada de aplicação do TCP/IP.

a) TCP e IMAP
b) UDP e SMTP
c) IMAP e SMTP
d) UDP e SNMP
e) IP e SNMP
_______________________ Comentários: conforme vimos em aula, TCP e UDP – Transporte; IP – Rede; IMAP e SMTP – Aplicação (Letra C).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






15
105
4 – Principais Protocolos 


4.1 – Protocolos da Camada de Rede 
4.1.1 – IP (INTERNET PROTOCOL) INCIDÊNCIA EM PROVA: Altíssima 
Vamos  explicar  esse  protocolo  com  várias  analogias para  que  vocês  consigam  compreender. O significa essa sigla? Significa Internet Protocol ou Protocolo de Internet. Vamos traduzir também Internet? Inter significa entre e net significa rede, logo Internet significa entre redes. Agora vamos juntar  tudo  isso  e  dar  um  significado!  IP  é  um  protocolo  –  um  conjunto  de  normas,  padrões  e convenções – para comunicação entre redes. Opa... já começou a ficar mais claro!

Pode-se  afirmar  que  IP  é  o  protocolo  de  distribuição  de  pacotes  não  confiável,  de  melhor esforço e sem conexão, que forma a base da internet.
O que significam esses conceitos?

Galera,  se  nós  fôssemos  fazer  uma  analogia,  o  IP  seria  como  o motorista dos Correios.
Ele é aquele cara que já dirigiu pelo Brasil inteiro e conhece as melhores rodovias e rotas para entregar os pacotes aos seus destinatários. Esse  cara  é  muito  gente  fina  e  vai tentar   fazer   o   máximo   possível   para   realizar   a   entrega,   mas infelizmente ele não consegue garantir que ela ocorrerá.

Imaginem que futuramente ocorra uma outra greve dos caminhoneiros! Pode acontecer de o nosso motorista  (IP)  tentar  passar  por  uma  rota,  mas  ela estar  bloqueada.  Pode  ser  que  ele tente  outra Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






16
105
rota, mas ela também pode estar bloqueada. Nesse caso, ele infelizmente pode atrasar a entrega dos pacotes! Pode acontecer pior que isso: imagine que o caminhão seja assaltado e ladrões levem todos os pacotes. Nesse caso, ele também não conseguirá entregar os pacotes!

Dessa forma, por mais que ele se esforce (e ele é esforçado), ele não é capaz de garantir que a entrega será realizada. Por conta disso, ele é um protocolo não confiável, mas é de melhor esforço (best-effort).
E por que ele é um protocolo sem conexão? Esse  eu  vou  explicar  no  próximo tópico, quando estivermos falando sobre o TCP! Vamos continuar... antigamente, para enviar uma informação a outra pessoa, eu utilizava o serviço de correspondências.

Eu  pegava  um  pedaço  de  papel,  escrevia  diversas  informações,  colocava  dentro  de  um  envelope com endereço de origem e endereço de destino. Na internet, ocorre de maneira bastante similar:
as informações que eu desejo transmitir são encapsuladas dentro de um envelope chamado Pacote IP
que contém necessariamente um endereço IP de origem e um endereço IP de destino.
Além disso, eu posso colocar outras informações acessórias no meu envelope (pacote IP)!

Eu  posso  carimbar  esse  envelope  como  confidencial; posso  informar  o  tipo  de  conteúdo  do envelope  (arquivo,  e-mail,  áudio,  etc). Dessa forma, o pacote IP é formado por dados que eu queira enviar e por um cabeçalho contendo informações técnicas que facilitam a entrega. Agora uma pergunta: eu posso enviar um processo com 50.000 páginas pelos Correios? Posso! No entanto, os Correios não vão conseguir colocar 50.000 páginas dentro de um único envelope!

Os  Correios  impõem  um  tamanho  limite  para  o  pacote que  ele  é capaz  de  transportar,  da  mesma  forma  que  existe  um tamanho limite para o pacote IP. E qual é o tamanho, Diego?
Esse limite é de
64 Kb! Caraca, professor... por que tão pequeno? Galera,  quando  a internet foi criada, isso era uma quantidade absurda de informação.
Vejam  essa  imagem  ao  lado:  isso  é  um  HD  de  1960  capaz  de armazenar estrondosos 5 Mb de informação. Incrível, não? Claro que não  é  mais  assim  hoje  em  dia.  Uma  foto  tirada  pelo celular  possui cerca de 6.4 Mb (= 6400 Kb). E se eu quiser enviar essa foto para outra pessoa, caberá tudo em um pacote?  Jamais!
O IP terá que dividir a foto em pacotes de 64 Kb . Como 6400 Kb dividido por 64 Kb é 100, teremos que dividir a foto em 100 pacotinhos e enviá-los um a um.

O  endereço  IP  define  de  forma  única  e  universal  a  conexão  de  um  dispositivo  (Ex:  um computador  ou  um  roteador).  Eles  são  exclusivos  no sentido  de  que  cada  endereço  define  uma única conexão com a Internet – dois dispositivos jamais podem ter o mesmo endereço ao mesmo tempo. Além disso, eles são universais no sentido de que o sistema de endereçamento tem de ser aceito por qualquer host que queira se conectar à Internet.

Esses são – portanto – os fundamentos básicos desse protocolo. Agora vamos falar um pouquinho sobre  endereçamento  e  versões.  Pessoal,  nós  dissemos  várias  vezes  durante  a  aula  que  os computadores de uma rede possuem um endereço lógico chamado Endereço IP.
Da mesma forma
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






17
105
que um carteiro precisa saber o CEP de uma casa, o protocolo IP precisa saber o endereço IP de uma máquina para entregar os dados destinados a ela.

E como é esse endereço? Galera, há duas notações predominantes de endereço IP:
Octetos Binários
ou Decimal Pontuada. Antes de prosseguir, vamos falar um pouco sobre numeração:



Existem  diversos  sistemas  de  numeração!  Seres  humanos  utilizam  um  sistema  de numeração decimal, isto é, nós fazemos contas utilizando dez dígitos (0, 1, 2, 3, 4, 5, 6, 7, 8 e 9). Já os computadores utilizam um sistema de numeração binária, isto é, eles fazem contas utilizando apenas dois dígitos (0 e 1) – o nome desse dígito binário é Bit (do inglês, Binary  Digit).  É  possível  converter  números  de  um  sistema  para  outro  sem  nenhum inconveniente. Vejam abaixo o número 123 em outros sistemas numéricos:




Ele basicamente possui 32 bits de comprimento (Versão 4). Esses 32 bits geralmente são divididos em 4 octetos. O que é um octeto, Diego? É um conjunto de 8 bits ou 1 byte!

Endereço Ip com notação de octetos binários 10101010 01010101 11100111 10111101 
Galera, usar endereço em bits pode acabar incorrendo em erros. Como só tem 0 e 1, se você tem miopia, pode acabar errando. Puxado, concordam?
Pois é, mas alguém teve a brilhante ideia de converter esses números do sistema binário para o sistema decimal. Dessa forma, cada octeto em  binário  pode  ir  de  0  a  255  em  decimal  –  você  nunca  vai  encontrar  um número  que não  esteja nessa extensão. Se convertermos os números da tabela acima para decimal, fica assim:

Endereço IP com NOTAÇÃO DECIMAl pontuada 170 . 85 . 231 . 189 
(PC/SP – 2017) Assinale a sequência numérica abaixo que pode representar o Endereço IP (Internet Protocol) válido de um microcomputador em uma rede:

a) 10.260.25.200
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






18
105
b) 10.35.29.129
c) 10.0.40.290
d) 10.0.290.129
e) 10.35.260.290
_______________________ Comentários: conforme vimos em aula, ele varia de 0 a 255. O octeto binário 00000000 é 0 em decimal e o octeto binário 11111111 é 255 em decimal. (a) Errado, 260 > 255; (b) Correto; (c) 290 > 255; (d) 290 > 255; (e) 260 e 290 > 255 (Letra B).

Professor, está tudo muito abstrato! Você pode dar um exemplo? Claro! Para tal, eu vou propor um exercício para vocês: eu quero que vocês pressionem simultaneamente as teclas Windows + R.



Quando  vocês  fizerem  isso,  aparecerá  essa  imagem  da  esquerda.  Eu  quero,  então,  que  vocês escrevam o comando
cmd conforme vemos na imagem da direita.



Notem  que  será  exibida  essa  janela  da  esquerda.  Em seguida,  eu  quero  que  vocês  escrevam  o comando
ipconfig conforme vemos na janela da direita. No meu caso, foi exibido:


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






19
105

Eu destaquei em branco uma informação importante. O que, professor? Esse é o meu Endereço IPv4:
192.168.0.17! Logo, se alguém quiser me encontrar, esse é o endereço lógico do meu computador na Internet. Agora tem um porém... o meu endereço IP não é fixo! Como assim, Diego? Pois é...
cada vez que eu me conecto à internet, é atribuído um novo endereço IP a minha máquina. No meu caso, eu possuo um IP dinâmico! Não entendi bulhufas...

Na Internet, você pode ter dois tipos de endereço IP:
estático ou dinâmico. O primeiro, também chamado de fixo, é um endereço que não muda – ele é bem pouco utilizado, sendo mais comuns em  máquinas  servidoras  do  que  em  máquinas  clientes (Ex:  IP  do  Estratégia  Concursos).  Já  o segundo   é   um   endereço   que   é  modificado   a   cada   conexão   –   ele   é   bem   mais   utilizado, principalmente em redes domésticas como em uma casa ou em um escritório.

Além  disso,  é  importante  entender  que esses endereços não são aleatórios  –  existem  diversas regras que devem ser obedecidas para cada endereço. Uma delas é o endereçamento com classes.
O que é isso, Diego? Galera, nós já vimos quem um endereço IP (Versão 4) possui 32 bits e já sabemos que  um  bit  só  pode  ter  dois  valores  (0  ou  1). Logo,  existem  quantos endereços  possíveis? 232  ou 4.294.967.296 possibilidades.

Diante de tantos números, foram criadas diversas regras para realizar o endereçamento de um IP. Uma delas busca dividir o espaço de endereços possível em cinco classes: A, B, C, D e E. Logo, todo e qualquer IP do universo pode ser classificado em uma dessas cinco classes. E como eu faço para descobrir, professor? É extremamente simples: basta analisar o primeiro número (na notação decimal pontuada). Eles seguem a seguinte tabela:

1º octeto CLASSE UTILIZAÇÃO 1 A 126 A Inicialmente destindo a grandes organizações.
128 A 191 B Inicialmente destindo a organizações de médio porte.
192 A 223 C Inicialmente destindo a pequenas organizações.
224 A 239 D Inicialmente destindo a reservado para multicast.
240 A 255 E Inicialmente destindo a reservado para testes.

Como interpreta essa tabela? Muito fácil! Se o primeiro número de um endereço IP for de 1 a 126, ele será da Classe A – geralmente utilizado por grandes organizações; se for de 128 a 191, ele será da Classe  B  –  geralmente  utilizado  por  organizações  de  médio  porte;  se  for  e  192  a  223,  ele será  da Classe C – geralmente utilizado por pequenas organizações; se for de 224 a 239, será da Classe D – reservado para multicast; e se for de 240 a 254, será da Classe E – reservado para testes.

Galera,  as  falhas  no  método  de  endereçamento  com  classes  combinada  com  o  imenso crescimento da Internet levaram ao rápido esgotamento dos endereços disponíveis.  Ficamos sem  endereços  de  classe  A  e  B,  e  um  bloco  de  classe  C  é  muito  pequeno  para  a  maioria  das organizações  de  porte  médio.  Esse  método  está  obsoleto  atualmente,  mas  ainda  cai  em  prova.
Agora eu preciso fazer uma confissão...
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






20
105



Eu preciso confessar: o endereço IP mostrado algumas páginas atrás não é meu IP real! Como assim, professor? Galera, todo dispositivo na internet necessita de um endereço IP único – não pode existir dois dispositivos com o mesmo IP !  No  entanto,  com  o  passar  dos  anos  a  quantidade  de dispositivos  conectados  à  internet  subiu  assustadoramente.  Na  minha  casa,  eu  tenho  um computador, minha esposa tem outro, nós temos um notebook e um tablet.

Além disso, temos o meu celular e o celular dela – todos com acesso à Internet! Por baixo, existe apenas na minha casa seis dispositivos conectados. Seguindo o que eu falei no parágrafo anterior, eu  preciso  de  seis  endereços  únicos  diferentes  para  os  meus  dispositivos.  Agora  imagine  uma família  com  três  filhos!  Aliás,  agora  imagine  uma  empresa  com  mil  funcionários.  Existem  quatro bilhões de possibilidades de endereço IP, mas somente cerca de metade pode ser usada.

Ora, como eu faço se existem dois bilhões de endereços úteis e nosso planeta tem uma população de sete bilhões de habitantes? E se considerarmos que cada habitante atualmente pode ter três, quatro ou até mais dispositivos conectados à internet? Pessoal, os engenheiros tiveram que quebrar a cabeça para conseguir uma solução para esse problema. E como eles fizeram, Diego? Cara, eles fizeram de uma maneira genial!

Uma coisa é a rede doméstica privada na sua casa/escritório e outra coisa é a rede mundial de computadores  (Internet).
Por  conta  disso,  foram  padronizadas  faixas  de  endereços  IP  que deveriam ser utilizados exclusivamente para redes privadas, isto é, eles não existem na internet – Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






21
105
eles  só  existem  como  endereços  internos.  Na  tabela a  seguir,  nós  podemos  ver  quais  são  essas faixas de endereços:

Endereços para redes privadas CLASSE A – 10.0.0.0 A 10.255.255.255 (2 24
POSSIBILIDADES)
CLASSE B – 172.16.0.0 A 172.31.255.255 (2 20
POSSIBILIDADES)
CLASSE C – 192.168.0.0 A 192.168.255.255 (2 16
POSSIBILIDADES)

Professor, ainda não entendi por que você disse que mentiu? Pessoal, eu  disse  algumas  páginas  atrás  que  o  meu  IP  era 192.168.0.17.
Façam-me  um  favor: confiram  agora  na  tabela  anterior  se  esse endereço informado está presente em alguma dessas faixas! Ora, está  na  Classe  C!  Logo,  eu  não  menti  exatamente  para  vocês  –  eu apenas  informei  qual  era  o  meu  endereço  IP  dentro  da  minha  rede doméstica – esse endereço é chamado de IP Privado ou Local!

Para  deixar  mais  claro  ainda,  eu  olhei nas  configurações  de  rede  do meu  celular  para  descobrir  qual  era  o  IP  dele:
192.168.0.20. Como
meu celular está conectado na minha wi-fi, ele faz parte da minha rede doméstica, logo esse também é um IP Privado ou Local.
Em
outras palavras, eu possuo seis equipamentos na minha casa e cada um  possui  um  endereço privado  diferente. Qual foi a grande sacada dos engenheiros?

Foi  um  mecanismo chamado  Network  Address  Translation  (NAT).
Ele permite a um usuário ter internamente em sua rede doméstica uma grande quantidade de endereços e, externamente, possuir apenas um endereço (ou um pequeno conjunto de endereços). Qualquer rede doméstica pode utilizar um endereço da nossa tabela sem a necessidade de pedir permissão para provedores de internet. Capiche?

Galera, olha que sacada... a internet chega em uma casa ou organização geralmente por meio de um  modem  ou  um  roteador  que  provavelmente  implementa  o  NAT! O roteador é um dispositivo conectado  à  internet?  Sim,  então  ele  possui  um  IP!
Logo, sempre que um pacote sai da rede privada  para  a  internet  –  passando  por  um  roteador NAT  –  tem  seu  endereço  de  origem substituído pelo endereço do Roteador NAT.



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






22
105
Dessa forma, se eu tiver 10 equipamentos conectados ao mesmo roteador na minha rede local, todos eles apresentarão um único endereço IP público e vários endereços privados.  Vejam  na imagem acima que temos três computadores com endereços IP privados diferentes. No entanto, sempre que qualquer pacote sai dessa rede a partir de qualquer equipamento e acessa a internet, ele sai com um único endereço público:
200.24.5.8.

Professor, há uma maneira de descobrir meu IP público? Sim, basta acessar www.whatismyip.com.
Vejam que esse site informa que meu IP público é: 191.176.124.141.



Pessoal, o NAT é responsável manter uma tabela de endereços de origem e destino de modo que consiga mapear – quando um recurso vem da Internet para a rede privada – para qual máquina da  rede  privada  as  informações  de  fora  devem  ser  enviadas.  Em  suma,  ele  traduz  endereços privados (que existem apenas dentro de redes internas) para endereços públicos (que existem na internet e é utilizada por provedores e servidores de internet).

(TJ/SP – 2012) O uso de um endereço IP real para os computadores de uma rede local é dispendioso  e torna  os  computadores  mais  vulneráveis  aos  ataques  com  o  objetivo  de quebra da segurança. Para minimizar esse problema, pode-se utilizar o esquema de IPs virtuais  para  os  computadores  de  uma  rede  local.  Para  isso,  é  necessário  o  uso  de  um recurso de rede denominado:

a) MIB.   b) NAT. c) DNS. d) DHCP. e) LDAP.
_______________________ Comentários: conforme vimos em aula, trata-se do NAT (Letra B).

Apesar de todas  as soluções de curto prazo (Ex: DHCP, NAT, etc), o esgotamento de endereços ainda é um problema de longo prazo para a Internet.
Esse e outros problemas no protocolo IP em si  –  como  a  falta  de  tratamento  específico  para  transmissão  de  áudio  e  vídeo  em  tempo  real  e  a criptografia/autenticação  de  dados  para  algumas  aplicações  –  têm  sido  a  motivação  para  o surgimento do IPv6 (IP Versão 6).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






23
105
(MPE/RN – 2010) A Internet não foi originalmente projetada para lidar com um número extremamente grande  de  usuários.  Como  o número  de pessoas  com  acesso  à  Internet aumentou  de  maneira  explosiva,  o  mundo  está  ficando  sem  endereços  IP  disponíveis.
Para resolver esse problema está sendo implantado o:

a) IPv4   b) IPvPLUS    c) IPMAX d) IPv6 e) IPv8 _______________________ Comentários: conforme vimos em aula, trata-se do IPv6 (Letra D).

A  nova  versão  possui  128  Bits,  logo  temos  até 2¹² 8
possíveis  endereços  ou 340 undecilhões de endereços ou 340.282.366.920.938.000.000.000.000.000. 000.000.000 de endereços!

No  IPv4,  decidiu-se  utilizar  uma  representação  decimal  de  32  bits  para  facilitar  a  configuração!
Ainda que fizéssemos isso com o IPv6, teríamos uma quantidade imensa de números. Dessa forma, optou-se por utilizar uma representação com hexadecimal, que necessita de todos os números e mais algumas letras: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F. Dividem-se 128 Bits em 8 grupos de 16 Bits (seção de 4 hexadecimais), separados por dois-pontos.



O IPv6 não possui o conceito de classes e nem endereço de broadcast. Além  disso,  como  o endereço  ainda  fica  grande  com  o  hexadecimal,  há  algumas  formas  de  abreviar:  zeros  não significativos  de  uma  seção  (quatro  dígitos  entre  dois-pontos)  podem  ser  omitidos,  sendo  que apenas  os  zeros  não  significativos  podem  ser  omitidos  e,  não,  os  zeros  significativos.  Na  tabela abaixo, temos um exemplo:

ENDEREÇO ORIGINAL
FDEC:0074:0000:0000:0000:B0FF:0000:FFF0 ENDEREÇO ABREVIADO
FDEC:74:0:0:0:B0FF:0:FFF0 ENDEREÇO MAIS ABREVIADO FDEC:74::B0FF:0:FFF0 
Usando-se essa forma de abreviação, 0074 pode ser escrito como 74, 000F como F e 0000 como 0.
Observe que se tivéssemos o número 3210, por exemplo, não poderia ser abreviado. Outras formas de  abreviações  são  possíveis  se  existirem  seções  consecutivas  formadas  somente  por  zeros.
Podemos eliminar todos os zeros e substituí-los por um dois-pontos duplo. Note que esse tipo de abreviação é permitido apenas uma vez por endereço.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






24
105
Se existirem duas ocorrências de seções de zeros, apenas uma delas pode ser abreviada.  A reexpansão  do  endereço  abreviado  é  muito  simples:  devemos  alinhar  as  partes  não  abreviadas  e inserir  zeros  para  obter  o  endereço  original  expandido. É  interessante  notar  também  que  o  IPv6 permite  também  o  endereçamento local,  isto  é,  endereços  usados  em  redes  privadas.  Por  fim,  o IPv6 pode se comunicar com o IPv4. Bacana?

(CRP - 2º Região (PE) – 2018) Os computadores em redes IPv6 são identificados por um conjunto de algarismos conhecidos como endereços IP. Considerando essa informação, assinale a alternativa que apresenta um endereço IPv6 incorreto.

a) 2001:0DH8:000:000:130G:000:000:140B b) 2001: DB8:0:54::
c) 2001:DB8:0:0:130F::140B d) 2001:DB8:0:54:0:0:0:0 e) 2001:DB8::130F:0:0:140B _______________________ Comentários: (a) Errado, não existe G ou H em Hexadecimal (Letra A).

(TJ/AC – 2012) O IPV6 é um endereçamento de IP que utiliza 32 bits.
_______________________ Comentários: conforme vimos  em aula,  IPv6  é um  endereçamento  de IP  que  utiliza 128  bits –  em contraste com  o  IPv4, que utiliza 32 Bits (Errado).














Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






25
105
4.1.2 – ICMP (INTERNET CONTROL MESSAGE PROTOCOL) INCIDÊNCIA EM PROVA: baixíssima 
Nós já sabemos que o protocolo IP fornece serviços não confiáveis de entrega de pacotes. Ele foi projetado dessa forma para utilizar os recursos da rede de forma mais eficiente, oferecendo serviços de  entrega  de  melhor  esforço  que  possibilitam  encaminhar  um  pacote  desde  sua  origem até  seu destino  final.  No  entanto,  ele  apresenta  duas  deficiências:
falta de controle de erros e falta de mecanismos de notificação de erros.

Agora  o  que  acontece  quando  algo  dá  errado  na  entrega  de  um  pacote  ao  destinatário?  E  se  um roteador  não  conseguir  encontrar  um  caminho  até  o  destino  final?  O  que  acontece  se  houver  um problema nos cabos de Internet? Estes são alguns exemplos de situações nas quais ocorreram erros!
O protocolo IP não apresenta mecanismos integrados para notificar erros ao remetente dos dados. E agora, o que fazer?

O
ICMP (Internet Control Message Protocol) foi desenvolvido para suprir essas deficiências – ele é um protocolo auxiliar do protocolo IP.
Trata-se de um protocolo da camada de Internet/Rede da Arquitetura  TCP/IP,  sendo  utilizado  para  comunicar a  ocorrência  de  situações  anormais  na transferência  de  um  pacote,  gerando  relatórios  de  erros 2
à  fonte  original  e  respondendo  às consultas a respeito do estado das máquinas da rede e roteadores.



Na  imagem  acima,  eu  executo  o  comando ping. Esse comando utiliza o protocolo ICMP para verificar a conexão com  uma máquina qualquer.  Nesse  caso,  eu  tentei  acessar  o  servidor  do Estratégia  Concursos  em www.estrategiaconcursos.com.br.  Notem  que  ele  informa  que  foram enviados 4 pacotes para o servidor e 4 foram recebidos, logo não houve perda. Ocorreu tudo muito rápido (média de 171 milissegundos) e foi um sucesso.

(ANAC – 2009) O protocolo ICMP é exemplo de protocolo da camada de aplicação.
_______________________ Comentários: conforme vimos em aula, ele é um protocolo da Camada de Rede/Internet (Errado).

2
Note que ele não é responsável por corrigir eventuais falhas, apenas comunicá-las por meio de relatórios.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






26
105
4.1.3 – ARP (ADDRESS RESOLUTION PROTOCOL) INCIDÊNCIA EM PROVA: baixíssima 
Protocolo da Camada de Rede/Internet, ele é responsável por manter uma tabela de conversão de endereços lógicos em endereços físicos. Vocês devem se lembrar que endereço lógico é o endereço IP  e  endereço  físico  é  o  endereço  MAC.
Esse protocolo mantém uma tabela de mapeamento entre endereços IP (Camada de Rede) e endereços MAC (Camada de Enlace). Onde eu encontro essa tabela, professor?

No prompt de comando do sistema operacional, se você digitar arp -a, você verá a tabela e todas as suas  entradas,  conforme  imagem  a  seguir.  Note  que  temos  uma  coluna  com  Endereço  IP  e  outra com  Endereço  Físico.
Existe  também  o  Reverse  ARP  (RARP),  que  é  responsável  por  fazer  o sentido contrário, isto é, ele mapeia endereços MAC (Camada de Enlace) para endereços IP (Camada de Rede).



(ANP – 2013) O ARP (Address Resolution Protocol) é um protocolo de interface entre as camadas  de  enlace  e  rede,  permitindo  livre  escolha de  endereços  IP  no  nível  inferior (enlace).   Ele  seria   desnecessário   se   todas   as   interfaces   da   rede   entendessem   o endereçamento IP.
_______________________ Comentários: conforme vimos em aula, ele não permite a livre escolha de Endereços IP. Na verdade, dado um Endereço IP, ele é capaz de mapear um Endereço MAC (Errado).





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






27
105
4.2 - Protocolos da Camada de Transporte 
4.2.1 – TCP (TRANSMISSION CONTROL PROTOCOL) INCIDÊNCIA EM PROVA: ALTA 
Seus lindos, nós vimos insistentemente que o protocolo IP é não confiável, porque ele não consegue garantir que as informações sejam entregues em perfeito estado, mas existe um cara que consegue garantir isso – ele se chama Transmission Control Protocol (TCP). Vocês se lembram do exemplo do motorista do caminhão dos Correios? Ele não garantia a entrega dos pacotes, porque ele poderia pegar um congestionamento na estrada, poderia ser assaltado, etc.

Agora suponha que o caminhão do nosso motorista infelizmente seja assaltado e os ladrões levem seu  pacote  embora.  Ora,  você  não  receberá  seu  pacote!  Pergunto: você entrará com um processo contra o motorista ou contra os Correios? Imagino que a segunda opção, uma vez que eles são – como instituição  –  os  responsáveis  pela  entrega  e,  não, o  motorista.  Voltando  para  nossa  analogia,  o motorista do caminhão é o IP e a Empresa de Correios e Telégrafos é o TCP!

O Protocolo de Controle de Transmissão (TCP) é um protocolo confiável, pois garante que os dados serão entregues íntegros, em tempo e em ordem.  Logo,  se  eu  quero  garantir  que  meu pacote chegará ao seu destino final, eu devo usar tanto o IP (protocolo que vai levar o pacote por várias  redes)  quanto  o  TCP  (que  vai  garantir  a  entrega  do  pacote).  Para  tal,  encapsula-se  o  TCP dentro do pacote IP. Isso mesmo! O TCP vai dentro do IP controlando e monitorando tudo...

O IP é um protocolo muito bom, mas ele não estabelece um contato com o destino antes de enviar os  pacotes;  não  é  capaz  de  garantir  a  entrega  dos  dados;  não  é  capaz  de  predizer  quão congestionada  está  uma  rede;  e  não  é  capaz  controlar  o  fluxo  de  pacotes  enviados  para  o destinatário.
Já o TCP é um protocolo orientado à conexão e confiável que faz o controle de congestionamento e de fluxo e ainda permite a comunicação ponto-a-ponto .

 PROTOCOLO TCP É ORIENTADO A CONEXÕES:

Porque comunica o destinatário que enviará pacotes antes de enviá-los de fato! Como assim, Diego? Imaginem que eu moro em uma casa pequena e quero me desfazer de algumas coisas para sobrar mais espaço em casa. Para tal, eu tenho a ideia de armazenar tudo em pacotes e deixá-los na casa do meu pai – que é bem mais espaçosa. Antes de simplesmente enviar os pacotes para o meu pai, eu entro em contato:

- Oi, pai! Como você está?
- Tudo ótimo, filho! O que você manda?
- Eu queria te enviar 100 pacotes para armazenar na sua casa. Pode ser?
- Pode, sim! Sem problemas.
- Eu vou começar enviando dez pacotes agora. Ok?
- Ok! Estou pronto para receber os dez pacotes agora!
...
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






28
105

Vocês podem notar que, antes de enviar os pacotes efetivamente, eu bati um papo com meu pai e expliquei  a  situação  de  forma  que  ele  ficasse  preparado.  Se  eu  falasse  que  iria  enviar  naquele momento dez pacotes e meu pai não recebesse nada, ele me avisaria que não havia recebido e eu poderia  verificar  o  que  aconteceu  no  meio  do  caminho.
Por meio desse mecanismo, é possível garantir que – ao final da conexão – todos os pacotes foram bem recebidos.

Logo,  quando  um  ponto  A  quer  enviar  e  receber  dados  a  um  ponto  B,  os  dois  estabelecem  uma conexão entre eles, depois os dados são efetivamente trocados em ambos os sentidos, e a conexão é encerrada. Nesse sentido, esse protocolo é diferente do UDP (que veremos no próximo tópico).
O
UDP não é orientado à conexão, logo ele não estabelece nenhuma conversa inicial antes de enviar os pacotes de dados.

 PROTOCOLO TCP É CONFIÁVEL:

Professor,  como  esse  protocolo  pode  garantir  a  entrega  confiável  de  pacotes  de  dados?  Uma  das maneiras  é  por  meio  do  estabelecimento  de uma  conexão  inicial,  mas  existem diversas técnicas que  ele  pode  implementar  para  recuperar  pacotes  perdidos,  eliminar  pacotes  duplicados, recuperar dados corrompidos e ele pode recuperar até mesmo a conexão em caso de problemas no sistema ou na rede.

 PROTOCOLO TCP IMPLEMENTA CONTROLE DE CONGESTIONAMENTO:

Galera, toda vez que meu pai recebe dez pacotes, ele me avisa que os recebeu. Se eu percebo que ele está demorando demais para receber os pacotes que eu estou enviando, eu posso concluir – por exemplo – que o tráfego está intenso e que o caminhão de entrega está em um congestionamento.
Se  eu  percebo  isso,  eu  posso  reduzir  a  quantidade  de  pacotes  enviados.
É basicamente dessa
forma que esse protocolo faz um controle de congestionamento.


 PROTOCOLO TCP IMPLEMENTA CONTROLE DE FLUXO:

Imaginem que meu pai me diga que hoje ele não conseguiu abrir muito espaço na casa dele para armazenar meus dez pacotes e me avise que – dessa vez – ele só tem espaço para armazenar apenas cinco pacotes. Eu posso reduzir meu fluxo e enviar apenas a quantidade que ele consegue absorver de forma que ele não fique sobrecarregado. É basicamente dessa forma que esse protocolo faz um controle de fluxo.

 PROTOCOLO TCP PERMITE UMA CONEXÃO PONTO-PONTO:

Imaginem que na rota terrestre entre duas capitais existam dezenas de cidades. Nós podemos dizer que entre esses dois pontos existem dezenas de caminhos diferentes. O protocolo TCP é capaz de criar  uma  conexão  entre  dois  pontos  –  fim-a-fim  –  ignorando  quaisquer  nós  intermediários  que existam entre emissor e destinatário da informação.
O IP é um protocolo nó-a-nó e o TCP é um protocolo ponto-a-ponto (ou fim-a-fim).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






29
105

Vamos  voltar  agora  para  aquele  exemplo  lááááá  de  trás  em  que  dividimos  uma  foto  em  cem pacotinhos. Quando a máquina de destino receber o primeiro dos cem pacotes, ela vai enviar uma confirmação para o emissor dizendo que tudo chegou corretamente. Quando o emissor receber a confirmação, ele enviará o segundo pacote, e assim por diante. Dessa forma, ele garante que todos os pacotes chegaram íntegros, em tempo e na ordem correta.

Ele  monitora,  acompanha,  rastreia,  controla  e  gerencia  todo  o  transporte  da  informação.
Professor, e se acontecer algum problema e o pacote se perder no meio do caminho? Pode acontecer!
O  TCP  é  responsável  por  requisitar  o  reenvio  daquele  pacote  pela  máquina  de  origem.  Quando todos  os  cem  pacotes  chegarem,  a  máquina  de  destino  os  remonta  de  forma  que  o  destinatário consiga abrir o conteúdo enviado.

Por  fim,  vamos  falar  sobre  portas! Para  tal,  vamos  fazer  uma  analogia:
imaginem  que  moram  cinco  pessoas  na  sua  casa.  Para que  um  carteiro  lhe entregue um pacote, ele precisa do seu endereço. No entanto, esse endereço é compartilhado por toda a sua família. O carteiro não vai entrar na sua casa, procurar  qual  é  o  seu  quarto,  bater  na  sua  porta  e entregar  um  pacote diretamente para você.

Nesse  sentido,  podemos  dizer  que  a  sua  casa  possui um  único  endereço,  mas  ela  possui  diversos quartos, cada um com uma porta de modo que cada morador pode utilizar o serviço dos Correios.
Agora acompanhem o Tio Diego:
imaginem que um pacote de dados viajou o planeta e por meio do seu endereço IP, ele finalmente chegou no seu computador . Só que o seu computador possui dezenas de processos diferentes em execução. E aí, qual deles é o dono do pacote?

Processos, professor? Sim, veja só! Pressione simultaneamente as teclas CTRL+SHIFT+DEL!   Esse   atalho   abrirá   o Gerenciador de Tarefas do seu computador.
Observem
que várias abas serão exibidas, sendo  que  a  primeira  delas  é  a  aba  de processos.

Nessa    aba,    estarão    listados    diversos processos   que   estão   sendo   executados atualmente    em    seu    computador.    No exemplo  ao  lado,  no  meu  computador,  há nove  aplicativos  abertos  em  primeiro  plano no momento em que eu escrevo essa aula – cada um executando um ou mais processos.

Pois é... na camada de enlace de dados, nós utilizamos o endereço MAC; na camada de rede, nós utilizamos  o  endereço  IP;  já  na  camada  de  transporte,  nós  utilizamos  o  número  da  porta  para Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






30
105
escolher um entre vários processos que estão em execução no destino. Então o pacote percorreu o mundo inteiro em rotas terrestres e submarinas, chegou no meu computador e agora ele precisa saber qual processo deve recebê-lo. Para tal, ele precisa do número da porta!

Galera, o número da porta de destino é necessário para entrega e o número da porta de origem é necessário para resposta. Professor, como são esses números?  Cara,  são  apenas  números  que variam  entre  zero  e  65535.  Cada  uma  pode  ser  usada por  um  programa  ou  serviço  diferente,  de forma  que  –  em  tese  –  poderíamos  ter  até  65536  serviços  diferentes  ativos  simultaneamente  em um mesmo servidor (com um único Endereço IP).

Por exemplo: quando você está acessando uma página web por meio de um navegador, a página web  está  armazenada  em  um  servidor  em  algum  lugar  do  mundo  e  o  navegador  está  no  seu computador.
O navegador é utilizado para acessar a web e o protocolo padrão da web é o HTTP!
Logo,  para  que  o  seu  computador  troque  dados  com  o servidor  que  armazena  a  página  do Estratégia Concursos, você precisará de uma porta. Vocês se lembram do porquê?

Porque um pacote encontrará o computador ou o servidor, mas não saberá qual processo é o dono do pacote. No caso do HTTP, a porta padrão é a 80! Por que exatamente esse número? Galera, tem uma organização chamada  IANA  (Internet Assigned Number Authority) responsável por definir e controlar algumas portas – ela definiu que a porta do HTTP é a 80! Logo, vamos fazer um último teste! Tentem acessar o endereço:
http://www.estrategiaconcursos.com.br:80.

Notem que a página do Estratégia Concursos abrirá normalmente. Agora tentem com um número de porta diferente – por exemplo:
http://www.estrategiaconcursos.com.br:21.



Vejam que retornará um erro chamado ERR_UNSAFE_PORT. Esse erro é retornado quando você tenta acessar dados utilizando uma porta não recomendada pelo navegador. Em outras palavras, você está utilizando a porta errada! Agora para fechar a nossa analogia:
o endereço IP contém o endereço da sua casa, mas é a porta que  determinará à qual quarto (processo) pertence o pacote. Bacana? Então vamos ver uma listinha com as principais portas...

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






31
105

PROTOCOLO (CAMADA DE APLICAÇÃO) PROTOCOLO (CAMADA DE TRANSPORTE) NÚMERO DA PORTA HTTP TCP 80
HTTPS
TCP 443
POP3 TCP 110
SMTP TCP
25/587
3

IMAP3
TCP 220
IMAP4 TCP 143
FTP
TCP 20/21
TELNET
TCP 23
SSH TCP 22
DNS
TCP/UDP 53
DHCP UDP 67/68
IRC TCP 194
SNMP
UDP 161/162

(DPE/RR  –  2015) Um  Técnico  em  Informática  executou  um  procedimento que  fez  a conexão a um servidor na porta TCP 443. Esta é a porta padrão do protocolo:

a) IPsec  b) HTTP c) HTTPS d) SSH e) SGMP _______________________ Comentários: conforme vimos em aula, trata-se do Protocolo HTTPS (Letra C).

(TJ/SP – 2012) Numa  rede  com  o  ISA  Server  2006,  os  usuários  necessitam  acessar  os protocolos POP3, HTTP, HTTPs e SMTP nas suas portas padrões. Assinale a alternativa que apresenta, correta e respectivamente, as portas correspondentes a esses protocolos.

a) 25, 80, 443,110
b) 110, 80, 443, 25
c) 110, 80, 25, 443
d) 443, 80, 25, 110
e) 443, 80, 110, 25
_______________________ Comentários: conforme vimos em aula, trata-se das Portas 110, 80, 443 e 25 (Letra B).

3
Via de regra, o padrão respaldado pela RFC do SMTP é Porta 25. Excepcionalmente, o Brasil adotou a porta 587 para evitar SPAM.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






32
105
4.2.2 – UDP (USER DATAGRAM PROTOCOL) INCIDÊNCIA EM PROVA: baixíssima Protocolo da Camada de Transporte, ele fornece um serviço de entrega sem conexão e não- confiável (sem controle de fluxo e de erros). Esse protocolo é praticamente o inverso do anterior –  ele  não  adiciona  nenhum  controle  adicional  aos  serviços  de  entrega  do  IP,  exceto  pelo  fato  de implementar  a  comunicação  entre  processos,  em  vez  da  comunicação  entre  nós.  Ele  até  realiza alguma verificação de erros de erros, mas de forma muito limitada.

Professor,  se  esse  protocolo  é  tão  simples  assim,  por  que  um  processo  iria  querer  usá-lo? Com  as desvantagens vêm algumas vantagens! Por ser muito simples, ele tem um baixo overhead (tráfego adicional desnecessário). Se um processo quiser enviar uma pequena mensagem e não se preocupar muito com a confiabilidade, o UDP é uma boa escolha. Ele exige menor interação entre o emissor e o receptor do que quando utilizamos o TCP.

Pessoal,  alguns  contextos  específicos  não  se  preocupam  se  um  pacote  eventualmente  for perdido, duplicado ou chegar fora de ordem. Se eu estou conversando com outra pessoa por áudio ou vídeo, perder um ou outro pacote de dados não causa problemas significativos – talvez eu perca uma palavra ou outra quando estou conversando por áudio com alguém; se eu estiver conversando por vídeo, pode ser que eu perca alguns quadros.

No entanto, não faz nenhum sentido tentar reenviar esses pacotes perdidos – como ocorre com o TCP. Por  que?   Porque   nesses   serviços real-time   (tempo   real),   essas   pequenas   perdas   são insignificantes. Bacana?
Então TCP e UDP  possuem algumas vantagens e desvantagens em relação ao outro dependendo do contexto de utilização.  Por  fim...  eu  quero  fazer  mais  uma analogia para que vocês entendam melhor!


TCP é a aquele seu colega do trabalho que é bastante formal e sistemático e que – quando deseja ir na  sua  casa  –  liga  antes  para  avisá-lo,  verifica  se  você  pode  recebê-lo,  verifica  se  você  tem disponibilidade, marca uma data e chega na sua casa com pontualidade britânica. Já o UDP é aquele seu  brother  da  época  de  faculdade  que  não  avisa  coisa  nenhuma,  bate  na  sua  porta  22h  de  uma quarta-feira, diz que veio para assistir um jogo de futebol e peida no meio da sala.

Abaixo  há  uma  famosa  piada  nerd  sobre  o  protocolo  TCP!  Quem entender, comenta no fórum; e quem não entender pergunta :) 
- Você quer ouvir uma piada sobre o TCP?
- Sim, eu quero ouvir uma piada sobre o TCP.
- Você está pronto para ouvir uma piada sobre o TCP?
- Sim, estou pronto para ouvir uma piada sobre o TCP.
- Aqui está uma piada sobre o TCP.
- Você recebeu a piada sobre o TCP?
- Eu recebi a piada sobre o TCP.
- Excelente. Você recebeu a piada sobre o TCP. Tchau!
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






33
105
4.3 – Protocolos da Camada de Aplicação 
4.3.1 – SMTP (SIMPLE MAIL TRANSFER PROTOCOL) INCIDÊNCIA EM PROVA: ALTA Protocolo da Camada de Aplicação, ele é o principal protocolo de envio de correio eletrônico (e- mail) através da rede .  Esse  protocolo  é  utilizado  para  enviar  um  e-mail de  um cliente  de  correio eletrônico até um ou mais servidores de correio eletrônico. Como assim, Diego? Calma, nós vamos entender  isso  melhor,  mas  antes  precisamos  definir alguns  termos  importantes  para  todos  os protocolos de correio eletrônico. Vejam só...


Cliente de E-Mail: trata-se de uma aplicação geralmente instalada em uma máquina local que permite enviar/receber e-mails (Ex: Mozilla Thunderbird, Microsoft Outlook, etc);


Servidor de E-Mail: trata-se do servidor remoto que recebe e-mails de um cliente de e-mail ou de um webmail e os envia para o servidor de e-mail de destino;

 Provedor de E-Mail:  trata-se  de  uma  empresa  que  hospeda  e  disponibiliza  serviços  de  e-mail para outras empresas ou usuários finais (Ex: Gmail, Outlook, Yahoo, Uol, etc);


Webmail:  trata-se  de  uma  aplicação  geralmente  hospedada  em um  servidor  remoto  que permite enviar/receber e-mails (Ex: Outlook.com, Gmail.com, Yahoo.com, Uol.com, etc).

Imaginemos   um   cenário   em   que   uma   menina   chamada Maggie  deseja  enviar  um  e-mail  para  o  seu  amigo  chamado Rob.  Ela  utiliza  o  Yahoo!  como  Provedor  de  E-Mail. Além disso, ela gosta de utilizar o Microsoft Outlook – instalado em seu  computador  – como  seu  Cliente  de  E-Mail.  Para  garantir que  ele  consiga  se  comunicar  com  o  Servidor  de  E-Mail  do Yahoo!,   ela   deve   fazer   uma   série   de  configurações   (Ex:
Endereço do Servidor SMTP do Yahoo!).


smtp.email.yahoo.com 
Bacana! Agora que ela configurou o endereço do Servidor  de  E-Mail  (SMTP)  do  Yahoo!,  ela  pode enviar e-mails para quem ela quiser. Vamos supor que  ela  deseje  enviar  e-mails  para  o  seu  amigo Rob!   No   entanto,   seu   amigo   utiliza   outro provedor de e-mail – ele utiliza o Gmail. Há algum problema?
Não, não há problema algum!

Nesse  caso,
quando ela clicar no botão de enviar e-mail, ocorrerão alguns passos.  Primeiro,  o Microsoft  Outlook  enviará  a  mensagem  para  o  Servidor  de  E-Mail  do  Yahoo!  Cadastrado Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






34
105
anteriormente.  Segundo,  o  Servidor  SMTP  dividirá  0 e-mail  do  destinatário  –  no  caso,  Rob  –  em duas  partes: rob e gmail.com.  Terceiro,  ele  ignorará  a  primeira  parte,  identificará  o  domínio  na segunda parte (gmail.com) e procurará na Internet o Servidor SMTP do Gmail.



Quarto,  quando  ele  encontrar  o  Servidor  SMTP  do  Gmail,  ele  enviará  a  mensagem  para  esse servidor. Quinto, quando a mensagem chegar ao Servidor SMTP do Gmail, ele também quebrará o e-mail de Rob em duas partes, mas ignorará a segunda parte e identificará apenas a primeira (rob).
Se esse nome de usuário existir no servidor, ele armazenará a mensagem de Maggie na caixa de entrada de Rob
! Ficou mais fácil de entender agora?



Galera, eu preciso falar um pequeno detalhe para vocês. Isso caiu apenas uma vez em prova, mas foi  uma  polêmica  absurda!  Eu  disse  na  primeira  frase  sobre  esse  protocolo  que  ele  é  o  principal protocolo de envio de correio eletrônico através da rede. Eu menti? Não!
No entanto, notem que ele pode ser utilizado para receber e-mail em uma única situação. Para entender melhor, vamos analisar a imagem a seguir:



Percebam  que  o  remetente  utiliza  o  protocolo  SMTP  para  enviar  uma  mensagem  de  correio eletrônico.
No entanto, notem que na comunicação entre o servidor de correio eletrônico do remetente  e  do  destinatário  também  é  utilizado  o  SMTP.  Logo,  nesse  caso  específico  de Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






35
105
comunicação entre servidores, ele é utilizado tanto para recebimento quanto para envio de correio eletrônico. Não é o padrão, é apenas nesse caso! Bacana?

(Polícia Federal – 2018) SMTP é o protocolo utilizado para envio e recebimento de email e opera na camada de aplicação do modelo TCP/IP.
_______________________ Comentários: conforme vimos em aula, ele realmente pode ser utilizado para envio e recebimento de e-mail (Correto).

Importante: nós vimos o caso em que o remetente envia um e-mail por meio de um Cliente de E-Mail.  No  caso  da  utilização  de  um  webmail  (Ex:  Yahoo.com),  a  transferência  de  mensagens  do navegador do remetente para seu servidor de correio eletrônico é feita pelo HTTP; em seguida, a transferência  de  mensagens  do  servidor  do  remetente  para  o  servidor  do  destinatário  se  dá  por meio do SMTP; e, por fim, o HTTP é novamente usado pare recuperar o e-mail.



S M T P
SUA MENSAGEM TÁ  PARTINDO 
(TJ/PE – 2012) Em  relação  às  etapas  envolvidas  no  envio  e  recebimento  de  e-mail,  é INCORRETO afirmar:

a) O usuário redige a mensagem e clica no botão Enviar, do seu programa cliente de e- mail para que a mensagem chegue até o servidor, chamado Servidor de Saída.

b) Após receber a solicitação do programa cliente, o Servidor de Saída analisa apenas o segmento de endereço que se encontra após o símbolo @.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






36
105

c)  Após  identificar  o  endereço  de  domínio  de  destino,  a  próxima  tarefa  do  Servidor  de Saída é enviar a mensagem solicitada por seus usuários, e para isso, utiliza o protocolo SMTP (Simple Mail Transfer Protocol).

d)  Quando  a  mensagem  chega  ao  servidor  de  destino, conhecido  como  Servidor  de Entrada,  este  identifica  a  informação  existente  antes  do  símbolo  @  e  deposita  a mensagem na respectiva caixa postal.

e) Para transferir as mensagens existentes no Servidor de Entrada para seu computador, o usuário utiliza o programa cliente de e-mail que, por sua vez, utiliza o protocolo SMTP (Simple Mail Transfer Protocol) para depositar a mensagem no seu computador.
_______________________ Comentários: conforme vimos em aula, todos os itens estão corretos, exceto o último! O usuário utiliza os Protocolos POP3 ou IMAP para descarregar a mensagem para o seu computador (Letra E).




























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






37
105
4.3.2 – POP3 (POST OFFICE PROTOCOL, VERSÃO 3) INCIDÊNCIA EM PROVA: ALTA Protocolo  da  Camada  de  Aplicação, ele foi criado como uma forma simplificada para receber, baixar e deletar mensagens de um servidor de e-Mail.  Vocês  devem  se  lembrar  que  o  SMTP  é responsável por enviar o e-mail até o servidor de e-mail do destinatário. A partir daí, se ele estiver utilizando um cliente de e-mail, ele poderá utilizar o POP3 ou IMAP para recuperar do servidor de correio eletrônico os e-mails recebidos.



Esse protocolo trabalha em dois modos distintos: em um modo, ele apaga as mensagens da caixa postal  logo  após  a  realização  do  download  – era  normalmente  utilizado  quando  o  usuário estava trabalhando  em  um  computador  fixo  e  tinha  condições  de  salvar  e  organizar  as  mensagens recebidas após sua leitura ou resposta; e em outro modo, ele mantém uma cópia das mensagens na caixa postal mesmo após a realização do download.

Esse  modo  era  normalmente  utilizado  quando  o  usuário  acessava  suas  mensagens  de  outro computador  que  não  fosse  o  seu  principal  –  as  mensagens  eram  lidas,  mas  mantidas  no  sistema para futura recuperação e organização.
Eu gostaria que vocês pensassem nesse protocolo como uma secretária eletrônica antiga – aquelas que utilizavam uma fita para gravar mensagens de voz
. Todos sabem o que era uma secretária eletrônica?

Para os mais novos: era um dispositivo para responder automaticamente chamadas telefônicas e gravar  mensagens  deixadas  por  pessoas  que  ligavam  para  um  determinado  número,  quando  a pessoa  chamada  não  podia  atender  o  telefone.  Podia acontecer  de  várias  pessoas  deixarem mensagens de voz pela secretária.
Nesse caso, você poderia ouvir as mensagens e não as apagar ou você poderia ouvi-las e imediatamente após apagá-las (como no POP).

Em geral, o protocolo utiliza – por padrão – o primeiro modo, isto é, apagam-se da caixa postal as mensagens  logo  após  a  realização  do  download. Qual  é  o  problema  disso?
Uma  vez  feito  o
download, as mensagens só ficam disponíveis para vê-las novamente na máquina em que foi feito o download.  Logo,  após  apagadas  as  mensagens,  você  não  poderia  vê-las  por meio  de  um webmail, por exemplo.

Esse  protocolo  era  indicado  para  as  pessoas  não  conectadas  permanentemente  à  Internet,  para poderem consultar os e-mails recebidos de forma offline.
Lembrem-se que – até um tempo atrás Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






38
105
– o acesso à Internet era algo bastante raro e muitas pessoas não podiam ficar sem acesso aos seus e-mails quando não estivessem conectadas à Internet. Nesse contexto, o POP era bastante indicado!

(Prefeitura de Amontada – Adaptado – 2016) O POP3 é responsável por receber e-mail do servidor do destinatário armazenando-a na máquina do destinatário.
_______________________ Comentários: conforme  vimos  em  aula,  ele  é  realmente  utilizado  para  receber  e-mail  do  servidor  do  destinatário  e  é armazenado na máquina do destinatário por padrão (Correto).


































Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






39
105
4.3.3 – IMAP (INTERNET MESSAGE ACCESS PROTOCOL) INCIDÊNCIA EM PROVA: ALTA O  POP3  é  ineficiente em  diversas  situações! Ele  não permite  ao  usuário  organizar  mensagens  ou criar  pastas  no  servidor.  Além  disso,  não  é  possível  que  o  usuário  verifique  parte  do  conteúdo  da mensagem antes de fazer o download. O IMAP permite que você acesse todos os seus correios eletrônicos – por meio de um cliente de e-mail ou de um webmail – a qualquer momento . Além
disso, ele traz diversas funções adicionais:

Um usuário pode verificar o cabeçalho de um e-mail antes de baixá-lo; pode procurar pelo conteúdo de  um  e-mail  antes  de  baixá-lo;  pode  baixar  parcialmente  um  e-mail  –  isso  é  útil  se  a  largura  de banda  for  limitada  e  o  e-mail  tiver  conteúdos  com  grandes  exigências  de  largura  de  banda;  um usuário pode criar, eliminar ou renomear caixas de correio no servidor de e-mail; e pode criar uma hierarquia de caixas de correio em pastas para armazenamento de e-mails.




Ele permite armazenar seus e-mails nos servidores de e-mail do seu provedor de e-mail até que você os delete
. Apesar de isso ser bem mais conveniente, alguns provedores de e-mail limitam a quantidade   de   e-mail   que   você   pode   armazenar   em   seus   servidores   e   pode   suspender temporariamente  seus  serviços  se  você  exceder  esse limite. Alguém  aí  já  chegou  perto  do  limite gratuito de 15 Gb do Gmail? Se sim, é esse o caso!

Vocês podem pensar no IMAP como uma secretária eletrônica online – possivelmente armazenada na nuvem.
Dessa forma, qualquer mensagem que ela receber fica armazenada na nuvem e pode ser acessada por meio de diferentes dispositivos ou softwares até que você as delete.  Não  é necessária  muita  preocupação  com  segurança,  visto  que  o  IMAP  possui  uma  versão  mais  segura chamada IMAPS (IMAP Secure).

Em  geral,  se  você  sempre  utiliza  seu  e-mail  em  uma única  localização  ou  por  meio  de  um  único dispositivo, ou até mesmo se você tem problemas com acesso à Internet – recomenda-se utilizar o POP.
Por  outro  lado, se  você  utiliza  seu  e-mail  em  diferentes  localizações  ou  por  meio  de dispositivos diferentes, e se você não tem problemas com acesso à Internet – recomenda-se utilizar o IMAP
.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






40
105
(TJ/RS  –  Adaptado  –  2017) Qual  protocolo  de  acesso  ao  correio  eletrônico  possui comandos que permitem a um usuário, através de sua ferramenta de correio eletrônico (agente  de  usuário),  criar  remotamente  uma  estrutura  de  pastas  e  subpastas  em  seu servidor de correio eletrônico para organizar suas mensagens?

a) IMAP
b) HTTP
c) POP3
d) SMTP
e) SNMP
_______________________ Comentários: conforme vimos em aula, trata-se do IMAP (Letra A).































Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






41
105
4.3.4 – DHCP (DYNAMIC HOST CONFIGURATION PROTOCOL) INCIDÊNCIA EM PROVA: baixa Protocolo  da  Camada  de  Aplicação, ele  permite  a  a alocação estática e dinâmica de endereços lógicos, que pode  ser  manual  ou  automática.  Nós  já  vimos  que,  em uma  rede  de  computadores,  pode  ser  necessário  que  um mesmo  endereço  IP  possa  ser  utilizado  em  diferentes dispositivos  em  momentos  distintos.  Para  tal,  tem  que  se configurar  quais  serão  os  endereços  desses  dispositivos.  A configuração de uma rede pode ser feita de maneira manual –  como  mostramos  ao  lado.  Dessa  forma,  a  configuração tem   que   ser   feita   máquina   a   máquina   a   partir   das propriedades   de   conexão   local.   Essa   configuração   é trabalhosa,  exige  uma  equipe  técnica  e  pode  ocasionar erros  importantes  quando  temos  uma  rede  com  muitos computadores para configurar.


No entanto, essa configuração também pode ser feita de forma automática. Nesse caso, utiliza-se um servidor para obtenção de um Endereço IP .  O  nome  desse  servidor  capaz  de  encontrar  um endereço  IP  é  Servidor  DHCP.  Ele  é  capaz  de  atribuir  uma  alocação  dinâmica  de  endereços  de acordo  com  a  disponibilidade  (muda  a  cada  nova  conexão).  Em  suma:  esse  protocolo  é  capaz  de designar e configurar endereço IP aos dispositivos de uma rede local de forma automática.

(Prefeitura  de  Carpina/PE  –  2016) Protocolo   através   do   qual   é   possível   fazer automaticamente  a  configuração  dinâmica  de  um  computador  ligado  a  uma  rede TCP/IP:

a) FDDI
b) ETHERNET
c) HDLC
d) SNMP
e) DHCP
_______________________ Comentários: conforme vimos em aula, trata-se do DHCP (Letra E).







Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






42
105
4.3.5 – DNS (DOMAIN NAME SYSTEM) INCIDÊNCIA EM PROVA: Altíssima Galera, quantos números vocês sabem decorados? Eu, por exemplo, tenho uma péssima memória!
Eu sei meu Nº de CPF, Nº de RG, Nº de Conta Bancária e Nº de Telefone. Fora isso, eu já começo a ter  dificuldades  de  lembrar.  Nós  sabemos  que  os  computadores  na  Internet  são  identificados utilizando endereços IP (Exemplo: 192.168.10.15).
Uma vez que é mais fácil decorar nomes que números, foi criado um sistema capaz de traduzir números em nomes e vice-versa.

Vamos  fazer  mais  um  teste!  Dessa  vez,  eu  quero  que vocês  abram  um  navegador  web  qualquer, digitem
216.58.211.14 e vejam o que acontece! Pois é, abrirá a página do Google! Professor, como isso é possível? Galera, toda página web está armazenada em algum servidor e nós já sabemos que todo dispositivo na internet precisa ter um endereço lógico exclusivo. Logo, um servidor também precisa de um endereço para ser acessado.




O servidor que armazena o Google tem o endereço lógico apresentado no parágrafo anterior. Agora vocês já imaginaram se nós tivéssemos que decorar todos os endereços IP de todos os sites que nós acessamos  diariamente? Seria  completamente  inviável!  Para  resolver  esse  problema,  surgiu  o Domain Name System (DNS). Trata-se de um protocolo da camada de aplicação responsável por atribuir endereços léxicos aos recursos da rede – ele é como uma agenda de contatos da Internet!

Professor,  falou  difícil  agora! Galera,  endereço  léxicos  são  aqueles  formados  por  palavras  ou vocábulos  de  um  idioma,  em  vez  de  um  número.  Em outras  palavras,  ele  busca  transformar endereços numéricos  em  nomes  amigáveis, mais  compreensíveis  para  humanos  e  mais  fáceis  de memorizar. O que é mais fácil de decorar: 216.58.211.14 ou Google.com? Pois é! Notem que, apesar de ser mais fácil para você memorizar, o computador entende apenas Endereço IP.

Imaginem que um dia você sai de uma balada de madrugada, chama um taxi e simplesmente diz ao motorista: “Parceiro, me leva na casa do João”! Ora, galera... o taxista lá sabe quem é João? Taxista conhece endereços e, não, nomes de pessoas. Nessa analogia, o taxista seria o seu navegador – ele só reconhece endereços e, não, nomes de pessoas . Professor, como o DNS consegue fazer essa tradução de nome para endereço e vice-versa?

Para fazer isso, ele consulta uma tabela parecida com uma agenda telefônica! Quem aí é da época da lista telefônica? Tô velho! Pessoal, se você possuísse o nome de uma pessoa, era possível Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






43
105
descobrir  seu  número  de  telefone.  Ocorria  também  o caso  inverso:  por  meio  de  um  número  de telefone, era possível descobrir um nome. Bem, vejamos na tabela a seguir como tudo isso funciona no caso dos computadores:

DNS (DOMAIN NAME SYSTEM) URL IP
www.google.com 216.58.211.14 
Esse endereço que nós mostramos na tabela acima é um endereço de rede no qual se encontra um recurso informático – no caso, uma página web . No entanto, é possível buscar qualquer tipo de recurso (um computador, uma impressora, um arquivo, entre outros). Para tal, é preciso saber o nome desse recurso e esse nome nós chamamos de Uniform Resource Locator (URL). Uma URL é geralmente formada pela seguinte estrutura:

ESTRUTURA DE URL
protocolo-ou-esquema://ip-ou-domínio:porta/caminho 
A URL – Localizador de Recursos Uniformes – oferece uma maneira uniforme e padronizada de localizar recursos na web. Claro  que,  na  maioria  das  vezes,  não  é  necessário  utilizar  toda  essa estrutura  apresentada  acima  para  ter  acesso  aos  recursos.  Notem,  por  exemplo,  que  a  porta  e  o caminho  são  atributos  opcionais!  Além  disso,  muitas  vezes  o  protocolo  ou  esquema  também  é opcional. O que temos, então?

Temos um protocolo: também chamado de esquema; IP ou Domínio: endereço lógico ou léxico da máquina hospedeira (host); Porta: ponto lógico em que se pode executar uma conexão; Caminho:
especifica  onde  se  encontra  um  determinado  recurso.  Na  tabela  abaixo,  há  diversos  exemplos diferentes.  Notem  que  alguns  possuem  porta,  outros não;  alguns  possuem  protocolo,  outros esquema, outros nenhum; alguns possuem caminho, outros não; etc.

DNS (DOMAIN NAME SYSTEM) www.estrategiaconcursos.com.br http://www.estrategiaconcursos.com.br http://www.estrategiaconcursos.com.br:80 http://www.estrategiaconcursos.com.br/professores ftp://admin@diegocarvalho.com.br mailto://contato@diegocarvalho.com.br 
Apesar de todas essas partes, o nome do domínio é o principal membro da URL! Por isso, dizemos que o DNS traduz, transforma, resolve um nome ou domínio em um endereço IP e um endereço IP em  um  nome  ou  domínio.  Percebam  também  na  próxima  imagem  que o DNS apresenta uma
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






44
105
estrutura hierárquica e distribuída em que seu espaço de nomes é dividido em vários servidores de domínio baseado em níveis.



Diego, o que é um espaço de nomes? Para  evitar  ambiguidades,  os  nomes  atribuídos  às  máquinas devem ser cuidadosamente selecionados a partir de um espaço de nomes – que nada mais é que um conjunto organizado de possíveis nomes. Em outras palavras, os nomes devem ser exclusivos, uma vez que os endereços IP também são.  Galera,  caso  vocês  queiram  registrar  um  domínio algum dia, vocês provavelmente terão que acessar o seguinte site:

www.registro.br

Professor, eu não tenho grana para isso não! Galera, fiquem tranquilos porque é bem baratinho. Em um plano de 10 anos, custaria pouco mais de R$3/Mês. Vejam abaixo os planos mais comuns:



O meu queridíssimo Prof. Renato da Costa, por exemplo, possui um domínio para o seu site – apesar de ele não o utilizar (deem um puxão de orelha nele)!

www.RENATODACOSTA.COM.BR 
Além disso, existem algumas categorias de domínio .br. Como assim, professor? Se você exerce uma atividade  comercial,  você  poderá  ter  um  domínio .com.br;  se  você  possui  uma  organização  não- governamental, você poderá ter um domínio .org.br. Algumas categorias possuem ainda restrições .br
.gov
tesouro
.com
estratégia
.org
lbv
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






45
105
adicionais   por   serem   direcionadas   a   empresas   de   setores   específicos,   sendo   necessária comprovação por meio de envio de documentos. Vamos ver vários exemplos abaixo...



D N S
DÁ NOME AO SITE

(CESPE – MPS – Técnico em Comunicação Social) Um  servidor  DNS  (Domain  Name Service)  permite  identificar  os  endereços  IP  de  usuários  e  servidores  da  Internet,  por meio da associação de um conjunto de números com domínios.
_______________________ Comentários: conforme  vimos em aula, ele  realmente permite  identificar  endereços lógicos  (IP)  de usuários  e  servidores  da Internet, por meio da associação de um conjunto de números com domínios, isto é, é possível identificar um endereço IP por meio de um domínio e vice-versa (Correto).




Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






46
105
4.3.6 – HTTP (HYPER TEXT TRANSFER PROTOCOL) INCIDÊNCIA EM PROVA: Altíssima Protocolo da Camada de Aplicação, ele é utilizado por programas de navegação (browsers) para acessar  dados  na  web.  Em  português,  seria  traduzido  como  Protocolo  de  Transferência  de Hipertexto. Por  que,  professor?  Porque  ele  é  responsável  pela  transferência,  formatação  e apresentação  de  páginas  web  com  conteúdo  multimídia  (textos,  áudio,  imagens,  vídeos,  entre outros) entre um servidor e um cliente na Internet.



A imagem anterior ilustra uma transação típica entre um cliente e um servidor no HTTP.  O cliente  inicializa  uma  transação  enviando  uma  mensagem  de  solicitação.  O  servidor  responde enviando  uma  mensagem  de  resposta. Como  assim,  Diego? Galera,  toda  página  web  está armazenada em um servidor web. Logo, quando você acessa qualquer página pelo navegador, você está fazendo uma solicitação ao servidor para acessar aquela página.

Se você conseguir acessá-la, significa que o servidor web autorizou e te devolveu como resposta a página que você desejava acessar.
Por falar em servidor web, esse é o nome dado ao servidor que hospeda ou armazena páginas ou recursos web – assim como o servidor que armazena e-mails é chamado de servidor de e-mail. Prosseguindo... toda solicitação ou requisição a um servidor web retorna um código de status de três dígitos e divididos em cinco categorias:

CÓDIGO CATEGORIA SIGNIFICADO 1XX INFORMAÇÃO
100 significa que o servidor concorda em atender à requisição.

2XX SUCESSO
200  significa  que  a  requisição  foi  bem-sucedida  e  204  significa  que  a página está sem conteúdo.
3XX REDIRECIONAMENTO 301  significa  que  a  página  foi  movida  e  304  significa  que  a  página  em cache ainda é válida.
4XX ERRO DO CLIENTE
403 significa que a página é proibida e 404 significa que a página não foi encontrada.
5XX ERRO DO SERVIDOR 500  significa  que  houve  um  erro  interno  e  503  significa  que  você  deve tentar novamente mais tarde.

Professor, há como explicar melhor o que você quis dizer? Claro que sim! Façam um teste: abaram seu navegador favorito e digitem:
www.estrategiaconcursos.com.br/euamopinkfloyd.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






47
105



Vocês viram que retornou um erro? Pois é, Erro 404! Esse erro é da categoria Erro do Cliente e significa que  uma  determinada  página  não  foi  encontrada. Por  que,  professor?  Cara,  essa  página  não  foi encontrada  basicamente  porque  ela  não  existe  –  eu  acabei  de  inventar  apenas  para  mostrar  um código de retorno!
Esse código sempre existirá para qualquer requisição, mas nem sempre será exibida para os usuários.


Não confundam HTTP com HTML! HTML é uma linguagem para criação de páginas web.
Basta lembrar da última letra: HTTP é Protocolo e HTML é Linguagem.

(IFTO  –  2018) Os  protocolos  de  comunicação,  em  redes  de  computadores,  são  o conjunto   de   regras   que   governam   a   interação   entre   sistemas   de   computadores distribuídos em rede. Os protocolos são usados para permitir a comunicação entre dois ou mais computadores. Os navegadores de internet utilizam um protocolo que é a base de  comunicação  de  dados  da  world  wide  web,  específico  para  a  transferência  e apresentação  de  páginas  com  conteúdo  multimídia  (informações  de  textos,  áudio, imagens  e  vídeos).  Assinale  a  opção  correta  que  identifica  o  protocolo  usado  pelos browsers que permitem os usuários a navegar na internet.

a) File Transfer Protocol (FTP) b) Internet Message Access Protocol (IMAP) c) Simple Mail Transfer Protocol (SMTP) d) Post Office Protocol (POP) e) HyperText Transfer Protocol (HTTP) _______________________ Comentários: conforme vimos em aula, trata-se do HTTP (Letra E).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






48
105
4.3.7 – HTTPS (HYPER TEXT TRANSFER PROTOCOL SECURE) INCIDÊNCIA EM PROVA: Altíssima Protocolo da Camada de Aplicação, ele tem a mesma finalidade do HTTP. Ele é responsável pela transferência, formatação e apresentação de páginas web com conteúdo multimídia (textos, áudio, imagens,  entre  outros)  entre  um  servidor  e  um  cliente.  No  entanto,  ele  realiza  transferências  de forma  segura,  oferecendo  criptografia,  autenticação  e  integridade  às  transferências  de  páginas de/para um servidor web.

Trata-se  de  uma  implementação  do  HTTP  sobre uma camada adicional de segurança que utiliza um outro   protocolo   chamado   SSL/TLS .     Esses
protocolos possuem propriedades criptográficas que permitem assegurar confidencialidade e integridade à comunicação. Dessa forma, é possível que os dados sejam   transmitidos   por   meio   de   uma   conexão criptografada  e  que  se  verifique  a  autenticidade  do servidor   web   e   do   cliente   web   por   meio   de certificados digitais.

Se  você  entrar  em  um  site  de  Internet  Banking,  você  visualizará  o  endereço  começando  com https:// e um pequeno cadeado do lado esquerdo da barra de endereço indicando que a conexão a essa  página  é  segura.  Conexões  por  meio  desse  protocolo  são  frequentemente  utilizadas  para transações de pagamentos na web e também para transações sensíveis em sistemas de informação corporativos. Bacana?

(Banco da Amazônia – 2018) O protocolo que permite a navegação na internet segura através de criptografia de informações é o:

a) HTTPS
b) HTTP
c) HTML
d) XHTML
e) XML
_______________________ Comentários: conforme vimos em aula, trata-se do HTTPS (Letra A).







Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






49
105
4.3.8 – FTP (FILE TRANSFER PROTOCOL) INCIDÊNCIA EM PROVA: Altíssima Protocolo  da  Camada  de  Aplicação, ele  é  responsável  pela  realização  de  transferências  de arquivos entre um Cliente FTP e um Servidor FTP. Definições que já encontrei em prova:

- FTP é o protocolo de transferência de arquivos entre computadores;
- FTP é o protocolo para transferência de arquivos entre dois computadores conectados à Internet;
- FTP é o protocolo responsável pela transferência de arquivos remotos;
- FTP é o protocolo que permite a cópia de arquivos entre dois computadores;
- FTP é o protocolo responsável pelo download/upload de arquivos;
- FTP é o protocolo que permite fazer upload de arquivos para um servidor remoto.

Esse protocolo difere de outros por estabelecer duas conexões entre cliente e servidor:
uma para a
transferência dos dados em si (Porta TCP 20) e a outra para a troca de informações de controle (Porta TCP 21). Essa divisão ocorre para tornar o protocolo mais eficiente, visto que as informações de  controle  utilizam  uma  conexão  mais  simples,  enquanto  a  transferência  de  dados  possui  uma conexão mais complexa, permitindo o envio de múltiplos arquivos, etc.

Trata-se  do  protocolo-padrão  para  copiar  arquivos  de  uma  máquina  para  outra,  possuindo  três modos de transmissão diferentes: de fluxo contínuo, blocado e comprimido.

MODO DE TRANSMISSÃO DESCRIÇÃO FLUXO CONTÍNUO
(stream)
O  arquivo  é  enviado,  por  um  fluxo  contínuo  de bytes,  ao TCP.  Quando  chega  nesse protocolo,  ele  separa  os  dados  recebidos  em  porções  com  um  tamanho  apropriado para o transporte – trata-se do modo-padrão.
BLOCADO
Os  dados  são  entregues  do  FTP  para  o  TCP  em  blocos.  Nesse  caso,  cada  bloco  é precedido por um cabeçalho de três bytes. O primeiro byte é chamado de descritor de blocos; os dois seguintes definem o tamanho do bloco em bytes.
COMPRIMIDO
No caso de arquivos muito grandes, os dados podem ser comprimidos, antes de serem enviados, usando um algoritmo.


(IFSP – 2012) Assinale a alternativa que informa o protocolo usado para transferência de arquivos entre computadores ligados na Internet.

a) IMAP b) FTP  c) SMTP  d) DHCP e) SNMP _______________________ Comentários: conforme vimos em aula, trata-se do FTP (Letra B).

Galera,  por  que  nós  utilizamos  a  internet? Basicamente  para  nos  comunicar!  E  para  haver comunicação,  são  necessárias  duas  partes:  um  emissor  e  um  receptor.  Quando  você  acessa  um portal da web, quando você faz o download de um arquivo, quando você joga um jogo na internet, Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






50
105
quando  você  acessa  uma  rede  social  ou  quando  você  vê  um  vídeo  no  Youtube, sempre haverá transferência (envio ou recebimento) de informações.



Por falar nisso, há dois termos que eu tenho certeza que vocês estão bastante familiarizados porque já  fazem  parte  do  nosso  vocabulário  em  português:  Download  e  Upload!  Nós  já  sabemos  que  a Internet funciona por meio de uma arquitetura ou modelo chamado Cliente/Servidor! O que é isso, professor?
Grosso modo, isso significa que ela é baseada em um conjunto de computadores que exercem a função de clientes ou servidores. Relembrando...

Os computadores servidores são aqueles que fornecem um serviço e os computadores clientes são aqueles que consomem um serviço. Sabe aquele domingo à noite em que quer ver um filme maneiro?  Você  liga  sua  televisão,  acessa  a  página  web  da  Netflix,  escolhe  um  filme  e  começa  a assisti-lo!  Nesse  momento,  sua  televisão  funciona  como  um  cliente  que  está  consumindo  um serviço. Esse serviço é disponibilizado por quem? Pela Netflix!

A Netflix possui um bocado  de computadores servidores que hospedam ou armazenam os filmes, então a sua televisão está consumindo um serviço de um servidor da Netflix .  E  quase
tudo na internet é assim: você acessa o servidor do Estratégia para ver uma videoaula; você acessa o  servidor  do  Spotify  para  ouvir  uma  música;  você  acessa  o  servidor  do  Google  para  acessar  sua página e fazer alguma busca; e assim por diante. Dito isso, vamos ver o que é download e upload...

Ambos  os  termos  são  utilizados  para  referenciar  a  transmissão  de  dados  de  um  dispositivo  para outro  através  de  um  canal  de  comunicação  previamente  estabelecido.
O termo download está relacionado com a obtenção de conteúdo da Internet, em que um servidor hospeda dados que são  acessados  pelos  clientes  através  de  aplicativos  específicos  que  se  comunicam  com  o servidor por meio de protocolos preestabelecidos (Ex: HTTP, FTP, etc).

De forma análoga, o termo upload faz referência a operação inversa à do download, isto é, refere- se  ao  envio  de  conteúdo  à internet.  Apesar  de  serem  termos  com  sentidos  opostos,  do  ponto  de vista  técnico,  a  distinção  de  um  processo  de  transmissão  entre  download  ou  upload  pode  ser associada simplesmente à uma questão de perspectiva, pois sempre que um dispositivo faz um download, o dispositivo que disponibiliza o arquivo/informação faz um upload e vice-versa .

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






51
105
No  entanto,  essa  distinção  é  normalmente  feita  considerando  a  participação  do  dispositivo  que iniciou a transmissão de dados, seja obtendo ou disponibilizando, isto é, se está obtendo dados é um download; e se está disponibilizando dados é um upload .  Voltando  agora  à  questão  dos protocolos:  FTP
4
(File  Transfer  Protocol)  é  um  protocolo  de  transferência  de  arquivos  entre computadores e HTTP (HyperText Transfer Protocol) é um protocolo de transferência de textos.

HTTP permite apenas a transferência de textos? Não!  Quando  você  faz  o  download  da  nossa  aula pelo navegador, você está transferindo arquivos por meio do Protocolo HTTP. Bacana?

(UFBA – 2018) FTP é o protocolo de transferência de arquivos entre computadores.
_______________________ Comentários: conforme vimos em aula, a questão está impecável (Correto).

(IFMS – 2016) Sobre transferência de arquivos pela internet é CORRETO afirmar que:

a) O upload corresponde à transferência de um arquivo de um servidor na internet para o computador de um usuário, sempre criando uma cópia.

b) O upload corresponde à transferência de  um arquivo do computador de um usuário para um servidor na internet, sempre eliminando o arquivo do seu local de origem.

c)  O  download  corresponde  à  transferência  de  um  arquivo  de  um  servidor  na  internet para o computador de um usuário, sempre eliminando o arquivo do servidor.

d) Para um arquivo da internet ser visualizado na tela de um computador deve sempre ocorrer o seu download antes da visualização, gerando uma cópia no computador.

e) A maioria dos downloads é feita por um método chamado FTP (File Transfer Protocol) anônimo.
_______________________ Comentários: (a) Errado, isso é um download; (b) Errado, não elimina o arquivo do seu local de origem; (c) Errado, não elimina o arquivo do servidor; (d) Errado, nem sempre é necessário ocorrer o download antecipadamente (Ex: streaming de músicas do Spotify ou de filmes da Netflix); (e) Correto. O FTP anônimo possibilita ao usuário baixar e carregar arquivos de seu site por FTP sem a necessidade de uma conta ou senha específicos (Letra E).




4
FTP tem sido cada vez menos utilizado após o surgimento de ferramentas de armazenamento em nuvem (Cloud Storage), que podem ser acessadas por meio de navegadores web por meio do Protocolo HTTP.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






52
105
4.3.9 – TELNET (TELECOMMUNICATIONS NETWORKS) INCIDÊNCIA EM PROVA: baixíssima Protocolo  da  Camada  de  Aplicação, ele basicamente permite conectar dois computadores de forma que um usuário consiga efetuar login em outro computador através da rede de forma remota.  Desenvolvida  com  as  características  de  uma  aplicação  Cliente/Servidor,  ele  proporciona uma  facilidade  de  comunicação  baseada  em  texto  interativo  bidirecional  utilizando  um  terminal virtual. Como é, professor? Vejam só...

Nós já vimos o prompt de comando algumas vezes em nossa aula. Vocês se lembram que ele permite executar uma série de comandos? Pois é! O TELNET foi criado originalmente para permitir o acesso à  linha  de  comando  de  outro  computador  em  uma  rede.
Hoje em dia, ele está completamente obsoleto porque permite que uma pessoa tenha acesso ao prompt de comando de outra e pode causar potenciais problemas de segurança .

O TELNET permite que um terminal local estabeleça uma conexão virtual a um sistema remoto de tal maneira que o terminal local se comporte exatamente como se fosse um terminal do sistema remoto. O TELNET não garante uma comunicação segura, dados e senhas são compartilhados em  texto  livre.  O  ideal  seria  ter  algum  tipo  de  autenticação,  entre  outros  mecanismos  de segurança.


(Correios  –  2011) A   ferramenta   denominada   Telnet   foi   desenvolvida   com   as características de uma aplicação cliente/servidor.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






53
105
4.3.10 – SSH (SECURE SHELL) INCIDÊNCIA EM PROVA: baixíssima Protocolo da Camada de Aplicação, ele é um protocolo de acesso remoto que utiliza autenticação de  chave  pública  baseada  no  servidor  para  estabelecer  a  identidade  do  usuário  com  segurança  e oferecer suporte à compressão de dados para a execução de aplicações com interfaces gráficas. A principal diferença para o TELNET é que ele utiliza criptografia, o que significa que os dados transmitidos na rede estão seguros contra escutas não autorizadas.

Galera,  se  vocês  já  trabalharam  em  alguma  empresa  ou  órgão  grande,  já  devem  ter  ligado  para algum  técnico  de  informática  detalhando  algum  problema  que  foi  resolvido  sem  que  o  técnico tivesse  que  se  deslocar  até  o  seu  computador.  Isso é  muito  comum!
O  técnico  de  suporte remotamente  acessa  o  seu  computador  e  o  controla  totalmente,  realizando  todas  as manutenções ou correções requisitadas .

TELNET SSH
NÃO! NÃO TEM CRIPTOGRAFIA SIM! TEM CRPTOGRAFIA 
(DPU – 2016) Os  protocolos  de  comunicação  SSH  e  TELNET  garantem comunicação segura, uma vez que os dados são criptografados antes de serem enviados.
_______________________ Comentários: conforme vimos em aula, TELNET não tem criptografia (Errado).
















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






54
105
4.3.11 – IRC (INTERNET RELAY CHAT) INCIDÊNCIA EM PROVA: baixíssima Protocolo  da  Camada  de  Aplicação, ele  é  utilizado  basicamente  para  bate-papo  e  troca de arquivos, permitindo uma conversa em grupo ou privada. Galera, falar desse protocolo até me emociona! Quem é mais antigo sabe que antigamente a única maneira de falar com outra pessoa era  por  meio  de  um  telefone.  Quando  eu,  com  uns  oito  anos  de  idade,  vi  um  Cliente  IRC  pela primeira vez e descobri que era possível falar com outra pessoa, eu achei sensacional!

O Cliente IRC mais comum era o mIRC! Era lento e feio, mas para quem não tinha nada, era uma das melhores coisas do mundo. Crianças, eu vos apresento o mIRC:



(Polícia Federal – 2000) O  Internet  Relay  Chat  permite  que  diversas  pessoas realizem comunicação on-line por meio da Internet.
_______________________ Comentários: conforme vimos em aula, questão perfeita (Correto).







Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






55
105
RESUMO

MODELO OSI
Abstração teórica, uma referência conceitual para entender como se dá o fluxo de dados entre computadores em uma rede. Ele não especifica ou prescreve protocolos para cada camada, mas é possível identificar quais protocolos correspondem à função de cada camada – por isso, vocês verão exemplos de protocolos abaixo.



ARQUITETURA TCP/ip
Trata-se  de  um  conjunto  de  camadas  e  protocolos  para  conectar  várias  redes  diferentes  de  maneira  uniforme.
Pessoal, como nós vimos no início da aula, esse é o conjunto de protocolos padrão da internet – se você quiser ter acesso à internet, terá que utilizar os protocolos prescritos pela Arquitetura TCP/IP.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






56
105

PROTOCOLO PORTA DESCRIÇÃO IP
-
Protocolo da Camada de Rede que permite a comunicação entre duas ou mais máquinas em rede para encaminhamento dos dados.

ICMP -
Protocolo da Camada de Internet/Rede que é utilizado para comunicar a ocorrência de situações  anormais  na  transferência  de  um  datagrama,  gerando  relatórios  de  erros  à fonte original, etc.
ARP -
Protocolo da Camada de Rede que é responsável por manter uma tabela de conversão de endereços lógicos (IP – Camada de Rede) em endereços físicos (MAC – Camada de Enlace).
TCP -
Protocolo da Camada de Transporte que permite o controle de transmissão confiável, entrega na sequência correta e verificação de erros dos pacotes de dados.

UDP
-
Protocolo da Camada de Transporte que fornece um serviço de entrega sem conexão e rápido, porém não confiável.

SMTP 25/587
Protocolo da Camada de Aplicação que é responsável pelo envio de e-mail através da rede. POP e IMAP recuperam e-mails de um Servidor de E-Mail – SMTP envia e-mails para um Servidor de E-Mail.
POP3 110
Protocolo da  Camada  de  Aplicação  que  foi  criado  como  uma  forma  simplificada  para receber, baixar (fazer o download) e deletar mensagens de um Servidor de E-Mail.

IMAP
143
Protocolo  da  Camada  de  Aplicação  projetado  para  nos  livrar  dos  limites  de  envio  e recebimento  de  e-mail  de  um  único  Cliente  de  E-Mail.  Permite  visualizar  e-mails  a qualquer momento de diversos dispositivos.
DHCP
67/68
Protocolo da Camada de Aplicação que configura dinamicamente endereços de rede.
Em uma rede, pode ser necessário que um mesmo Endereço IP possa ser utilizado em diferentes dispositivos em momentos distintos.
DNS
53
Protocolo da Camada de Aplicação que é responsável por atribuir endereços léxicos aos recursos da rede. Busca transformar endereços numéricos em nomes amigáveis, mais compreensíveis por humanos.
HTTP
80
Protocolo da Camada de Aplicação que é utilizado em programas de navegação para acessar páginas web. É responsável pela transferência, formatação e apresentação de páginas web com conteúdo multimídia.
HTTPS
443
Protocolo  da  Camada  de  Aplicação  que  tem  a  mesma  finalidade  do  HTTP,  mas  ele realiza  transferências  de  forma  segura  e  criptografada,  oferecendo  autenticação  e integridade às páginas de um Servidor Web.
FTP 20/21
Protocolo da Camada de Aplicação que é responsável pela realização de transferências de arquivos entre um Cliente FTP e um Servidor FTP.

TELNET 23
Protocolo da Camada de Aplicação que permite conectar dois computadores de forma que um usuário consiga efetuar login em outro computador através da rede de forma remota.
SSH 22
Protocolo  da  Camada  de  Aplicação  que  é  um  protocolo  de  acesso  remoto  que  utiliza autenticação  de  chave  pública  e  oferece  suporte  à  compressão  de  dados  para  a execução de aplicações com interfaces gráficas.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






57
105
IRC 194
Protocolo da Camada de Aplicação que é utilizado basicamente para bate-papo e troca de arquivos, permitindo uma conversa em grupo ou privada.


S M T P
SUA MENSAGEM TÁ  PARTINDO 
D N S
DÁ NOME AO SITE

TELNET SSH
NÃO! NÃO TEM CRIPTOGRAFIA SIM! TEM CRPTOGRAFIA 

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






58
105
MAPA MENTAL

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






59
105

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






60
105
QUESTÕES COMENTADAS – BANCAS DIVERSAS 1. (CONSULPLAN / Prefeitura de Patos de Minas – 2015) Assinale a alternativa que se trata de um protocolo de internet de transferência de arquivo, bastante rápido e versátil utilizado.

a) FTP.
b) HTTP.
c) HTM.
d) HTML.

Comentários:

(a) Correto, esse é um protocolo de transferência de arquivos; (b) Errado, esse é um protocolo de transferência de hipertexto; (c) Errado, isso não é um protocolo; (d) Errado, isso não é um protocolo – trata-se de uma linguagem de marcação de hipertexto.

Gabarito: Letra A

2. (ESAF / Ministério da Fazenda – 2013)  Para  o  funcionamento  da  Internet,  há  um  sistema  de gerenciamento  de  nomes  hierárquico  e  distribuído,  que  resolve  nomes  de  domínios  em endereços de rede (IP), que é o:

a)   POP3
b)  DNS
c)   HTTP
d)  HTTPS
e)   SMTP

Comentários:

A  questão  trata  do  DNS!  Ele  busca  transformar  endereços  numéricos  em  nomes  de  domínios amigáveis,  mais  compreensíveis  para  humanos  e  mais fáceis  de  memorizar.  Ele  apresenta  uma estrutura hierárquica e distribuída, em que seu espaço de nomes é dividido em vários servidores de domínio baseado em níveis.

Gabarito: Letra B

3. (ESAF / Ministério da Fazenda – 2013)  Um  exemplo  de  protocolo  de  transporte  utilizado  na Internet é o protocolo:

a)   XTP
b)  TPP
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






61
105
c)   UDP
d)  TRP
e)   HTTP

Comentários:

Os protocolos mais comuns da Camada de Transporte são: TCP (Transmission Control Protocol) e UDP (User Datagram Protocol).

Gabarito: Letra C

4. (CONSULPLAN / Prefeitura de Cantagalo – 2013) O  Outlook  Express  é  um  aplicativo  para gerenciamento de e-mail, porém, para enviar e receber, são necessárias algumas configurações, como as portas dos protocolos POP e SMTP. As portas dos protocolos POP e SMTP configuradas no Outlook Express são, respectivamente, 
a)   25 e 115.
b)  110 e 587.
c)   466 e 25.
d)  587 e 965.
e)   993 e 587.

Comentários:

PROTOCOLO (CAMADA DE APLICAÇÃO) PROTOCOLO (CAMADA DE TRANSPORTE) NÚMERO DA PORTA HTTP TCP 80
HTTPS
TCP 443
POP3 TCP 110
SMTP TCP 25/587
IMAP3
TCP 220
IMAP4 TCP 143
FTP
TCP 20/21
TELNET
TCP 23
SSH TCP 22
DNS
TCP/UDP 53
DHCP UDP 67/68
IRC TCP 194
SNMP
UDP 161/162

Dessa forma, o SMTP utiliza a Porta 25 ou 587 (essa última, mais segura) e o POP3 utiliza a Porta 110.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






62
105
Gabarito: Letra B

5. (ESAF / Ministério da Fazenda – 2012) O Correio Eletrônico é um método que permite compor, enviar e receber mensagens através de sistemas eletrônicos de comunicação. O termo e-mail é aplicado aos sistemas que utilizam a Internet e são baseados no protocolo:

a)   SNMP.
b)  SMTP.
c)   Web.
d)  HTTP.
e)   HTTPS.

Comentários:

A questão trata do SMTP (Simple Mail Transfer Protocol). Esse é o protocolo utilizado pelos clientes de e-mail para enviar correio eletrônico de um host a outro.

Gabarito: Letra B

6. (ESAF  /  Ministério  da  Fazenda  –  2012) O  componente  mais  proeminente  da  Internet  é  o Protocolo  de  Internet  (IP),  que  provê  sistemas  de  endereçamento  na  Internet  e  facilita  o funcionamento da Internet nas redes. O IP versão 4 (IPv4) é a versão inicial usada na primeira geração da Internet atual e ainda está em uso dominante. Ele foi projetado para endereçar mais de 4,3 bilhões de computadores com acesso à Internet. No entanto, o crescimento explosivo da Internet levou à exaustão de endereços IPv4. Uma nova versão de protocolo foi desenvolvida, denominada:

a)   IPv4 Plus.
b)  IP New Generation.
c)   IPV5.
d)  IPv6.
e)   IPv7.

Comentários:

O nome da nova versão do protocolo IP é IPv6 – nenhum dos outros nomes faz sentido!

Gabarito: Letra D

7. (ESAF / Ministério da Fazenda – 2012) Quando um visitante de um sítio Web se conecta a um servidor  que  está  utilizando  um  protocolo  específico  de  segurança,  ele  irá  notar,  na  barra  de endereços,  que  o  protocolo  de  comunicação  passa  a  ser  https://  (no  lugar  do  http://  padrão).
Além disso, a maioria dos browsers (como o Internet Explorer por exemplo) mostram no browser Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






63
105
o desenho de um cadeado. Quando este cadeado está sendo mostrado, o usuário passa a ter a tranquilidade  de  saber  que  as  informações  fornecidas  àquele  Website  não  poderão  ser interceptadas no seu trajeto. Este protocolo específico de segurança é o:

a)   WebSec
b)  HTTP
c)   HTML
d)  SSL
e)   TCP/IP

Comentários:

Quando um endereço começa com https:// significa que o protocolo que está sendo utilizado é o HTTPS (HyperText Transfer Protocol Secure) e, portanto, significa que o protocolo é seguro. HTTPS é o protocolo HTTP de forma segura, pois utiliza o protocolo TLS ou SSL para criptografia dos dados assim como certificados digitais para garantia de autenticidade.

Gabarito: Letra D

8. (IBADE / IPERON – 2017) Ao  utilizar  um  software  de  correio  eletrônico,  um  usuário  precisou configurar  o  funcionamento  do  protocolo  responsável  pelo  envio  de  e-mail  através  da  rede.
Nesse caso, ele acessou a configuração do protocolo:

a) WAP.
b) SMTP.
c) POP.
d) IMAP.
e) ARP.

Comentários:

(a)  Errado.  WAP  (Wireless  Application  Protocol)  é  um  protocolo  para  aplicações  que  utilizam comunicações de dados digitais sem fio;

(b) Correto. SMTP (Simple Mail Transfer Protocol) é um protocolo para envio de correio eletrônico pela Internet;

(c)  Errado.  POP  (Post Office Protocol)  é  um  protocolo  utilizado  no  acesso  remoto  a  uma  caixa  de correio eletrônico que permite o recebimento local de mensagens;

(d) Errado. IMAP (Internet Message Access Protocol) é um protocolo de gerenciamento de correio eletrônico que permite o recebimento de mensagens localmente ou remotamente;

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






64
105
(e) Errado. ARP (Address Resolution Protocol) é um protocolo de resolução de endereços lógicos (IP) para endereços físicos (MAC).

Gabarito: Letra B

9. (IBADE / PREVES – 2017) Um administrador de rede configurou as contas de e-mail dos usuários de uma empresa de modo a permitir que o status das mensagens recebidas seja igual tanto no servidor  como  no  aplicativo  de  e-mail  utilizado  pelos  usuários;  que  haja  sincronia  dessas mensagens,  mantendo-se  a  conexão,  para  que  as  alterações  e  as  novas mensagens  recebidas no servidor sejam atualizadas quase que em tempo real no aplicativo de e-mail do usuário e que se mantivessem as duas cópias, tanto no servidor, quanto no aplicativo de e-mail. Para isso, esse administrador configurou o protocolo de recepção das mensagens de cada usuário como sendo o protocolo:

a) ARP
b) SMTP
c) FTP
d) IMAP
e) POP

Comentários:

(a) Errado. ARP (Address Resolution Protocol) é um protocolo de resolução de endereços lógicos (IP) para endereços físicos (MAC).

(b)  Errado.  SMTP  (Simple Mail Transfer Protocol)  é  um  protocolo  para  envio  de  correio  eletrônico pela Internet;

(a)   Errado.   FTP   (File  Transfer  Protocol)   é   um   protocolo   para   transferência   de   arquivos (download/upload);

(d) Correto. IMAP (Internet Message Access Protocol) é um protocolo de gerenciamento de correio eletrônico que permite o recebimento de mensagens localmente ou remotamente;

(c)  Errado.  POP  (Post  Office  Protocol)  é  um  protocolo  que  permite  o  recebimento  local  de mensagens, mas não permite a sincronização de mensagens.

Gabarito: Letra D

10. (FUNRIO / Câmara Municipal de Nova Iguaçu – 2016) Dois tipos de protocolos que atendem de forma direta aos serviços de correio eletrônico na internet são os protocolos:

a) HTTP e NNTP.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






65
105
b) SMTP e POP3.
c) RARP e ARP.
d) SSL e ICMP.

Comentários:

(a) Errado. HTTP é um protocolo de transferência de hipertexto que permite navegar em páginas na  internet;  NNTP  é  um  protocolo  que  permite  fazer o  download  de  grandes  quantidades  de informações e que é bastante utilizado em grupos de notícia e discussão;

(b)  Correto.  SMTP  é  o  protocolo  utilizado  por  clientes  de  e-mail  para  o  envio  de  mensagens  de correio  eletrônico;  POP3  é  um  protocolo  utilizado  para  receber  mensagens  e  que  permite  o download de mensagens de correio eletrônico do provedor para o computador;

(c) Errado. RARP é um protocolo que possibilita que uma estação conheça um Endereço IP (Lógico) a  partir  de  um  Endereço  MAC  (Físico);  ARP  é  o  protocolo  permite  conhecer  um  Endereço MAC  a partir de uma Endereço IP (Lógico).

(d) Errado. SSL é um protocolo utilizado em conjunto com outros (Ex: HTTP e FTP) para fornecer serviços  de  criptografia  no  tráfego  de  informações.  ICMP  é  um  protocolo  utilizado  para  fornecer relatórios de erro de uma rede 
Gabarito: Letra B

11. (FUNRIO / Câmara Municipal de Nova Iguaçu – 2016) O protocolo utilizado nos navegadores da internet para transmissão dos hipertextos é o:

a) BCP.
b) RARP.
c) HTTP.
d) SNMP.

Comentários:

O  protocolo  utilizado  para  transmissão  de  hipertexto  é  o  HTTP  –  a  sigla  já  dá  a  dica:  HyperText Transfer Protocol.

Gabarito: Letra C

12. (FUNRIO / Câmara Municipal de Tanguá – 2016) As informações que trafegam durante uma navegação pela Internet podem ser facilmente capturadas. Uma forma de garantir seu sigilo é o uso de criptografia, encontrada em sites que usam o seguinte recurso:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






66
105
a) https
b) firewall
c) antivírus
d) antispyware

Comentários:

O protocolo HTTP pode ser utilizado sobre uma camada de criptografia oferecida pelos protocolos TLS/SSL que fornece autenticidade –passando a se chamar HTTPS.

Gabarito: Letra A

13. (FUNRIO  /  CEITEC  –  2012) Na  internet  o  protocolo_________  permite  a  transferência  de mensagens  eletrônicas  dos  servidores  de  _________para  caixa  postais  nos  computadores dos usuários. As lacunas se completam adequadamente com as seguintes expressões:

a) Ftp/ Ftp.
b) Pop3 / Correio Eletrônico.
c) Ping / Web.
d) navegador / Proxy.
e) Gif / de arquivos.

Comentários:

Na internet, o protocolo POP3 permite a transferência de mensagens eletrônicas dos servidores de Correio Eletrônico para caixa postais nos computadores dos usuários.

Gabarito: Letra B

14. (FUNRIO / SEBRAE/PA – 2010) Sobre  o  modelo  cliente/servidor  utilizado  pela  Internet,  qual afirmativa abaixo é a correta?

a) Um servidor SMTP é também conhecido como servidor de saída de e-mails.
b) Um servidor FTP é responsável pelo recebimento de e-mails.
c) Um cliente WWW realiza a função de mediar a comunicação da rede local com a Internet.
d) Um cliente Proxy fornece uma pasta para armazenamento de arquivos em servidores.
e) Um servidor POP serve para envio de arquivos para outros servidores.

Comentários:

(a)  Correto,  ele  é  também  conhecido  como  Servidor  de  Saída;  (b)  Errado,  um  servidor  FTP  é responsável  pelo  envio  e  recebimento  de  arquivos;  (c)  Errado,  essa  é  a  função  de  um  Proxy;  (d) Errado, trata-se do Servidor FTP; (e) Errado, a questão trata do Servidor SMTP.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






67
105

Gabarito: Letra A

15. (FUNRIO / DEPEN – 2009) Ao criar contas de e-mail para conexão numa ferramenta de correio eletrônico  (como  Microsoft  Outlook  Express  ou  Mozilla  Thunderbird),  deve-se  escolher  um protocolo  para  recebimento  de  mensagens.  Qual  das  alternativas  abaixo  serve  para  essa finalidade?

a) FTP
b) POP
c) IP
d) SMTP
e) UDP

Comentários:

(a) Errado, esse é um protocolo de transferência de arquivos; (b) Correto, esse é um protocolo de recebimento de mensagens de correio eletrônico; (c) Errado, esse é um protocolo de roteamento de pacotes; (d) Errado, esse é um protocolo de envio de e-mails; (e) Errado, esse é um protocolo não confiável de transporte.

Gabarito: Letra B

16. (FUNRIO / DEPEN – 2009) Qual tipo de servidor utilizado para converter os nomes digitados na barra de endereços de um navegador para um endereço IP válido?

a) ISP
b) SMTP
c) Proxy
d) DHCP
e) DNS

Comentários:

O servidor utilizado para converter nomes digitados na barra de endereços de um navegador para um endereço IP válido é o Sistema de Nome de Domínio (DNS).

Gabarito: Letra E

17. (FUNRIO / MDIC – 2009) O protocolo HTTP (Hiper Text Transfer Protocol) tem a função básica de:

a) transferir arquivos.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






68
105
b) exibir páginas em formato HTML.
c) traduzir URL em endereços IP.
d) evitar o acesso não autorizado aos recursos de uma rede.
e) criar páginas dinâmicas.

Comentários:

(a) Errado, essa é a função básica do FTP; (b) Correto, essa é a função básica do HTTP; (c) Errado, essa é a função básica do DNS: (d) Errado, essa é a função básica de um Firewall; (e) Errado, essa é a função básica de algumas linguagens de programação.

Gabarito: Letra B

18. (FUNRIO / Ministério da Justiça – 2009) O Protocolo da Internet responsável pelo recebimento de mensagens, copiando-as para o computador é o:

a) SMTP
b) http
c) Webmail
d) FTP
e) POP3

Comentários:

O  protocolo  responsável  pelo  recebimento  de  mensagens, copiando-as  para  o  computador  é  o...
POP3.

Gabarito: Letra E

19. (FUNRIO / Ministério da Justiça – 2009) O protocolo HTTPS é considerado seguro porque:

a) verifica com um AntiSpyware o endereço acessado.
b) escaneia os arquivos procurando por vírus antes de baixá-los.
c) só funciona dentro de uma Intranet.
d) utiliza criptografia.
e) impede o uso de Spoofing.

Comentários:

(a) Errado, ele não realiza essa atividade; (b) Errado, ele não realiza essa atividade; (c) Errado, ele funciona  também  na  Internet;  (d)  Correto,  ele  realmente  utiliza  criptografia;  (e)  Errado,  ele  não impede uso de spoofing.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






69
105
Gabarito: Letra D

20. (FUNRIO / SUFRAMA – 2008) No contexto da Internet, qual o significado da sigla DNS?

a) Provedor de serviços de internet através do qual um computador se conecta à internet.
b) Conjunto de protocolos que permitem a comunicação entre computadores.
c) Servidor de rede que controla o acesso dos demais computadores a uma rede.
d) Computador central que traduz nomes de domínios para endereços de protocolo na internet.
e) Sistema que permite localizar os computadores ligados a uma rede pelo seu nome.

Comentários:

(a) Errado, esse é o ISP; (b) Errado, esse é o TCP/IP; (c) Errado, isso seria uma pilha ou arquitetura de  protocolos;  (d)  Correto.  A  sigla  significa  Serviço  de  Nome  de  Domínio,  logo  trata-se  de  um computador central capaz de traduzir nomes de domínios para endereços de protocolo na internet;
(e) Errado, essa é a URL.

Gabarito: Letra D

21. (CS-UFG  /  UFG  –  2017) Um  funcionário  está  acessando  o  site  de  um  dos  fornecedores  da empresa, no endereço http://fornecedor.org/. Em um determinado momento, o site apresenta um formulário solicitando diversas informações. Antes de preencher o formulário, o funcionário quer saber se o site é seguro, no sentido de ter as informações transmitidas por meio de uma conexão criptografada.

Qual endereço indica que o site é seguro?

a) http://siteseguro.org/fornecedor.org/formulario/ b) sec://firewall/fornecedor.org/formulario/ c) https://fornecedor.org/formulario/ d) http://https.fornecedor.org/formulario/ 
Comentários:

O protocolo da camada de aplicação (HTTPS) tem a mesma finalidade do HTTP. Ele é responsável pela transferência, formatação e apresentação de páginas web com conteúdo multimídia (textos, áudio, imagens, etc) entre um servidor e um cliente. No entanto, ele realiza transferências de forma segura e criptografada, oferecendo autenticação e integridade às páginas de um Servidor Web.

Gabarito: Letra C

22. (CS-UFG / UNIRG – 2017) O uso do prefixo “HTTPS” é um dos recursos da Internet que ajudam a garantir o acesso e a navegação entre páginas de maneira protegida.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






70
105

Quando o termo “https:”aparece significa que a comunicação com a página é feita de forma 
a) segura.
b) anônima.
c) prioritária.
d) privilegiada.

Comentários:

Questão bem parecida com a anterior, podemos associar o S da sigla HTTPS à Segurança!

Gabarito: Letra A

23. (CS-UFG  /  APARECIDAPREV  –  2018) Há  sites  na  Internet  que  são  acessados  por  meio  do protocolo HTTPS, como, por exemplo, o site https://cs.ufg.br.

Qual é a função do HTTPS?

a) Tornar mais rápida a navegação pelo site.
b) Bloquear as janelas pop-up.
c) Garantir que o navegador apresente uma única página por aba.
d) Fazer com que os dados sejam transmitidos de forma criptografada.

Comentários:

O protocolo da camada de aplicação (HTTPS) tem a mesma finalidade do HTTP. Ele é responsável pela transferência, formatação e apresentação de páginas web com conteúdo multimídia (textos, áudio, imagens, etc) entre um servidor e um cliente. No entanto, ele realiza transferências de forma segura  e  criptografada,  oferecendo  autenticação  e  integridade  às  páginas  de  um  Servidor  Web.
Sendo assim, ele possui a função de transmitir os dados de forma segura, criptografada.


Gabarito:
Letra D

24. (IADES  /  ARCON  PA  –  2018) [...]  é  um  tipo  de  rede  local  que  utiliza  sinais  de  rádio  para comunicação.

CERT.br. Centro de Estudos, Resposta e Tratamento de Incidentes de Segurança no Brasil. Cartilha de Segurança para Internet. Disponível em:
<https://cartilha.cert.br/livro/cartilha_segurança_internet.pdf>.
Acesso em: 28 jun. 2018.

A definição apresentada refere-se a:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






71
105
a) IP: Internet Protocol.
b) DNS: Domain Name Server.
c) SMTP: Simple Mail Transfer Protocol.
d) URL: Universal Resource Locator.
e) Wi-Fi: Wireless Fidelity.

Comentários:

(a) Errado. O IP é o protocolo de comunicação da Internet responsável por endereçar os dispositivos em uma rede; (b) Errado. O DNS é o sistema e protocolo responsável pela resolução de nomes da Internet,  isto  é,  por  traduzir  os  endereços  IPs  numéricos  em  nomes;  (c)  Errado.  O  SMTP  é  um protocolo utilizado para envios de correio eletrônico; (d) Errado. A URL é o identificador único usado para localizar um recurso na Internet; (e) Correto. O Wi-Fi é a tecnologia composta por um conjunto de especificações (IEEE802.11) para redes locais sem fio (WLAN). A ideia do Wi-Fi é possibilitar a comunicação  de  dispositivos  sem  necessidade  de  cabos,  utilizando  a  propagação  das  ondas  de rádio através de antenas.


Gabarito: Letra E

25. (IDECAN / IPC – 2018) Considerando os recursos que podem ser consumidos ou acessados na Internet, analise as seguintes informações.

I. O FTP é o protocolo utilizado para a transferência de arquivos entre duas máquinas ligadas à Internet.

II. Um correio eletrônico permite a troca de mensagens que um usuário de Internet pode fazer para outras pessoas conectados à Internet.

III
. O HTTP é o protocolo utilizado para controlar a comunicação entre o servidor de Internet e o browser ou navegador.

IV.  O  ICMP  é  o  protocolo  responsável  por  estabelecer a  comunicação  entre  os  computadores emissores e receptores de maneira na qual a informação não se perca na rede.

De acordo com as afirmativas acima, marque a alternativa correta.

a) Apenas as afirmativas I e II estão corretas.
b) Apenas as afirmativas I, II e III estão corretas.
c) Apenas as afirmativas II e III estão corretas.
d) Apenas as afirmativas I, II e IV estão corretas.

Comentários:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






72
105
(I)  Correto,  ele  é  realmente  um  protocolo  para  transferência  de  arquivos  entre  duas  máquinas conectadas à Internet; (II) Correto, ele realmente permite a troca de mensagens entre pessoas na internet; (III) Correto, ele é utilizado para controlar a comunicação a comunicação entre servidor de Internet  e  navegador;  (IV)  Errado,  a  função  do  ICMP  é  fornecer  relatórios  de  erros  e,  não, estabelecer a comunicação.

Gabarito:
Letra B

26. (IDECAN / BANESTES – 2012) Segundo Kurose (2010), o correio eletrônico existe desde o início da  Internet.  Ao  contrário  do  correio  normal,  que  anda  a  passos  lentos,  o  correio  eletrônico  é rápido, fácil de distribuir e barato. Identifique dois protocolos utilizados em correio eletrônico.

a) DNS e http.
b) POP3 e TCP.
c) IMAP e FTP.
d) POP3 e SMTP.
e) SMTP e IP.

Comentários:

(a) Errado, eles não são utilizados em correio eletrônico; (b) Errado, TCP não é utilizado em correio eletrônico; (c) Errado, FTP não é utilizado em correio eletrônico; (d) Correto, ambos são utilizados em correio eletrônico; (e) Errado, IP não é utilizado em correio eletrônico.

Gabarito: Letra D

27. (IESES  /  CRM/SC  –  2017) Considerando  o  cliente  de  e-mails  Microsoft  Outlook,  aponte  o número de porta padrão para o recebimento de mensagens POP3:

a) 587
b) 110
c) 25
d) 443

Comentários:

Essa questão é um pouco decoreba! Vamos relembrar para que servem as portas apresentadas: (a) Porta  587:  utilizada  para  enviar  e-mails  pelo  protocolo  SMTP;  (b)  Porta  110:  utilizada  para  o recebimento  de  e-mails  pelo  protocolo  POP;  (c)  Porta  25:  não  é  mais  utilizada  para  o  envio  de mensagens; (d) Porta 443: utilizada pela navegação com o protocolo HTTPS.

Gabarito:
Letra B

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






73
105
28. (IESES  /  CRMV/SC  –  2017) Uma  das  principais  preocupações  ao  se  realizar  transações eletrônicas  através  da  internet  está  na  segurança  da  comunicação  entre  o  computador  do usuário  e  o  servidor  que  provê  o  produto/serviço.  Esta  segurança  é  proporcionada  pela criptografia dos dados entre as duas partes da comunicação, através de um protocolo específico, que usualmente é representado antes do endereço do site no qual se está navegando. Dentre os protocolos abaixo mencionados, qual representaria uma conexão criptografada entre o cliente e o servidor?

a) wwws
b) https
c) http
d) stp

Comentários:

Galera,  a  questão  pergunta  qual  é  o  protocolo  que  proporciona  segurança  por  criptografia  e  que geralmente é inserido antes do endereço de um site em um navegador. Logo, estamos falando do HTTPS, que é protocolo HTTP com a adição de uma camada de segurança por criptografia.

Gabarito: Letra B

29. (IESES / CRO/SC – 2017) O servidor responsável por traduzir para números IP os endereços de sites que digitamos nos navegadores é o servidor:

a) DNS.
b) IMAP.
c) SMTP.
d) DHCP.

Comentários:

Pessoal, sempre que digitamos o nome de um site em nosso navegador existe um protocolo que “transforma” o texto em códigos, o conhecido IP, que é o verdadeiro responsável pelo acesso das páginas  solicitadas.  Esse  protocolo  é  o  DNS  (Domain  Name  System),  que  possui  a  função  de converter ou traduzir as letras digitadas em número de IP.

Gabarito: Letra A

30. (IESES / CRO/SC – 2016) O  protocolo  responsável  pelo  envio  de  mensagens  eletrônicas  (e- mails) através da internet é o:

a) POP3.
b) SNMP.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






74
105
c) SMTP.
d) FTP.

Comentários:

(a)  Errado,  esse  protocolo  é  responsável  pelo  recebimento  de mensagens  eletrônicas;  (b) Errado, esse  protocolo  é  responsável  pelo  gerenciamento  de redes;  (c)  Correto,  esse  protocolo  é responsável  pelo  envio  de  mensagens  eletrônicas;  (d)  Errado,  esse  protocolo  é  responsável  pela transferência de arquivos.

Gabarito: Letra C

31. (IESES / IGP/SC – 2014) Analise as afirmativas abaixo e assinale a alternativa correta:

I. POP3
II. SMTP
III. FTP
IV. SSH
V. IMAP

a) Apenas as afirmativas II e III são protocolos utilizados no envio ou recebimento de e-mails.
b) As afirmativas I, II e V são protocolos utilizados no envio ou recebimento de e-mails.
c) A afirmativa I é um protocolo utilizado no envio de e-mails.
d) As afirmativas II, III e IV são protocolos utilizados no recebimento de e-mails.

Comentários:

(I) POP3: utilizado para receber mensagens de e-mail; (II) SMTP: utilizado para enviar mensagens de e-mail (Sua Mensagem Está Partindo); (III) FTP: utilizado para a transferência de arquivos; (IV) SSH:  utilizado  para  realizar  a  comunicação  segura  entre  duas  estações  de  trabalho;  (V)  IMAP4:
utilizado  para  o  acesso  online  e  offline  da  caixa  postal.  Dessa  forma,  POP3,  SMTP  e  IMAP4  são utilizados para envio ou recebimento de e-mails.

Gabarito: Letra B

32. (AOCP / Prefeitura de Paranavaí/PR – 2013) Com  relação  a  conceitos  de  Internet  assinale  a alternativa INCORRETA.

a) Navegador de internet é um programa que permite você acessar e navegar entre as páginas de um ou mais sites.

b) Os Cookies possuem como principal função armazenar as preferências dos usuários sobre um determinado site na Internet.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






75
105

c) Download é a saída de arquivos do seu computador para a internet. Os provedores gratuitos de   download   variam   bastante   na   sua   política,   capacidades   e   prazo   de   validade   das transferências.

d) E-mail é uma ferramenta que permite compor, enviar e receber mensagens, textos, figuras e outros arquivos através da Internet.

e) HTTP é um protocolo que permite o funcionamento da interface gráfica na Internet, esta que é a mais conhecida e que permite transmissão de texto, fotos e gráficos de uma maneira simples e rápida.

Comentários:

(a) Correto. Navegador de Internet realmente permite acessar e navegar páginas web; (b) Correto.
Cookies  –  de  fato  –  tem  como  função  principal  armazenar  preferências  dos  usuários  em  sua navegação na internet; (c) Errado. Download Upload é a saída de arquivos do seu computador para a internet; (d) Correto. E-mail realmente é uma ferramenta para compor, enviar e receber e-mails, entre outros; (e) Correto. HTTP é realmente o protocolo que permite o funcionamento da interface gráfica na internet, permitindo a transmissão de texto, fotos, gráficos, etc.

Gabarito: Letra C

33. (AOCP / Prefeitura de Valença/BA – 2016) A base para a comunicação de dados da internet é um  protocolo  da  camada  de  aplicação  do  modelo  OSI, que  é  responsável  por  transferir hipertextos. Esse protocolo é conhecido como:

a) HTML.
b) HTTP.
c) FTP.
d) PHP.
e) www.


Comentários:

(a) Errado, HTML não e um protocolo, mas uma linguagem de marcação; (b) Correto, HTTP é um protocolo  da  camada  de  aplicação  responsável  por  transferir  hipertexto;  (c)  Errado,  FTP  é  um protocolo  da  camada  de  aplicação  responsável  pela  transferência  de  arquivos;  (d)  Errado,  PHP  é uma  linguagem  de  programação;  (e)  Errado,  WWW  é  a  sigla  para  World  Wide  Web,  que  é  um sistema de documentos de hipermídia da internet.

Gabarito: Letra B

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






76
105
34. (AOCP / FUNDASUS – 2015) Em redes de computadores, existem, basicamente, dois modelos de  referência  divididos  em  camadas  e  que  possuem  protocolos  de  comunicação  específicos.
Esses modelos são conhecidos como:

a) OSI e TCP/IP.
b) DHCP e HTTP.
c) IEEE e OSI.
d) Ethernet e IP
e) IANA e TCP.


Comentários:

(a) Correto, ambos são modelos de referência divididos em camadas e que possuem protocolos de comunicação  específicos;  (b)  Errado,  ambos  são  protocolos  de  comunicação  e,  não,  modelos  de referência; (c) Errado, o primeiro é uma instituição profissional de engenharia dedicada ao avanço da tecnologia; (d) Errado, o primeiro é um padrão de arquitetura de redes locais e o segundo é um protocolo de comunicação; (e) Errado, o primeiro é uma organização mundial que supervisiona a atribuição global dos números na Internet e o segundo é um protocolo de comunicação.

Gabarito: Letra A

35. (AOCP / FUNDASUS – 2015) Os protocolos de comunicação são a base da internet. Dentre os protocolos da camada de transporte do modelo TCP/IP, está o protocolo UDP (User Datagram Protocol) que se caracteriza por:

a) não dar garantias que o pacote enviado chegará ao seu destino.
b) ser utilizado pelos sistemas de informação de hipermídia, distribuídos e colaborativos.
c) permitir que um usuário se conecte a um computador rodando o Microsoft Terminal Services.
d)  ser  um  protocolo  de  comunicação  usado  entre  todas  as  máquinas  de  uma  rede  para  o encaminhamento de dados.
e) verificar se os dados são enviados de forma correta, na sequência apropriada e sem erros para o destino.


Comentários:

(a)  Correto,  UDP  realmente  não  dá  garantias  de  entrega  de  pacotes;  (b)  Errado,  o  item  trata  do HTTP; (c) Errado, o item trata do RDP; (d) Errado, o item trata do IP; (e) Errado, o item trata do TCP.

Gabarito: Letra A

36. (CONSULPLAN / TRT - 13ª Região / PB – 2012) A conexão entre computadores e meios físicos de dados é realizada através do dispositivo placa de rede. Toda placa de rede recebe um número único para a sua identificação denominado:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






77
105

a) IPV4.
b) IPV6
c) MAC.
d) RASH.
e) BIT.

Comentários:

Toda placa de rede recebe um número único para a sua identificação denominado Endereço MAC (Media Access Control). Galera, não confundam Endereço MAC com Endereço IP – o primeiro trata do endereço físico e o segundo trata do endereço lógico.

Gabarito:
Letra C

37. (ITAME / Prefeitura de Aragoiânia – 2016) Assinale a alternativa correta:

a) POP3 é um protocolo de envio de e-mails.
b) FTP é um protocolo utilizado para transferência de arquivos.
c) SMTP é um protocolo de recebimento de emails.
d) HTTPS é um protocolo criado somente para trafegar voz na internet.

Comentários:

(a)  Errado.  POP3  é  um  protocolo  de  recebimento  de  e-mails;  (b)  Correto.  FTP  é  realmente  um protocolo utilizado para transferência de arquivos; (c) Errado. SMTP é um protocolo de envio de e- mails; (d) Errado. HTTPS é um protocolo seguro para transferência de hipertexto.

Gabarito:
Letra B

38. (FACET / Prefeitura de Sobrado – 2016) Qual  é  o  protocolo  utilizado  para  transferência  de hipertextos na camada de aplicação segundo o modelo OSI?

a) FPT
b) TCP/IP
c) Proxy
d) DHCP
e) HTTP

Comentários:

(a) Errado, esse protocolo não existe; (b) Errado, TCP/IP não é um protocolo – é uma arquitetura ou pilha  de  diversos  protocolos;  (c)  Errado,  proxy  é  um  intermediário  de  requisições  de  clientes  e Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






78
105
servidores;  (d)  Errado,  DHCP  é  um  protocolo  da  camada  de  aplicação,  mas  é  responsável  pela concessão  de  endereço  IP  em  uma  rede;  (e)  Correto, esse  protocolo  é  realmente  utilizado  para transferência de hipertextos (HTTP – HyperText Transfer Protocolo).

Gabarito: Letra E

39. (AOCP  /  ITEP-RN  –  2018) Em  relação  à  transferência  de  arquivos  pela  internet,  assinale  a alternativa correta.

a)  Quando  uma  pessoa  envia  um  arquivo  de  seu  computador  para  um  site  na  internet,  a operação de transferência que está sendo executada é conhecida como Download.

b)  FTP  é  um  protocolo  que  pode  ser  utilizado  para  transferir  arquivos  entre  computadores conectados à internet.

c)  Podemos  considerar  os  termos  Upload  e  Download  como  análogos,  ou  seja,  possuem  o mesmo significado.

d) O protocolo FTP é utilizado exclusivamente para se realizar o acesso a websites na internet.

e) O termo Upload se refere à velocidade na qual um computador conectado à internet consegue receber os dados de um website qualquer.

Comentários:

(a) Errado, está sendo executado um Upload; (b) Correto, o Protocolo FTP é comumente utilizado para  transferência  de  arquivos  entre  computadores  via  internet;  (c)  Errado,  eles  possuem significados diametralmente opostos: download para recebimento de dados e upload para envio de dados;  (d)  Errado,  ele  é  utilizado  exclusivamente  para  a  transferência  de  arquivos na  internet  –  a questão  trata  do  Protocolo  HTTP;  (e)  Errado,  upload  é  a  operação  de  transferência  de  dados  do computador do usuário para um servidor na internet.

Gabarito:
Letra B

40. (CONSESP / Prefeitura de Quedas do Iguaçu - PR – 2012) A  transferência  de  arquivos  entre dois computadores ligados à Internet é realizada pelo protocolo denominado de:

a) FUNDNET
b) IP
c) WWW
d) FTP

Comentários:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






79
105

A  transferência  de  arquivos  entre  dois  computadores  ligados  à  internet  é  realizada  por  meio  do Protocolo FTP (File Transfer Protocol).

Gabarito: Letra D

41. (PR-4 / UFRJ – 2012) O  protocolo  da  Internet  utilizado  principalmente  para  transferência  de arquivos entre dois computadores é o:

a) FTP;
b) DHCP;
c) NTP;
d) DNS;
e) WINS.

Comentários:

A  transferência  de  arquivos  entre  dois  computadores  ligados  à  internet  é  realizada  por  meio  do Protocolo FTP (File Transfer Protocol).

Gabarito: Letra A

42. (IFSP / IFSP – 2012) Assinale a alternativa que informa o protocolo usado para transferência de arquivos entre computadores ligados na Internet.

a) IMAP.
b) FTP.
c) SMTP.
d) DHCP.
e) SNMP.

Comentários:

A  transferência  de  arquivos  entre  dois  computadores  ligados  à  internet  é  realizada  por  meio  do Protocolo FTP (File Transfer Protocol).

Gabarito: Letra B

43. (EPL / Câmara Municipal de Paraíso do Norte/PR – 2013) Na  internet  o  termo  UPLOAD  é designado para:

a) Enviar um arquivo para um local na internet, como por exemplo um disco virtual.
b) Baixar um arquivo de um servidor ou disco virtual.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






80
105
c) Compactar um arquivo d) Enviar uma mensagem instantânea e) Carregar uma página da web no navegador 
Comentários:

Upload é o termo utilizado quando se deseja enviar um arquivo para um local na internet – como um disco virtual de armazenamento em nuvem.

Gabarito:
Letra A

44. (IBFC / ABDI – 2008) "____________ é a transferência de dados de um computador remoto para um computador local, e o inverso chama-se ____________".

Complete a frase acima respectivamente com as seguintes palavras:

a) upload / download b) download / upload c) upload / reload
d) reload / download 
Comentários:

A transferência de dados de um computador remoto para um computador local se chama download e o inverso é um upload.

Gabarito:
Letra B

45. (FADESP / Prefeitura de Conceição do Araguaia/PA – 2009) O  ato  de  transferir  arquivos  do computador de um usuário para a Web é denominado:

a) Download.
b) Upload.
c) NumLoad.
d) EndLoad.


Comentários:

O ato de transferir arquivos do computador de um usuário para a web é denominado Upload. É a ação   de enviar   dados de   um   computador   local   para   um   computador   ou   servidor   remoto, geralmente através da internet.

Gabarito:
Letra B
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






81
105

46. (UNA  /  Prefeitura  de  São  Sebastião/RS  –  2015) O  processo  pelo  qual  um  programa  ou documento é baixado da Internet para o computador do usuário é conhecido como:

a) Download
b) Backup
c) Upload
d) Update


Comentários:

Falou em programa ou documento baixado da internet, trata-se de download.

Gabarito:
Letra A

47. (CAIP / Câmara Municipal de São Caetano do Sul/SP – 2014) Na Internet, a transferência de dados de um computador externo ou servidor para seu computador local é conhecida como:

a) Download.
b) Upload.
c) Peopleware.
d) Downgrade.


Comentários:

A transferência de dados de um computador externo ou servidor para seu computador local nada mais é que um download.

Gabarito:
Letra A

48.(CONSULPAM  /  Prefeitura  de  Tarrafas/CE  –  2015) Marcos  transferiu  um  arquivo  do  seu computador para a Web. Essa ação é denominada:

a) Upload
b) Download
c) EndLoad
d) NumLoad


Comentários:

Se Marcos transferiu um arquivo do seu computador para web, ele realizou um upload.

Gabarito:
Letra A
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






82
105

49. (SELECON / Prefeitura de Cuiabá/MT – 2015) Um internauta baixou o arquivo ccleaner-5-38- 6357.exe do site do fabricante na internet para viabilizar a instalação do software Ccleaner em seu computador. O procedimento de baixar um arquivo da internet para o computador de um usuário é conhecido pelo seguinte termo:

a) download
b) downsize
c) upload
d) upsize


Comentários:

O procedimento de baixar um arquivo da internet para o computador de um usuário é conhecido pelo termo: download.

Gabarito: Letra A


50. (CEPERJ / FSC – 2014) Atualmente,  é  comum  baixar  softwares  de  sites  da  internet  como  as atualizações  de  antivírus  e,  paralelamente,  enviar arquivos  para  sites  de  hospedagem  web.
Essas atividades são conhecidas, respectivamente, por:

a) download e upload b) upload e download c) download e downlink d) downlink e uplink e) uplink e downlink 

Comentários:

Baixar  softwares  de  sites  da  internet  é  um  exemplo de  download;  enviar  arquivos  para  sites  de hospedagem web é um exemplo de upload.

Gabarito: Letra A

51. (CPCON / Prefeitura de Catolé do Rocha/PB – 2015) O  envio  e  o  recebimento  de  dados  na internet, entre duas máquinas, constituem, respectivamente, em:

a) Downgrade e upgrade b) Upload e download c) Downfile e upfile d) Upgrade e downgrade Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






83
105
e) Download e upload 
Comentários:

O envio de dados na internet entre duas máquinas é um upload; o recebimento de dados na internet entre duas máquinas é um download.

Gabarito: Letra B

52. (FUNCAB  /  SESAU-RO  –  2009) Qual  o  nome  da  função  que  permite  ao  usuário  copiar  um arquivo de um site da Internet para o seu próprio computador?

a) Upload.
b) Transfer.
c) Download.
d) Copy.
e) Paste.


Comentários:

A cópia de um arquivo de um site da internet para o seu computador pessoal é um download.

Gabarito: Letra C

53. (FEPESE  /  UFFS  –  2012) Como  é  denominado  o  ato  de  baixar  dados  da  internet  para  um computador?

a) Reload.
b) Download.
c) Upload.
d) Formatação.
e) Refresh.


Comentários:

O ato de baixar dados da internet para um computador é denominado download.

Gabarito: Letra B

54. (BIO-RIO / Prefeitura de Três Rios-RJ – 2015) Redes  de  computadores  possibilitam  a  uma máquina  conectada  à  internet  baixar  de  sites  especializados  as  atualizações  de  programas antivírus,  como  o  Avast,  por  exemplo.  No  contexto  da  informática,  essa  atividade  recebe  a seguinte denominação:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






84
105

a) download
b) downsize
c) upgrade
d) upload
e) upsize

Comentários:

A atividade de baixar de sites especializados as atualizações de programas é também chamada de...
download.

Gabarito: Letra A

55. (AOCP / FUNDASUS – 2015) Acerca dos termos utilizados na internet, quando anexamos um arquivo a uma mensagem de e-mail, estamos realizando uma operação de:

a) ROM.
b) Boot.
c)  Hashtag.
d) Upload.
e)  UML.

Comentários:

Ao anexar arquivos a uma mensagem de e-mail, estamos realizando a atividade de upload.

Gabarito: Letra D

56. (NC-UFPR / COPEL – 2013) No contexto da Internet, como é comumente chamada a ação de transferir um ou mais arquivos de um computador local para um servidor remoto?

a) Download.
b) Upload.
c) Downstream.
d) Baixar.
e) Gravar.

Comentários:

A  ação  de  transferir  um  ou  mais  arquivos  de  um  computador  local  para  um  servidor  remoto  é chamada de... upload.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






85
105
Gabarito: Letra B

57. (ZAMBINI / PRODESP – 2010) A transferência de um arquivo de um computador local para um servidor na Internet é denominada(o):

a) Casting.
b) Upload.
c) Download.
d) Backup.
e) SMTP.

Comentários:

A   transferência   de   um   arquivo   de   um   computador   local   para   um   servidor   na   Internet   é denominada... upload.

Gabarito:
Letra B

58. (UEM / UEM – 2017) É possível ao usuário transferir um arquivo de um site da Internet para o seu próprio computador. Esta função é chamada de:

a)  E-book.
b) Upload.
c)  Lista.
d) Download.
e) Copy.

Comentários:

A  transferência  de  um  arquivo  de  um  site  da  Internet  para  o  seu  próprio  computador  é  também chamada de download.

Gabarito: Letra D

59. (IFSP / IFSP – 2012) O  ato  de  transferir  um ou  mais  arquivos  de  um  servidor  remoto  para um computador através da Internet é chamado de:

a) formatação.
b) relocação.
c) upload.
d) editoração.
e) download.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






86
105
Comentários:

O  ato  de  transferir  um  ou  mais  arquivos  de  um  servidor  remoto  para  um  computador  através  da Internet é chamado de... download.

Gabarito: Letra E

60. (FUNCAB / SEAD-PB – 2012) O recurso que permite transferir um arquivo da Internet para um computador ou para um dispositivo de armazenamento de dados é chamado de:

a) Recuperar fontes.
b) Print.
c) Hyperlink.
d) Download.
e) Upload.

Comentários:

O  recurso  que  permite  transferir  um  arquivo  da  Internet  para  um  computador  ou  para  um dispositivo de armazenamento de dados é chamado de... donwload.

Gabarito:
Letra D

61. (AOCP / Colégio Pedro II – 2013) Um usuário de um computador copiou uma foto de um site (servidor web) para seu computador. O processo feito por esse usuário foi:

a) Upload.
b) Compactação de arquivo.
c) Phishing.
d) Backup.
e) Download.

Comentários:

O  processo  feito pelo  usuário  de  copiar  uma  foto  de  um  servidor  remoto  para  seu  computador  é chamado de... download.

Gabarito: Letra E

62. (LEGATUS  /  Câmara  Municipal  de  Bertolínia/PI  –  2013) “____________  significa  fazer  a transferência  de  algum  arquivo,  como  imagem,  vídeo ou  documento,  armazenado  em  um servidor remoto para o computador local”. A alternativa que preenche corretamente a lacuna em branco é:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






87
105

a) Upload
b) Plug-in
c) Browser
d) Pop-up
e) Download

Comentários:

Fazer a transferência de algum arquivo, como imagem, vídeo ou documento, armazenado em um servidor remoto para o computador local é chamado de... download.

Gabarito: Letra E

63. (KLC / Prefeitura de Mamborê/PR – 2016) Você precisa enviar sua foto para o perfil de usuário na home page da empresa. Você fará este procedimento acessando a página de novo usuário da empresa  que  o  contratou,  com  seu  login  e  senha.  Este  processo  de  envio  de  arquivos  de  uma máquina local para um servidor de intranet ou internet é comumente chamado de:

a) Reload de página.
b) Upload.
c) Download.
d) Link.
e) Logon.

Comentários:

O processo de envio de arquivos de uma máquina local para um servidor de intranet ou internet é comumente chamado de... upload.

Gabarito:
Letra B

64. (IBGP / CISSUL-MG – 2017) Ao  se  utilizar  a  internet,  depara-se  com  diversos  termos,  dentre esses, o UPLOAD que significa:

a)  A  ação  de  enviar  dados  de  um  computador  local  para  um  computador  ou  servidor  remoto, geralmente através da internet.
b) O ato de transferir (baixar) um ou mais arquivos de um servidor remoto para um computador local.
c) O ato de enviar um arquivo para impressão.
d) A ação de realizar buscas na internet.

Comentários:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






88
105

(a) Correto, essa é a definição clássica de upload; (b) Errado, essa é a definição clássica de download;
(c) Errado, isso não é upload; (d) Errado, isso não é upload.

Gabarito: Letra A

65. (CONSULPLAN / Prefeitura de Congonhas-MG – 2010) Sobre  os  conceitos  de  utilização  da internet,  a  transferência  de  dados  de  um  computador  remoto  para  um  computador  local, denomina-se:

a) Web Browser.
b) Download.
c) Transfer Web.
d) Upload.
e) Transceiver Web.

Comentários:

A  transferência  de  dados  de  um  computador  remoto  para  um  computador  local,  denomina-se...
download.

Gabarito:
Letra B

66. (AOCP / FUNDASUS – 2015) Acerca dos termos utilizados na internet, quando baixa-se um arquivo, realiza-se:

a) uma desfragmentação de disco.
b) uma compactação em seu tamanho físico.
c) uma compactação em seu tamanho lógico.
d) um UPLOAD.
e) um DOWNLOAD.

Comentários:

O procedimento de baixar um arquivo é denominado... download.

Gabarito: Letra E






Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






89
105
LISTA DE QUESTÕES - BANCAS DIVERSAS 1. (CONSULPLAN / Prefeitura de Patos de Minas – 2015) Assinale a alternativa que se trata de um protocolo de internet de transferência de arquivo, bastante rápido e versátil utilizado.

a) FTP.
b) HTTP.
c) HTM.
d) HTML.

2. (ESAF / Ministério da Fazenda – 2013)  Para  o  funcionamento  da  Internet,  há  um  sistema  de gerenciamento  de  nomes  hierárquico  e  distribuído,  que  resolve  nomes  de  domínios  em endereços de rede (IP), que é o:

a)   POP3
b)  DNS
c)   HTTP
d)  HTTPS
e)   SMTP

3. (ESAF / Ministério da Fazenda – 2013)  Um  exemplo  de  protocolo  de  transporte  utilizado  na Internet é o protocolo:

a)   XTP
b)  TPP
c)   UDP
d)  TRP
e)   HTTP

4. (CONSULPLAN / Prefeitura de Cantagalo – 2013) O  Outlook  Express  é  um  aplicativo  para gerenciamento de e-mail, porém, para enviar e receber, são necessárias algumas configurações, como as portas dos protocolos POP e SMTP. As portas dos protocolos POP e SMTP configuradas no Outlook Express são, respectivamente, 
a)   25 e 115.
b)  110 e 587.
c)   466 e 25.
d)  587 e 965.
e)   993 e 587.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






90
105
5. (ESAF / Ministério da Fazenda – 2012) O Correio Eletrônico é um método que permite compor, enviar e receber mensagens através de sistemas eletrônicos de comunicação. O termo e-mail é aplicado aos sistemas que utilizam a Internet e são baseados no protocolo:

a)   SNMP.
b)  SMTP.
c)   Web.
d)  HTTP.
e)   HTTPS.

6. (ESAF  /  Ministério  da  Fazenda  –  2012) O  componente  mais  proeminente  da  Internet  é  o Protocolo  de  Internet  (IP),  que  provê  sistemas  de  endereçamento  na  Internet  e  facilita  o funcionamento da Internet nas redes. O IP versão 4 (IPv4) é a versão inicial usada na primeira geração da Internet atual e ainda está em uso dominante. Ele foi projetado para endereçar mais de 4,3 bilhões de computadores com acesso à Internet. No entanto, o crescimento explosivo da Internet levou à exaustão de endereços IPv4. Uma nova versão de protocolo foi desenvolvida, denominada:

a)   IPv4 Plus.
b)  IP New Generation.
c)   IPV5.
d)  IPv6.
e)   IPv7.

7. (ESAF / Ministério da Fazenda – 2012) Quando um visitante de um sítio Web se conecta a um servidor  que  está  utilizando  um  protocolo  específico  de  segurança,  ele  irá  notar,  na  barra  de endereços,  que  o  protocolo  de  comunicação  passa  a  ser  https://  (no  lugar  do  http://  padrão).
Além disso, a maioria dos browsers (como o Internet Explorer por exemplo) mostram no browser o desenho de um cadeado. Quando este cadeado está sendo mostrado, o usuário passa a ter a tranquilidade  de  saber  que  as  informações  fornecidas  àquele  Website  não  poderão  ser interceptadas no seu trajeto. Este protocolo específico de segurança é o:

a)   WebSec
b)  HTTP
c)   HTML
d)  SSL
e)   TCP/IP

8. (IBADE / IPERON – 2017) Ao  utilizar  um  software  de  correio  eletrônico,  um  usuário  precisou configurar  o  funcionamento  do  protocolo  responsável  pelo  envio  de  e-mail  através  da  rede.
Nesse caso, ele acessou a configuração do protocolo:

a) WAP.
b) SMTP.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






91
105
c) POP.
d) IMAP.
e) ARP.

9. (IBADE / PREVES – 2017) Um administrador de rede configurou as contas de e-mail dos usuários de uma empresa de modo a permitir que o status das mensagens recebidas seja igual tanto no servidor  como  no  aplicativo  de  e-mail  utilizado  pelos  usuários;  que  haja  sincronia  dessas mensagens,  mantendo-se  a  conexão,  para  que  as  alterações  e  as  novas mensagens  recebidas no servidor sejam atualizadas quase que em tempo real no aplicativo de e-mail do usuário e que se mantivessem as duas cópias, tanto no servidor, quanto no aplicativo de e-mail. Para isso, esse administrador configurou o protocolo de recepção das mensagens de cada usuário como sendo o protocolo:

a) ARP
b) SMTP
c) FTP
d) IMAP
e) POP

10. (FUNRIO / Câmara Municipal de Nova Iguaçu – 2016) Dois tipos de protocolos que atendem de forma direta aos serviços de correio eletrônico na internet são os protocolos:

a) HTTP e NNTP.
b) SMTP e POP3.
c) RARP e ARP.
d) SSL e ICMP.

11. (FUNRIO / Câmara Municipal de Nova Iguaçu – 2016) O protocolo utilizado nos navegadores da internet para transmissão dos hipertextos é o:

a) BCP.
b) RARP.
c) HTTP.
d) SNMP.

12. (FUNRIO / Câmara Municipal de Tanguá – 2016) As informações que trafegam durante uma navegação pela Internet podem ser facilmente capturadas. Uma forma de garantir seu sigilo é o uso de criptografia, encontrada em sites que usam o seguinte recurso:

a) https
b) firewall
c) antivírus
d) antispyware

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






92
105
13. (FUNRIO  /  CEITEC  –  2012) Na  internet  o  protocolo_________  permite  a  transferência  de mensagens  eletrônicas  dos  servidores  de  _________para  caixa  postais  nos  computadores dos usuários. As lacunas se completam adequadamente com as seguintes expressões:

a) Ftp/ Ftp.
b) Pop3 / Correio Eletrônico.
c) Ping / Web.
d) navegador / Proxy.
e) Gif / de arquivos.

14. (FUNRIO / SEBRAE/PA – 2010) Sobre  o  modelo  cliente/servidor  utilizado  pela  Internet,  qual afirmativa abaixo é a correta?

a) Um servidor SMTP é também conhecido como servidor de saída de e-mails.
b) Um servidor FTP é responsável pelo recebimento de e-mails.
c) Um cliente WWW realiza a função de mediar a comunicação da rede local com a Internet.
d) Um cliente Proxy fornece uma pasta para armazenamento de arquivos em servidores.
e) Um servidor POP serve para envio de arquivos para outros servidores.

15. (FUNRIO / DEPEN – 2009) Ao criar contas de e-mail para conexão numa ferramenta de correio eletrônico  (como  Microsoft  Outlook  Express  ou  Mozilla  Thunderbird),  deve-se  escolher  um protocolo  para  recebimento  de  mensagens.  Qual  das  alternativas  abaixo  serve  para  essa finalidade?

a) FTP
b) POP
c) IP
d) SMTP
e) UDP

16. (FUNRIO / DEPEN – 2009) Qual tipo de servidor utilizado para converter os nomes digitados na barra de endereços de um navegador para um endereço IP válido?

a) ISP
b) SMTP
c) Proxy
d) DHCP
e) DNS

17. (FUNRIO / MDIC – 2009) O protocolo HTTP (Hiper Text Transfer Protocol) tem a função básica de:

a) transferir arquivos.
b) exibir páginas em formato HTML.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






93
105
c) traduzir URL em endereços IP.
d) evitar o acesso não autorizado aos recursos de uma rede.
e) criar páginas dinâmicas.

18. (FUNRIO / Ministério da Justiça – 2009) O Protocolo da Internet responsável pelo recebimento de mensagens, copiando-as para o computador é o:

a) SMTP
b) http
c) Webmail
d) FTP
e) POP3

19. (FUNRIO / Ministério da Justiça – 2009) O protocolo HTTPS é considerado seguro porque:

a) verifica com um AntiSpyware o endereço acessado.
b) escaneia os arquivos procurando por vírus antes de baixá-los.
c) só funciona dentro de uma Intranet.
d) utiliza criptografia.
e) impede o uso de Spoofing.

20. (FUNRIO / SUFRAMA – 2008) No contexto da Internet, qual o significado da sigla DNS?

a) Provedor de serviços de internet através do qual um computador se conecta à internet.
b) Conjunto de protocolos que permitem a comunicação entre computadores.
c) Servidor de rede que controla o acesso dos demais computadores a uma rede.
d) Computador central que traduz nomes de domínios para endereços de protocolo na internet.
e) Sistema que permite localizar os computadores ligados a uma rede pelo seu nome.

21. (CS-UFG  /  UFG  –  2017) Um  funcionário  está  acessando  o  site  de  um  dos  fornecedores  da empresa, no endereço http://fornecedor.org/. Em um determinado momento, o site apresenta um formulário solicitando diversas informações. Antes de preencher o formulário, o funcionário quer saber se o site é seguro, no sentido de ter as informações transmitidas por meio de uma conexão criptografada.

Qual endereço indica que o site é seguro?

a) http://siteseguro.org/fornecedor.org/formulario/ b) sec://firewall/fornecedor.org/formulario/ c) https://fornecedor.org/formulario/ d) http://https.fornecedor.org/formulario/ 
22. (CS-UFG / UNIRG – 2017) O uso do prefixo “HTTPS” é um dos recursos da Internet que ajudam a garantir o acesso e a navegação entre páginas de maneira protegida.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






94
105

Quando o termo “https:”aparece significa que a comunicação com a página é feita de forma 
a) segura.
b) anônima.
c) prioritária.
d) privilegiada.

23. (CS-UFG  /  APARECIDAPREV  –  2018) Há  sites  na  Internet  que  são  acessados  por  meio  do protocolo HTTPS, como, por exemplo, o site https://cs.ufg.br.

Qual é a função do HTTPS?

a) Tornar mais rápida a navegação pelo site.
b) Bloquear as janelas pop-up.
c) Garantir que o navegador apresente uma única página por aba.
d) Fazer com que os dados sejam transmitidos de forma criptografada.

24. (IADES  /  ARCON  PA  –  2018) [...]  é  um  tipo  de  rede  local  que  utiliza  sinais  de  rádio  para comunicação.

CERT.br. Centro de Estudos, Resposta e Tratamento de Incidentes de Segurança no Brasil. Cartilha de Segurança para Internet. Disponível em:
<https://cartilha.cert.br/livro/cartilha_segurança_internet.pdf>.
Acesso em: 28 jun. 2018.

A definição apresentada refere-se a:

a) IP: Internet Protocol.
b) DNS: Domain Name Server.
c) SMTP: Simple Mail Transfer Protocol.
d) URL: Universal Resource Locator.
e) Wi-Fi: Wireless Fidelity.

25. (IDECAN / IPC – 2018) Considerando os recursos que podem ser consumidos ou acessados na Internet, analise as seguintes informações.

I
. O FTP é o protocolo utilizado para a transferência de arquivos entre duas máquinas ligadas à Internet.
II. Um correio eletrônico permite a troca de mensagens que um usuário de Internet pode fazer para outras pessoas conectados à Internet.
III. O HTTP é o protocolo utilizado para controlar a comunicação entre o servidor de Internet e o browser ou navegador.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






95
105
IV.  O  ICMP  é  o  protocolo  responsável  por  estabelecer a  comunicação  entre  os  computadores emissores e receptores de maneira na qual a informação não se perca na rede.

De acordo com as afirmativas acima, marque a alternativa correta.

a) Apenas as afirmativas I e II estão corretas.
b) Apenas as afirmativas I, II e III estão corretas.
c) Apenas as afirmativas II e III estão corretas.
d) Apenas as afirmativas I, II e IV estão corretas.

26. (IDECAN / BANESTES – 2012) Segundo Kurose (2010), o correio eletrônico existe desde o início da  Internet.  Ao  contrário  do  correio  normal,  que  anda  a  passos  lentos,  o  correio  eletrônico  é rápido, fácil de distribuir e barato. Identifique dois protocolos utilizados em correio eletrônico.

a) DNS e http.
b) POP3 e TCP.
c) IMAP e FTP.
d) POP3 e SMTP.
e) SMTP e IP.

27. (IESES  /  CRM/SC  –  2017) Considerando  o  cliente  de  e-mails  Microsoft  Outlook,  aponte  o número de porta padrão para o recebimento de mensagens POP3:

a) 587
b) 110
c) 25
d) 443

28. (IESES  /  CRMV/SC  –  2017) Uma  das  principais  preocupações  ao  se  realizar  transações eletrônicas  através  da  internet  está  na  segurança  da  comunicação  entre  o  computador  do usuário  e  o  servidor  que  provê  o  produto/serviço.  Esta  segurança  é  proporcionada  pela criptografia dos dados entre as duas partes da comunicação, através de um protocolo específico, que usualmente é representado antes do endereço do site no qual se está navegando. Dentre os protocolos abaixo mencionados, qual representaria uma conexão criptografada entre o cliente e o servidor?

a) wwws
b) https
c) http
d) stp

29. (IESES / CRO/SC – 2017) O servidor responsável por traduzir para números IP os endereços de sites que digitamos nos navegadores é o servidor:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






96
105
a) DNS.
b) IMAP.
c) SMTP.
d) DHCP.

30. (IESES / CRO/SC – 2016) O  protocolo  responsável  pelo  envio  de  mensagens  eletrônicas  (e- mails) através da internet é o:

a) POP3.
b) SNMP.
c) SMTP.
d) FTP.

31. (IESES / IGP/SC – 2014) Analise as afirmativas abaixo e assinale a alternativa correta:

I. POP3
II. SMTP
III. FTP
IV. SSH
V. IMAP

a) Apenas as afirmativas II e III são protocolos utilizados no envio ou recebimento de e-mails.
b) As afirmativas I, II e V são protocolos utilizados no envio ou recebimento de e-mails.
c) A afirmativa I é um protocolo utilizado no envio de e-mails.
d) As afirmativas II, III e IV são protocolos utilizados no recebimento de e-mails.

32. (AOCP / Prefeitura de Paranavaí/PR – 2013) Com  relação  a  conceitos  de  Internet  assinale  a alternativa INCORRETA.

a) Navegador de internet é um programa que permite você acessar e navegar entre as páginas de um ou mais sites.

b) Os Cookies possuem como principal função armazenar as preferências dos usuários sobre um determinado site na Internet.

c) Download é a saída de arquivos do seu computador para a internet. Os provedores gratuitos de   download   variam   bastante   na   sua   política,   capacidades   e   prazo   de   validade   das transferências.

d) E-mail é uma ferramenta que permite compor, enviar e receber mensagens, textos, figuras e outros arquivos através da Internet.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






97
105
e) HTTP é um protocolo que permite o funcionamento da interface gráfica na Internet, esta que é a mais conhecida e que permite transmissão de texto, fotos e gráficos de uma maneira simples e rápida.

33. (AOCP / Prefeitura de Valença/BA – 2016) A base para a comunicação de dados da internet é um  protocolo  da  camada  de  aplicação  do  modelo  OSI, que  é  responsável  por  transferir hipertextos. Esse protocolo é conhecido como:

a) HTML.
b) HTTP.
c) FTP.
d) PHP.
e) www.


34. (AOCP / FUNDASUS – 2015) Em redes de computadores, existem, basicamente, dois modelos de  referência  divididos  em  camadas  e  que  possuem  protocolos  de  comunicação  específicos.
Esses modelos são conhecidos como:

a) OSI e TCP/IP.
b) DHCP e HTTP.
c) IEEE e OSI.
d) Ethernet e IP
e) IANA e TCP.


35. (AOCP / FUNDASUS – 2015) Os protocolos de comunicação são a base da internet. Dentre os protocolos da camada de transporte do modelo TCP/IP, está o protocolo UDP (User Datagram Protocol) que se caracteriza por:

a) não dar garantias que o pacote enviado chegará ao seu destino.
b) ser utilizado pelos sistemas de informação de hipermídia, distribuídos e colaborativos.
c) permitir que um usuário se conecte a um computador rodando o Microsoft Terminal Services.
d)  ser  um  protocolo  de  comunicação  usado  entre  todas  as  máquinas  de  uma  rede  para  o encaminhamento de dados.
e) verificar se os dados são enviados de forma correta, na sequência apropriada e sem erros para o destino.


36. (CONSULPLAN / TRT - 13ª Região / PB – 2012) A conexão entre computadores e meios físicos de dados é realizada através do dispositivo placa de rede. Toda placa de rede recebe um número único para a sua identificação denominado:

a) IPV4.
b) IPV6
c) MAC.
d) RASH.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






98
105
e) BIT.

37. (ITAME / Prefeitura de Aragoiânia – 2016) Assinale a alternativa correta:

a) POP3 é um protocolo de envio de e-mails.
b) FTP é um protocolo utilizado para transferência de arquivos.
c) SMTP é um protocolo de recebimento de emails.
d) HTTPS é um protocolo criado somente para trafegar voz na internet.

38. (FACET / Prefeitura de Sobrado – 2016) Qual  é  o  protocolo  utilizado  para  transferência  de hipertextos na camada de aplicação segundo o modelo OSI?

a) FPT
b) TCP/IP
c) Proxy
d) DHCP
e) HTTP

39. (AOCP  /  ITEP-RN  –  2018) Em  relação  à  transferência  de  arquivos  pela  internet,  assinale  a alternativa correta.

a)  Quando  uma  pessoa  envia  um  arquivo  de  seu  computador  para  um  site  na  internet,  a operação de transferência que está sendo executada é conhecida como Download.

b)  FTP  é  um  protocolo  que  pode  ser  utilizado  para  transferir  arquivos  entre  computadores conectados à internet.

c)  Podemos  considerar  os  termos  Upload  e  Download  como  análogos,  ou  seja,  possuem  o mesmo significado.

d) O protocolo FTP é utilizado exclusivamente para se realizar o acesso a websites na internet.

e) O termo Upload se refere à velocidade na qual um computador conectado à internet consegue receber os dados de um website qualquer.

40. (CONSESP / Prefeitura de Quedas do Iguaçu - PR – 2012) A  transferência  de  arquivos  entre dois computadores ligados à Internet é realizada pelo protocolo denominado de:

a) FUNDNET
b) IP
c) WWW
d) FTP

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






99
105
41. (PR-4 / UFRJ – 2012) O  protocolo  da  Internet  utilizado  principalmente  para  transferência  de arquivos entre dois computadores é o:

a) FTP;
b) DHCP;
c) NTP;
d) DNS;
e) WINS.

42. (IFSP / IFSP – 2012) Assinale a alternativa que informa o protocolo usado para transferência de arquivos entre computadores ligados na Internet.

a) IMAP.
b) FTP.
c) SMTP.
d) DHCP.
e) SNMP.

43. (EPL / Câmara Municipal de Paraíso do Norte/PR – 2013) Na  internet  o  termo  UPLOAD  é designado para:

a) Enviar um arquivo para um local na internet, como por exemplo um disco virtual.
b) Baixar um arquivo de um servidor ou disco virtual.
c) Compactar um arquivo d) Enviar uma mensagem instantânea e) Carregar uma página da web no navegador 
44. (IBFC / ABDI – 2008) "____________ é a transferência de dados de um computador remoto para um computador local, e o inverso chama-se ____________".

Complete a frase acima respectivamente com as seguintes palavras:

a) upload / download b) download / upload c) upload / reload
d) reload / download 
45. (FADESP / Prefeitura de Conceição do Araguaia/PA – 2009) O  ato  de  transferir  arquivos  do computador de um usuário para a Web é denominado:

a) Download.
b) Upload.
c) NumLoad.
d) EndLoad.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






100
105

46. (UNA  /  Prefeitura  de  São  Sebastião/RS  –  2015) O  processo  pelo  qual  um  programa  ou documento é baixado da Internet para o computador do usuário é conhecido como:

a) Download
b) Backup
c) Upload
d) Update


47. (CAIP / Câmara Municipal de São Caetano do Sul/SP – 2014) Na Internet, a transferência de dados de um computador externo ou servidor para seu computador local é conhecida como:

a) Download.
b) Upload.
c) Peopleware.
d) Downgrade.


48.(CONSULPAM  /  Prefeitura  de  Tarrafas/CE  –  2015) Marcos  transferiu  um  arquivo  do  seu computador para a Web. Essa ação é denominada:

a) Upload
b) Download
c) EndLoad
d) NumLoad


49. (SELECON / Prefeitura de Cuiabá/MT – 2015) Um internauta baixou o arquivo ccleaner-5-38- 6357.exe do site do fabricante na internet para viabilizar a instalação do software Ccleaner em seu computador. O procedimento de baixar um arquivo da internet para o computador de um usuário é conhecido pelo seguinte termo:

a) download
b) downsize
c) upload
d) upsize



50. (CEPERJ / FSC – 2014) Atualmente,  é  comum  baixar  softwares  de  sites  da  internet  como  as atualizações  de  antivírus  e,  paralelamente,  enviar arquivos  para  sites  de  hospedagem  web.
Essas atividades são conhecidas, respectivamente, por:

a) download e upload b) upload e download c) download e downlink d) downlink e uplink Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






101
105
e) uplink e downlink 
51. (CPCON / Prefeitura de Catolé do Rocha/PB – 2015) O  envio  e  o  recebimento  de  dados  na internet, entre duas máquinas, constituem, respectivamente, em:

a) Downgrade e upgrade b) Upload e download c) Downfile e upfile d) Upgrade e downgrade e) Download e upload 

52. (FUNCAB  /  SESAU-RO  –  2009) Qual  o  nome  da  função  que  permite  ao  usuário  copiar  um arquivo de um site da Internet para o seu próprio computador?

a) Upload.
b) Transfer.
c) Download.
d) Copy.
e) Paste.


53. (FEPESE  /  UFFS  –  2012) Como  é  denominado  o  ato  de  baixar  dados  da  internet  para  um computador?

a) Reload.
b) Download.
c) Upload.
d) Formatação.
e) Refresh.


54. (BIO-RIO / Prefeitura de Três Rios-RJ – 2015) Redes  de  computadores  possibilitam  a  uma máquina  conectada  à  internet  baixar  de  sites  especializados  as  atualizações  de  programas antivírus,  como  o  Avast,  por  exemplo.  No  contexto  da  informática,  essa  atividade  recebe  a seguinte denominação:

a) download
b) downsize
c) upgrade
d) upload
e) upsize

55. (AOCP / FUNDASUS – 2015) Acerca dos termos utilizados na internet, quando anexamos um arquivo a uma mensagem de e-mail, estamos realizando uma operação de:

a) ROM.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






102
105
b) Boot.
c)  Hashtag.
d) Upload.
e)  UML.

56. (NC-UFPR / COPEL – 2013) No contexto da Internet, como é comumente chamada a ação de transferir um ou mais arquivos de um computador local para um servidor remoto?

a) Download.
b) Upload.
c) Downstream.
d) Baixar.
e) Gravar.

57. (ZAMBINI / PRODESP – 2010) A transferência de um arquivo de um computador local para um servidor na Internet é denominada(o):

a) Casting.
b) Upload.
c) Download.
d) Backup.
e) SMTP.

58. (UEM / UEM – 2017) É possível ao usuário transferir um arquivo de um site da Internet para o seu próprio computador. Esta função é chamada de:

a)  E-book.
b) Upload.
c)  Lista.
d) Download.
e) Copy.

59. (IFSP / IFSP – 2012) O  ato  de  transferir  um ou  mais  arquivos  de  um  servidor  remoto  para um computador através da Internet é chamado de:

a) formatação.
b) relocação.
c) upload.
d) editoração.
e) download.

60. (FUNCAB / SEAD-PB – 2012) O recurso que permite transferir um arquivo da Internet para um computador ou para um dispositivo de armazenamento de dados é chamado de:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






103
105
a) Recuperar fontes.
b) Print.
c) Hyperlink.
d) Download.
e) Upload.

61. (AOCP / Colégio Pedro II – 2013) Um usuário de um computador copiou uma foto de um site (servidor web) para seu computador. O processo feito por esse usuário foi:

a) Upload.
b) Compactação de arquivo.
c) Phishing.
d) Backup.
e) Download.

62. (LEGATUS  /  Câmara  Municipal  de  Bertolínia/PI  –  2013) “____________  significa  fazer  a transferência  de  algum  arquivo,  como  imagem,  vídeo ou  documento,  armazenado  em  um servidor remoto para o computador local”. A alternativa que preenche corretamente a lacuna em branco é:

a) Upload
b) Plug-in
c) Browser
d) Pop-up
e) Download

63. (KLC / Prefeitura de Mamborê/PR – 2016) Você precisa enviar sua foto para o perfil de usuário na home page da empresa. Você fará este procedimento acessando a página de novo usuário da empresa  que  o  contratou,  com  seu  login  e  senha.  Este  processo  de  envio  de  arquivos  de  uma máquina local para um servidor de intranet ou internet é comumente chamado de:

a) Reload de página.
b) Upload.
c) Download.
d) Link.
e) Logon.

64. (IBGP / CISSUL-MG – 2017) Ao  se  utilizar  a  internet,  depara-se  com  diversos  termos,  dentre esses, o UPLOAD que significa:

a)  A  ação  de  enviar  dados  de  um  computador  local  para  um  computador  ou  servidor  remoto, geralmente através da internet.
b) O ato de transferir (baixar) um ou mais arquivos de um servidor remoto para um computador local.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






104
105
c) O ato de enviar um arquivo para impressão.
d) A ação de realizar buscas na internet.

65. (CONSULPLAN / Prefeitura de Congonhas-MG – 2010) Sobre  os  conceitos  de  utilização  da internet,  a  transferência  de  dados  de  um  computador  remoto  para  um  computador  local, denomina-se:

a) Web Browser.
b) Download.
c) Transfer Web.
d) Upload.
e) Transceiver Web.

66. (AOCP / FUNDASUS – 2015) Acerca dos termos utilizados na internet, quando baixa-se um arquivo, realiza-se:

a) uma desfragmentação de disco.
b) uma compactação em seu tamanho físico.
c) uma compactação em seu tamanho lógico.
d) um UPLOAD.
e) um DOWNLOAD.























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 






105
105
GABARITO - BANCAS DIVERSAS 1. LETRA A
2. LETRA B
3. LETRA C
4. LETRA B
5. LETRA B
6. LETRA D
7. LETRA D
8. LETRA B
9. LETRA D
10. LETRA B
11. LETRA C
12. LETRA A
13. LETRA B
14. LETRA A
15. LETRA B
16. LETRA E
17. LETRA B
18. LETRA E
19. LETRA D
20. LETRA D
21. LETRA C
22. LETRA A
23. LETRA D
24. LETRA E
25. LETRA B
26. LETRA D
27. LETRA B
28. LETRA B
29. LETRA A
30. LETRA C
31. LETRA B
32. LETRA C
33. LETRA B
34. LETRA A
35. LETRA A
36. LETRA C
37. LETRA B
38. LETRA E
39. LETRA B
40. LETRA D
41. LETRA A
42. LETRA B
43. LETRA A
44. LETRA B
45. LETRA B
46. LETRA A
47. LETRA A
48. LETRA A
49. LETRA A
50. LETRA A
51. LETRA B
52. LETRA C
53. LETRA B
54. LETRA A
55. LETRA D
56. LETRA B
57. LETRA B
58. LETRA D
59. LETRA E
60. LETRA D
61. LETRA E
62. LETRA E
63. LETRA B
64. LETRA A
65. LETRA B
66. LETRA E

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 01
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 