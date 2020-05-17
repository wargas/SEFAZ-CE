

Livro Eletrônico
Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti 06315057411 - EVA CELESTE DE SOUZA 





1
132




Sumário
Redes de Computadores ................................................................................................................. 6 1 - Conceitos Básicos.................................................................................................................... 6 2 – Tipos de Conexão/Enlace ....................................................................................................... 9 3 – Modos de Transmissão ......................................................................................................... 11 3.1 – Simplex ........................................................................................................................... 11 3.2 – Half-Duplex .................................................................................................................... 11 3.3 – Full-Duplex ..................................................................................................................... 12 4 – Direções de Transmissão ...................................................................................................... 13 4.1 – Unicast [uni = um e cast = transmitir] ............................................................................. 13 4.2 – Multicast [multi = vários e cast = transmitir] ................................................................... 13 4.3 – Broadcast [broad = todos e cast = transmitir] ................................................................ 13 5 – Classificação de Redes.......................................................................................................... 14 5.1 – Quanto à Dimensão, Tamanho ou Área Geográfica ...................................................... 14 5.2 – Quanto à Arquitetura de Rede ou Forma de Interação .................................................. 20 5.3 – Quanto à Topologia (Layout) .......................................................................................... 23 6 – Meios de Transmissão .......................................................................................................... 27 6.1 – Cabo Coaxial .................................................................................................................. 28 6.2 – Cabo de Par Trançado.................................................................................................... 29 6.3 – Cabo de Fibra Óptica ..................................................................................................... 31 7 – Equipamentos de Redes ....................................................................................................... 32 7.1 – Network Interface Card (NIC ou Placa de Rede) ............................................................ 32 7.2 – Hub (Concentrador) ........................................................................................................ 34 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





2
132




7.3 – Bridge (Ponte)................................................................................................................. 36 7.4 – Switch (Comutador) ........................................................................................................ 37 7.5 – Router (Roteador) ........................................................................................................... 38 7.6 – Access Point (Ponto de Acesso) ..................................................................................... 40 7.7 – Modem ........................................................................................................................... 43 8 – Padrões de Redes ................................................................................................................. 46 8.1 – Padrão Ethernet (IEEE 802.3) ......................................................................................... 47 8.2 – Padrão Token Ring (IEEE 802.5) ..................................................................................... 52 8.3 – Padrão Wireless (IEEE 802.11) ........................................................................................ 53 8.4 – Padrão Bluetooth (IEEE 802.15) ..................................................................................... 56 8.5 – Padrão WiMAX (IEEE 802.16) ......................................................................................... 57 Internet........................................................................................................................................... 58 1 - Conceitos Básicos.................................................................................................................. 58 2 – Web (WWW) ......................................................................................................................... 66 2.1 – Web 0.0 .......................................................................................................................... 67 2.2 – Web 1.0 .......................................................................................................................... 67 2.3 – Web 2.0 .......................................................................................................................... 68 2.4 – Web 3.0 .......................................................................................................................... 68 3 – Internet das Coisas (IoT) ....................................................................................................... 69 4 – Tecnologias de Acesso ......................................................................................................... 71 4.1 – Dial-Up ........................................................................................................................... 72 4.2 – ISDN (Integrated Services Digital Network).................................................................... 73 4.3 – ADSL (Asymmetric Digital Subscriber Line) .................................................................... 73 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





3
132




4.4 – Acesso Via Cabo (HFC e Cable Modem) ........................................................................ 73 4.5 – PLC (Power Line Communication) .................................................................................. 73 4.6 – Telefonia Celular ............................................................................................................ 73 Resumo .......................................................................................................................................... 75 Mapa Mental .................................................................................................................................. 82 Questões Comentadas - FCC ........................................................................................................ 85 Lista de Questões – FCC................................................................................................................ 98 Gabarito – FCC ............................................................................................................................ 106 Questões Comentadas – Bancas Diversas ................................................................................... 107 Lista de Questões – Bancas Diversas ........................................................................................... 123 Gabarito – Bancas Diversas .......................................................................................................... 132 



















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





4
132




APRESENTAÇÃO DOS PROFESSORES 

QUEM SOMOS

Ahhh... eu sou esse cara da direita! Já o cara da esquerda é o Prof. Renato da
Costa! Um monstro da Informática para Concursos  Públicos.  Quem  é  do  RJ  já conhece muito bem esse mito vascaíno e  sabe  que  ele  tem  uma  didática sensacional.  Eu  garanto  que  a  nossa dupla  fará  o  melhor  possível  em  duas frentes diferentes – eu, no PDF e ele na videoaula  –  para  entregar  o  melhor material de concurso de informática :) 
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





5
132




APRESENTAÇÃO DA AULA 
Pessoal, o tema da nossa aula é: Redes de Computadores e Internet. A primeira parte não é muito comum  em  prova  (e  também  não  é  muito  fácil). Por que?  Porque  trata  de  assuntos  bastante técnicos! Diego, por que isso é cobrado na minha prova? Cara, isso é um pré-requisito para entender melhor Internet, uma vez que ela é um tipo de Rede de Computadores. Já a parte de Internet em si está no cotidiano de vocês, logo é bem mais tranquilo...

PROFESSOR DIEGO CARVALHO - www.instagram.com/professordiegocarvalho 
Galera, todos os tópicos da aula possuem Faixas de Incidência, que indicam se o assunto cai muito ou pouco em prova. Diego, se cai pouco para que colocar em aula? Cair pouco não significa que não cairá justamente na sua prova! A ideia aqui é: se você está com pouco tempo e precisa ver somente aquilo que cai mais, você pode filtrar pelas incidências média, alta e altíssima; se você tem tempo sobrando e quer ver tudo, vejam também as incidências baixas e baixíssimas. Fechado?

INCIDÊNCIA EM PROVA: baixíssima 
INCIDÊNCIA EM PROVA: baixa 
INCIDÊNCIA EM PROVA: média 
INCIDÊNCIA EM PROVA: ALTA 
INCIDÊNCIA EM PROVA: Altíssima 



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





6
132




REDES DE COMPUTADORES 1 - Conceitos Básicos INCIDÊNCIA EM PROVA: baixíssima 


Fala,  galera! Vamos  iniciar  nossos  estudos  sobre  os  Conceitos  Básicos  de  Redes  de Computadores – além de ser um assunto de suma importância, ele subsidia tudo que veremos mais à frente sobre Internet. Beleza? Agora vamos contar uma história! No Século XIX, enviar uma carta de Londres até Califórnia por meio dos correios demorava entre dois e três meses – isso se você tivesse grana suficiente para pagar pelo envio de cartas. Incrível, não?



Hoje em dia, enviar um correio eletrônico demora uma fração de segundos. Isso melhorou a eficiência das indústrias, dinamizou o comércio global e melhorou a economia mundial fazendo com que chegássemos em alta velocidade a praticamente qualquer ponto do planeta. Galera, vocês Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





7
132




podem até pensar que os computadores e as redes de computadores sempre andaram juntos, mas não funcionava assim – as redes vieram bem depois!

Durante a década de 1970, os computadores ficavam isolados no mundo – praticamente não se comunicavam.
Nessa época, eles tinham o tamanho de uma geladeira, às vezes de uma sala e, às vezes, até de um andar inteiro de prédios ou universidades. Os computadores pessoais 1
ainda
não tinham se popularizado, apesar de – em 1977 – um cara chamado Steve Jobs ter lançado um microcomputador com teclado integrado e... pasmem... capaz de gerar gráficos coloridos.

Enfim,  nessa  época, era comum termos um processamento centralizado,  ou  seja,  um  único computador de grande porte – chamado Mainframe – de alto custo e que rodava em geral poucas e simples aplicações. Na década seguinte, com a popularização dos computadores pessoais, as Redes de Computadores foram ganhando espaço, uma vez que as pessoas descobriram que era muito mais interessante compartilhar dados e recursos.

Do processamento que ocorria integralmente centralizado nos computadores de grande porte, passamos para um processamento distribuído nos computadores pessoais de uma rede. Dessa forma, em vez de um único mainframe ser responsável por todo processamento, computadores distintos espalhados em uma rede realizavam parte desse trabalho. Dito isso, chegou a hora de saber o conceito de uma rede:

“Uma rede é um conjunto de terminais, equipamentos, meios de transmissão e comutação que interligados possibilitam a prestação de serviços”.

Bem,  eu  gosto  de  uma  definição  mais  simples  que  afirma  que uma  rede  é  um  conjunto  de dispositivos (normalmente conhecidos como nós) conectados por links de comunicação.
Em
uma rede, um nó pode ser um computador, uma impressora, um notebook, um smartphone, um tablet, um Apple Watch ou qualquer outro dispositivo de envio ou recepção de dados, desde que ele esteja conectado a outros nós da rede.


As primeiras redes de computadores surgiram dentro de organizações – como uma empresa ou um laboratório  de  pesquisa  –  para  facilitar  a  troca  de  informações  entre  diferentes  pessoas  e computadores.
Esse método era mais rápido e confiável do que anterior, que consistia em pessoas carregando pilhas e pilhas de cartões perfurados ou fitas magnéticas de um lado para o outro dentro de uma organização.

Sim, antigamente os dados de um computador ficavam armazenados em pequenos cartões de papel cheio de furinhos chamado cartões perfurados; ou em um rolo enorme de fita magnética. Se você quisesse trocar informações entre pessoas ou equipamentos, você tinha que transportar pilhas enormes desses cartões perfurados ou de fitas magnéticas até o local onde se encontrava o destinatário
. Já imaginaram isso?

1
Computadores Pessoais são também conhecidos como Personal Computers (PC), Workstations ou Estações de Trabalho.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





8
132







Um segundo benefício das redes de computadores é a capacidade de compartilhar recursos físicos. Por exemplo: em vez de cada computador possuir sua própria impressora, todos em um departamento poderiam compartilhar apenas uma impressora conectada à rede de computadores.
Outro uso comum era compartilhar dispositivos de armazenamento, que na época eram muitos caros e não era viável ter um para cada computador.

Como nós podemos resumir tudo isso?
Bem, uma rede de computadores basicamente tem como objetivo  o  compartilhamento  de  recursos,  deixando  equipamentos,  programas  e principalmente dados ao alcance de múltiplos usuários , sem falar na possibilidade de servir como meio de comunicação entre pessoas através da troca de mensagens de texto, áudio ou vídeo entre os dispositivos. Fechado?

(Assembleia Legislativa de Goiás – 2016) Um  conjunto  de  unidades  processadoras interconectadas  que  permite,  inclusive,  o  compartilhamento  de  recursos  tais  como impressoras, discos, entre outros, denomina-se:

a) Time Sharing
b) Redes de Computadores c) Compartilhamento do Windows d) Interligação de Redes de Computadores _______________________ Comentários: quando a banca diz “um conjunto de unidades processadoras”, ela só está usando um nome técnico para “um conjunto de computadores”. Portanto, um conjunto de computadores interconectados que permite o compartilhamento de recursos tais como impressoras, discos, entre outros, só pode ser uma... rede de computadores (Letra B).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





9
132




2 – Tipos de Conexão/Enlace INCIDÊNCIA EM PROVA: baixíssima 
Redes  são  dois  ou  mais  dispositivos  conectados  através  de  links. O  que  é  um  link? Também chamado  de  enlace, trata-se  de  um  caminho  de  comunicação  que  transfere  dados  de  um dispositivo para outro.
Para fins de visualização, é mais simples imaginar qualquer link como uma reta entre dois pontos. Para ocorrer a comunicação, dois dispositivos devem ser conectados de alguma maneira ao mesmo link ao mesmo tempo.

Existem  dois  tipos  possíveis  de  conexão:  ponto-a-ponto  e  ponto-multiponto.  Ambos  se diferenciam em relação à utilização de um link dedicado ou compartilhado. Como assim, Diego?
Um link dedicado é aquele que transporta tráfego de dados apenas entre os dois dispositivos que ele conecta. Exemplo: para que eu acesse a internet, eu compartilho vários cabos subterrâneos espalhados pelo nosso planeta com todas as pessoas que tem acesso à internet.



Nesse contexto, pode-se afirmar que, quando eu acesso à internet, eu utilizo um link dedicado ou um link compartilhado? Galera, eu utilizo um link compartilhado porque o enlace de comunicação é compartilhado  com  várias  pessoas.
No  entanto,  só  é  possível  ter  links  dedicados  apenas  à comunicação entre dois – e apenas dois – dispositivos. Nesse caso, existe um tipo de conexão conhecido como ponto-a-ponto.

A maioria das conexões ponto-a-ponto utiliza um cabo para conectar dois dispositivos. No entanto, é possível haver links via satélite ou micro-ondas também de forma dedicada. Quando mudamos os canais de televisão por meio da utilização de um controle remoto infravermelho, nós estamos  estabelecendo  uma  conexão  ponto-a-ponto  entre  o  controle  remoto  e  o  sistema  de controle de TV. Bacana?



Já  uma  conexão  ponto-multiponto  é  uma  conexão  na  qual  mais  de  dois  dispositivos compartilham um único link.
E um ambiente multiponto, a capacidade do canal de comunicação Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





10
132




é compartilhada, seja de força espacial ou seja de forma temporal. Se diversos dispositivos puderem usar  o  link  simultaneamente,  ele  é  chamado  de  conexão  compartilhada  espacialmente.  Se  os usuários tiverem de se revezar entre si, trata-se de uma conexão compartilhada no tempo.

TIPO DE CONEXÃO DESCRIÇÃO PONTO-A-PONTO
Conexão que fornece um link dedicado entre dois dispositivos.
PONTO-MULTIPONTO
Conexão que fornece um link compartilhado entre mais de dois dispositivos.


































Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





11
132




3 – Modos de Transmissão INCIDÊNCIA EM PROVA: baixíssima 
3.1 – Simplex



O enlace é utilizado apenas em um dos dois possíveis sentidos de transmissão Exemplo: TV, Rádio AM/FM, Teclado, etc.

Uma comunicação é dita simplex quando há um transmissor de mensagem, um receptor de mensagem e esses papéis nunca se invertem no período de transmissão . Quando você vê TV, sua antena recebe um sinal de um satélite, mas ela jamais envia/transmite sinais para o satélite.
Logo, o satélite é o transmissor, sua antena é o receptor, e esses papéis não são trocados – o mesmo serve para Rádio AM/FM ou para o teclado de um computador.




3.2 – Half-Duplex



O enlace é utilizado nos dois possíveis sentidos de transmissão, porém apenas um por vez Exemplo: Walk&Talk e Nextel 
Uma comunicação é dita half-duplex quando temos um transmissor e um receptor, sendo que ambos podem transmitir e receber dados, porém nunca simultaneamente . Quando você fala em um Walk&Talk com outra pessoa, você pode falar e ela também. Porém, quando você apertar o Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





12
132




botãozinho para falar, o receptor apenas ouvirá. Se ele tentar falar junto, a comunicação é cortada e nenhum dos dois se ouvem.




3.3 – Full-Duplex



O enlace é utilizado nos dois sentidos de transmissão simultaneamente Ex: Celular, VoIP.

Uma comunicação é dita full-duplex quando temos um transmissor e um receptor, sendo que ambos podem transmitir e receber dados simultaneamente . Quando você fala com outra pessoa por meio do seu smartphone, ela pode te responder simultaneamente. Você não tem que falar, depois ouvir, depois falar de novo. Vocês dois podem falar juntos sem problema porque se trata de uma transmissão bidirecional.







Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





13
132




4 – Direções de Transmissão INCIDÊNCIA EM PROVA: baixíssima 
A  transmissão  de  dados  em  uma  rede  de  computadores pode  ser  realizada  em  três  sentidos diferentes: Unicast, Multicast e Broadcast. Vamos vê-los em detalhes:

4.1 – Unicast [uni = um e cast = transmitir] 
Nessa comunicação, uma mensagem só pode ser enviada para um destino. Observem que a primeira estação de trabalho está enviando uma mensagem endereçada especificamente para a terceira estação de trabalho. Analogamente, quando você envia uma mensagem no Whatsapp para uma pessoa específica, você está enviando uma mensagem unicast.



4.2 – Multicast [multi = vários e cast = transmitir] 
Nessa comunicação,
uma mensagem é enviada para um grupo de destino. Observem que a primeira estação de trabalho está enviando uma mensagem endereçada para o grupo da terceira e quarta estações. Analogamente, quando você cria uma lista de transmissão no Whatsapp   com um grupo de pessoas e os envia uma mensagem, você está enviando uma mensagem multicast.



4.3 – Broadcast [broad = todos e cast = transmitir] 
Nessa comunicação, uma mensagem é enviada para todos os destinos. Observem que a primeira estação de trabalho está enviando uma mensagem endereçada a todas as estações de trabalho.
Analogamente, quando você cria uma lista de transmissão no Whatsapp   com todos os seus contatos e os envia uma mensagem, você está enviando uma mensagem broadcast.




Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





14
132




5 – Classificação de Redes 5.1 – Quanto à Dimensão, Tamanho ou Área Geográfica 
Uma rede de computadores pode ser classificada quanto à dimensão, tamanho ou abrangência de área geográfica
. Galera, nós veremos detalhes sobre as características dessa classificação logo abaixo, no entanto é importante ressaltar uma particularidade a respeito da distância que essas redes de computadores podem abranger. Nós vamos passar algumas noções de distância, mas saibam que não existe nenhuma convenção rígida sobre isso. Fechado?

5.1.1 – PAN (Personal Area Network) INCIDÊNCIA EM PROVA: baixa 


A Rede de Área Pessoal é definida como uma rede de computadores utilizada para conectar e transmitir dados entre dispositivos localizados em uma área pessoal. Pode ser chamada também de WPAN (Wireless Area Network), uma vez que seu principal meio de transmissão é o Bluetooth.
Em suma, ela é basicamente uma rede de computadores ou dispositivos que abrange um espaço pequeno – em geral, do tamanho máximo de um quarto.

Sabe aquele domingo que você leva sua caixinha de som para ouvir uma música na beira da piscina e a conecta ao seu smartphone?
Pois é, isso é uma PAN! Sabe quando você vai dar aquela corridinha segunda-feira (para se recuperar da cachaça de domingo) e leva seu fone de ouvido sem fio conectado ao seu smartphone também para ouvir uma música? Adivinha... isso também é uma PAN! Enfim...
entenderam, não é?

Distância

ALGUNS CENTÍMETROS A POUCOS METROS 

PAN
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





15
132




5.1.2 – LAN (Local Area Network) INCIDÊNCIA EM PROVA: Altíssima 


A
Rede de Área Local é definida  como  uma  rede  de computadores  utilizada  para  conectar  e transmitir dados entre dispositivos localizados em uma área local. Quem aí já foi a uma Lan House?
O nome já dá a dica, trata-se de uma LAN. A rede da sua casa também, assim como a rede do andar de um prédio ou a rede de um órgão localizado em um único espaço físico também são redes locais.
Entendido, camaradas?

Em geral, esse tipo de rede possui baixa ocorrência de erros por redes pequenas e contidas em um local específico – e, não, espalhadas por vários locais. E o que tem a ver essa foto, professor? Galera, a imagem acima é do meu querido local de trabalho. Para quem não conhece, esse é o prédio do Tesouro Nacional e eu orgulhosamente vos apresento o fantástico céu de Brasília. Tem coisa mais bonita?
Venham aqui me visitar e me convidem para o churrasco de posse :) 

Distância

De algumas centenas de metros a alguns quilômetros.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





16
132




5.1.3 – MAN (Metropolitan Area Network) INCIDÊNCIA EM PROVA: Altíssima 


A
Rede de Área Metropolitana é definida como uma rede de computadores utilizada para conectar e transmitir dados entre dispositivos localizados em locais distintos. Elas possuem abrangência maior  que  a  de  uma  rede  local  e  menor  que  a  de  uma rede  extensa  –  que  veremos  a seguir.
Normalmente uma rede metropolitana resulta da interligação de várias redes locais em uma cidade, formando assim uma rede de maior porte.

Na imagem acima, temos uma foto aérea de Brasília! Eu não sei se vocês sabem, mas foi aqui que foi criada a Rede de Fast- food Giraffas! Na imagem, temos a localização de dezenas de filiais dessa empresa em uma mesma cidade – essas filiais
podem  se  conectar  formando  uma  única  rede  de  área metropolitana espalhada em diferentes locais dentro de uma mesma cidade ou metrópole a uma distância maior que a de uma rede local e menor que a de uma rede extensa.



Distância

algumas dezenas de quilômetros 

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





17
132




5.1.4 – WAN (Wide Area Network) INCIDÊNCIA EM PROVA: Altíssima 


A
Rede de Área Extensa é definida como uma rede de computadores utilizada para conectar e transmitir dados entre dispositivos localizados em uma grande área geográfica . E quando eu digo
grande,  é  grande  mesmo  –  podendo  ser  entre  cidades,  entre  países  ou  –  até  mesmo –  entre continentes diferentes. O Programa Antártico Brasileiro (PROANTAR)  – por exemplo – realiza pesquisas nesse continente e envia os dados para o Brasil por meio de uma rede extensa.

Quando uma empresa possui filiais em cidades ou países diferentes, ela pode criar uma Rede WAN. Aliás, vocês sabem qual é o melhor e mais clássico exemplo de WAN? A Internet! Sim, a Internet  é  uma  WAN  –  conforme  mostra  a imagem  ao  lado.  Outro  exemplo  seria  uma rede entre filiais de empresas localizadas em Brasília  e  Goiânia  –  como  apresentado  na imagem acima.
Essa rede formaria o que nós chamamos de rede de área extensa.



Distância

centenas a milhares de quilômetros 


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





18
132




Em suma, a classificação quanto à dimensão pode ser resumida a seguinte tabela:

TIPO SIGLA DESCRIÇÃO DISTÂNCIA PERSONAL

AREA NETWORK
PAN
Rede  de  computadores  pessoal  (celular,  tablet, notebook, entre outros).
De alguns centímetros a alguns poucos metros.
LOCAL

AREA NETWORK
LAN
Rede  de  computadores  de  lares,  escritórios, prédios ou campus.
De algumas centenas de metros a alguns quilômetros.
METROPOLITAN

AREA NETWORK
MAN
Rede de computadores entre uma matriz e filiais em uma cidade.
Cerca de algumas dezenas de quilômetros.
WIDE

AREA NETWORK
WAN
Rede de computadores entre cidades, países ou até continentes.
De algumas dezenas a milhares de quilômetros.

Essas classificações apresentadas possuem uma classificação correspondente quando se trata de um contexto de transmissão sem fio (wireless). Em  outras  palavras,  há  também  WPAN, WLAN, WMAN e WWAN. Por outro lado, as questões de prova nem sempre são rigorosas na utilização desses termos (Ex: é comum enunciados tratando de redes locais sem fio como LAN e, não, WLAN). Infelizmente, desencanem na hora de resolver questões de prova...

(TELEBRÁS – 2015) As redes locais (LANs) são aquelas instaladas em grandes cidades de regiões metropolitanas, para a interconexão de um grupo grande de usuários.
_______________________ Comentários: grandes cidades de regiões metropolitanas? Não, essa é a MAN (Metropolitan Area Network)! A LAN (Local Area Network) conecta casas, escritórios, pavimentos ou prédios (Errado).

(TRT/SP – 2008) A configuração de rede mais adequada para conectar computadores de:

- um pavimento
- um estado
- uma nação

é, respectivamente:

a) LAN, WAN, WAN.
b) LAN, LAN, WAN.
c) LAN, LAN, WAN.
d) WAN, WAN, LAN.
e) WAN, LAN, LAN.
_______________________ Comentários: conforme vimos em aula, para conectar um pavimento ou andar de um prédio, utilizamos uma Rede de Área Local (LAN). Já para conectar um estado, isto é, as cidades que o compõem, nós utilizamos uma Rede de Área Extensa (WAN).
Por fim, para conectar uma nação, isto é, os estados que a compõem, nós utilizamos uma Rede de Área Extensa (WAN).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





19
132




Professor, e a MAN? Galera, lembrem-se que a MAN é para conectar redes dentro de uma mesma cidade – que não era o caso da questão. Tranquilo? Então, a resposta é LAN, WAN e WAN (Letra A).

(UFF – 2017) As redes podem ser classificadas quanto à extensão e, nesse caso, aquelas que normalmente permanecem em locais com extensão pequena, como um prédio de poucos andares ou uma sala, são conhecidas como:

a) LAN e MAN.
b) MAN e PAN.
c) PAN e LAN.
d) WAN e MAN.
e) LAN e WAN.
_______________________ Comentários: conforme vimos em aula, redes em locais com pequena extensão como um prédio ou uma sala geralmente são LANs ou PANs (Letra C).



Apenas a título de curiosidade, existem diversas outras classificações menos tradicionais. Duas são bastante interessantes: Body Area Network (BAN) e Interplanetary Area Network (IAN).


A  BAN  se  trata  de  uma  rede  de  área  corporal  que  está  geralmente relacionada  à  área  de  saúde  e  tem  ganhado  enorme  destaque recentemente
. Dispositivos podem ser implantados dentro do corpo humano ou vestidos em sua superfície. Vocês sabem esses smartwatches que estão na moda agora? Eles são capazes de realizar diversas medidas no seu corpo e enviar  para  o  seu  smartphone  formando  uma  rede  corporal,  no  entanto existem dezenas de outras possibilidades...


Existe também uma classificação chamada Interplanetary Area Network.
Sabe a Curiosity? Ela é um veículo-sonda que está percorrendo a superfície de  Marte  desde  2012  e  enviando  dados  para  a  Terra. Pois  é,  pode-se classificar a rede formada entre a sonda e nosso planeta como uma IAN – uma Rede de Área Interplanetária cuja distância é de... alguns milhões de quilômetros. Diz se informática não é a melhor disciplina do universo :) 

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





20
132




5.2 – Quanto à Arquitetura de Rede ou Forma de Interação 
Antes de entrar nessa classificação, é importante entender alguns conceitos. Primeiro, vamos entender o que é um cliente e o que é um servidor. Galera, é muito comum que empresas tenham uma grande quantidade de computadores. Antigamente, eles funcionavam de forma isolada. No entanto, com o passar do tempo, descobriu-se que conectá-los era uma estratégia interessante para otimizar processos e correlacionar informações de setores diferentes de uma empresa.


Um dos grandes incentivos para conectar computadores era o compartilhamento de recursos, isto é, tornar todos os programas, equipamentos e especialmente dados ao alcance de todas as pessoas na rede, independentemente da localização física do recurso e do usuário. Exemplo: um grupo de funcionários de um escritório que compartilham uma impressora comum. Ora, raramente alguém necessita de uma impressora privativa.

Todo mundo sabe que, quando uma impressora de grande capacidade é conectada em rede, ela acaba sendo até mais econômica, mais rápida e de mais fácil manutenção que um grande conjunto de  impressoras  individuais.  Mais  importante  que  compartilhar  recursos  físicos,  é  compartilhar dados.
Nesse modelo, é comum que dados sejam armazenados em poderosos computadores chamados de servidores.


Em contraste, os funcionários têm em suas escrivaninhas máquinas mais simples, chamadas clientes,  com  as  quais  eles  acessam  dados  remotos  que  estão  armazenados  aonde?  No servidor!  As máquinas clientes e servidores são conectadas entre si por uma rede. Como na vida real, cliente é o aquele que consome algum serviço ou recurso; e servidor é aquele que fornece algum serviço ou recurso.

Quer um exemplo? Quando você faz o download um vídeo no site do Estratégia Concursos, você está consumindo um recurso do servidor do Estratégia. Sim, o Estratégia possui uma máquina especializada chamada de servidor, onde fica hospedado o seu site.
Quando você faz o download da sua aula de informática, você está exercendo um papel de Cliente. E quem fornece o recurso solicitado por você está exercendo o papel de Servidor.
Dito isso, vamos à classificação...


5.2.1 – Rede Ponto-a-Ponto INCIDÊNCIA EM PROVA: baixa 
Também chamada de Rede Par-a-Par ou Peer-to-Peer (P2P), trata-se do modelo de rede mais simples de ser montado. Nesse modelo, todas as máquinas podem compartilhar dados e periféricos umas com as outras.
Essas redes são comuns em residências e entre filiais de empresas, porque demandam um baixo custo, são facilmente configuráveis e possibilitam altas taxas de velocidade de conexão.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





21
132




Observem a imagem acima: as máquinas estão ligadas umas com as outras de uma maneira bem simples, compartilhando recursos e sem hierarquia – todas as máquinas são iguais, por isso são chamadas de pares. Uma máquina pode fornecer um recurso para a outra, que pode fornecer outro recurso de volta. Nesse tipo de rede, todas as máquinas oferecem e consomem recursos uma das outras, logo todas são eventualmente clientes, eventualmente servidoras.

Ponto-a-ponto é geralmente utilizado em redes domésticas com poucos computadores com o intuito típico de trocar arquivos, compartilhar impressoras e internet – sem nenhum gerenciamento de usuário.
Como não há um dispositivo central capaz de oferecer serviços de autenticação, criptografia, etc, o nível de segurança é reduzido nesse tipo de rede em comparação a redes de computadores do tipo cliente/servidor.
Ademais, não há nenhum gerenciamento de usuário.

5.2.2 – Rede Cliente/Servidor INCIDÊNCIA EM PROVA: média 
É um modelo de redes mais complexo, porém mais robusto e confiável.
Nesse  modelo,  existe  uma  máquina  especializada,  dedicada  e geralmente remota
, respondendo rapidamente aos pedidos vindos dos demais computadores da rede – o que aumenta bastante o desempenho de algumas tarefas. É a escolha natural para redes grandes, como a Internet – que funciona tipicamente a partir do Modelo Cliente/Servidor.


Observem  a  imagem  acima: as  máquinas  estão  todas  ligadas  a  uma  única  máquina, hierarquicamente diferente. Ao contrário do que ocorre nas redes par-a-par, os computadores que funcionam como clientes não fornecem recursos e serviços aos outros computadores da rede.
Existem diversos tipos de servidores, como por exemplo: servidor de impressão, servidor de e- mails, servidor de arquivos, servidor de comunicação, servidor de banco de dados, etc.



O termo ponto-a-ponto costuma confundir porque pode ser utilizado em dois contextos com significados diferentes. No contexto de tipos de conexão, ele pode ser utilizado como contraponto ao enlace ponto-multiponto, ou seja, trata-se de um link dedicado entre dois dispositivos, em contraste com o enlace ponto-multiponto, em que o link é compartilhado entre dispositivos. Já vimos isso...

No  contexto  de  arquitetura  ou  forma  de  interação,  ele  pode  ser  utilizado  como contraponto  ao  modelo  cliente/servidor.  Nesse  caso,  trata-se  de  uma  máquina  que  é simultaneamente cliente e servidor, diferente do modelo cliente/servidor, em que uma máquina  ou  é  um  cliente  ou  é  um  servidor.  Em  suma, o  termo  ponto-a-ponto  pode significar um enlace dedicado entre dois dispositivos ou uma rede em que uma máquina exerce o papel de cliente e de servidor.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





22
132





(Telebrás – 2015) Redes de comunicação do tipo ponto a ponto são indicadas para conectar, por exemplo, matriz e filiais de uma mesma empresa, com altas taxas de velocidade de conexão.
_______________________ Comentários: essa foi uma questão um pouco polêmica, porque termo "ponto-a-ponto" pode ser utilizado em dois contextos diferentes: pode ser ponto-a-ponto como um contraponto ao modelo de rede cliente-servidor ou pode ser ponto-a-ponto como um contraponto ao tipo de enlace ponto-multiponto. Como eu vou saber a qual deles a questão se refere? A única maneira é por meio da avaliação do termo ‘redes de comunicação'. Se fosse 'redes de computadores', nós poderíamos presumir que se tratava do modelo de rede ponto-a-ponto, mas como ele diz 'redes de comunicação', que tem um sentido mais amplo que ‘redes de computadores’, nós podemos inferir que se trata do tipo de enlace. A questão fala em um enlace capaz de conectar matrizes e filias, logo ele não é compartilhado por outras redes - apenas as matrizes e as filiais dessa rede podem ser comunicar por esse enlace. Assim, ele é capaz de fornecer altas taxas de velocidade de conexão, visto que o enlace (também chamado de link) não é compartilhado com outras máquinas de fora da rede (Correto).































Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





23
132




5.3 – Quanto à Topologia (Layout) 
Quando  falamos  em  topologia, estamos  tratando  da  forma  como  os  dispositivos  estão organizadores. Dois ou mais dispositivos se conectam a um link; dois ou mais links formam uma topologia. A topologia é a representação geométrica da relação de todos os links e os dispositivos de uma conexão entre si. Existem quatro topologias básicas 2
possíveis: barramento, estrela, anel e malha. No entanto, vamos primeiro entender a diferença entre topologia física e lógica.


A topologia lógica exibe o fluxo de dados na rede, isto é, como as informações percorrem os links e transitam entre dispositivos – lembrando que links são os meios de transmissão de dados. Já a topologia física exibe o layout (disposição) dos links e nós de rede.
Em outras palavras, o primeiro trata  do  percurso  dos  dados  e  o  segundo  trata  do  percurso  dos  cabos,  uma  vez  que  não necessariamente os dados vão percorrer na mesma direção dos cabos.


TIPO DE TOPOLOGIA DESCRIÇÃO FÍSICA
Exibe o layout (disposição) dos links e nós de rede.
LÓGICA Exibe o fluxo ou percurso dos dados na rede.



Quando uma determinada questão de prova não deixar explícito em sua redação qual é o tipo de topologia, pode-se assumir que ela se refere à Topologia Física e, não, à Topologia Lógica. É importante  destacar  também  que  uma  rede  de  computadores  pode  ter  uma  topologia  física completamente diferente de sua topologia lógica. Por exemplo: o Padrão Token Ring utiliza – em regra – uma topologia física em estrela e uma topologia lógica em anel.

2
Existe também a topologia híbrida, em que é possível ter uma topologia principal em anel e cada ramificação conectando várias estações em uma topologia de barramento.
TOPOLOGIA
BARRAMENTOESTRELA
ANELMALHA
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





24
132




5.3.1 – Barramento (Bus) INCIDÊNCIA EM PROVA: ALTA 
Nessa  topologia,
todas as estações ficam ligadas ao mesmo meio de transmissão em uma conexão ponto-multiponto, isto é, um único enlace (chamado backbone) compartilhado em que os nós se ligam através de conectores. Um sinal gerado por um nó de origem se propaga no barramento em ambas as direções (também conhecido como half-duplex) e pode ser recebido por todos os demais nós (também conhecido como broadcast).



Entre as vantagens, temos a facilidade de instalação e economia de cabeamento. Em outras palavras, como se trata de apenas de um conjunto de nós conectados a um único cabo, trata-se de uma fácil instalação, além de uma patente economia de cabeamento.
Entre as desvantagens, temos o aumento do atraso e o isolamento de falhas.
Como o link é compartilhado, quanto maior o número de máquinas, maior o atraso (delay) na comunicação e menor o desempenho da rede.

Além disso, uma falha ou ruptura no cabo de backbone implica a interrupção da transmissão, até mesmo  entre  os  dispositivos  que  se  encontram  do  mesmo  lado  em  que  ocorreu  o  problema.
Professor, não entendi muito bem!
Galera, imaginem que nós temos um varal com diversas roupas penduradas. Caso haja um rompimento do varal, todas as roupas caem; no entanto, se uma única roupa cair, nada acontece com o restante. É semelhante na topologia em barramento.

5.3.2 – Anel (Ring)
INCIDÊNCIA EM PROVA: média 
Nessa topologia, cada dispositivo tem uma conexão ponto-a-ponto com outros dois dispositivos conectados  lado  a  lado,  e  fazendo  uso  de  uma  comunicação  com  transmissão unidirecional (chamada simplex). Nesse caso, a mensagem circula o anel, sendo regenerada e retransmitida a cada nó, passando pelo dispositivo de destino que copia a informação enviada, até retornar ao emissor original. Nesse momento, o link é liberado para que possa ser utilizado pelo nó seguinte.



É similar às luzes de natal, mas com as pontas do cabo conectadas. Forma-se um anel em que os dados são transmitidos apenas em uma direção. Nessa topologia, um anel é relativamente fácil de Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





25
132




ser instalado e reconfigurado, com isolamento de falhas simplificado. Cada dispositivo é ligado apenas aos seus vizinhos imediatos. Acrescentar/eliminar um dispositivo exige apenas a mudança de conexões, mas há limitadores relacionados ao comprimento do anel e número de dispositivos.

Em um anel, geralmente, um sinal está circulando tempo todo. Se um dispositivo não receber um sinal dentro de um período especificado, ele pode emitir um alarme. Esse alarme alerta do operador sobre  o  problema  e  a  sua  localização.  Entretanto,  o  tráfego  unidirecional  pode  ser  uma desvantagem. Em um anel simples, uma interrupção no anel pode derrubar toda a rede.
Outro
problema: para que a informação chegue ao destinatário, ela tem de passar por todos os nós.

5.3.3 – Estrela (Star) INCIDÊNCIA EM PROVA: Altíssima 
Nessa topologia,
as estações são ligadas através de uma conexão ponto-a-ponto dedicada a um nó central
3
controlador, pelo qual passam todas as mensagens, não havendo tráfego direto entre os dispositivos. Notem que o enlace entre estações e o nó central é ponto-a-ponto. É a topologia mais usada atualmente por facilitar a adição de novas estações e a identificação ou isolamento de falhas, em que – se uma conexão se romper – não afetará as outras estações.



Observem que para que uma estação de trabalho envie uma informação para outra, haverá sempre uma passagem pelo nó central. Além disso, caso alguma estação tenha um defeito, não afeta o restante da rede. Por outro lado, temos um ponto único de falha, ou seja, se o dispositivo central  falhar,  toda  a  rede  será  prejudicada.  Para reduzir  essa  probabilidade,  utilizam-se dispositivos redundantes para que, caso algum pare de funcionar, o outro entra em ação.


5.3.4 – Malha (Mesh) INCIDÊNCIA EM PROVA: baixa 
Nessa topologia, cada estação de trabalha possui um link ponto a ponto dedicado com transmissão bidirecional (full-duplex) entre cada uma das demais estações. Colocando de outra forma, todas as estações de trabalho estão interligadas entre si, de modo que – caso haja uma ruptura em algum cabo – não se prejudica a rede como um todo, somente o nó conectado a esse cabo.
Entendido?

3
Nó central é um dispositivo que concentra conexões – em geral, ele liga os cabos dos computadores de uma rede (Ex: Hub ou Switch).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





26
132







Essa solução é boa para poucas máquinas, visto que com mais redundância a rede é mais confiável, mas é inviável para muitas máquinas, pois a redundância se tornaria muito cara. Pensa comigo:
Se um computador estiver ligado diretamente a outros cinco, nós precisaremos de cinco placas de rede e cinco cabos. Na verdade, para cada n computadores, são necessário n.(n-1)/2 cabos e n.(n- 1)
placas de rede. Para 20 computadores, seriam 190 cabos e 380 placas de rede!

(Telebrás – 2013) Na topologia de rede, conhecida como barramento, ocorre interrupção no  funcionamento  da  rede  quando  há  falha  de  comunicação  com  uma  estação  de trabalho.
_______________________ Comentários: conforme vimos em aula, há falha de comunicação somente se houver problema no cabo (backbone). Se houver problema em uma estação, não há problema (Errado).



Qual é a diferença entre arquitetura e topologia da rede?

Uma pergunta frequente no fórum de dúvidas é: qual é a diferença entre a arquitetura e a topologia de uma rede? A arquitetura trata apresenta a forma como os dispositivos de uma rede  se  comunicam:  se  é  diretamente  um  com  o  outro ou  se  é  por  meio  de  algum dispositivo central. Já a topologia trata da organização física (a forma como os dispositivos estão dispostos) ou da organização lógica (a forma como os dados fluem na rede).






Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





27
132




6 – Meios de Transmissão Um meio de transmissão, em termos gerais, pode ser definido como qualquer coisa capaz de transportar informações de uma origem a um destino. Por exemplo: o meio de transmissão para duas  pessoas  conversando  durante  um  jantar  é  o  ar; para  uma  mensagem  escrita,  o meio  de transmissão poderia ser um carteiro, um caminhão ou um avião.
Em telecomunicações, meios de transmissão são divididos em duas categorias: meios guiados e não-guiados.

TIPO DE MEIO DESCRIÇÃO GUIADO
Trata-se da transmissão por cabos ou fios de cobre, onde os dados transmitidos são  convertidos  em  sinais  elétricos  que  propagam  pelo  material  condutor.
Exemplo: cabos coaxiais, cabos de par traçado, fibra óptica, entre outros.
NÃO-GUIADO
Trata-se  da  transmissão  por  irradiação  eletromagnética,  onde  os  dados transmitidos são irradiados através de antenas para o ambiente. Exemplo: ondas de rádio, infravermelho, bluetooth e wireless.



(PC/AL  –  2012) Cabos  de  par  trançado,  coaxiais  e  fibras  ópticas  são  os  tipos  mais populares de meios de transmissão não guiados.
_______________________ Comentários: conforme vimos em aula, cabos de par trançado, coaxial e fibras ópticas são populares meios de transmissão de dados guiados, ou seja, são materiais que conduzem a informação enviada do transmissor ao receptor (Errado).














Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA ==12b2d8==






28
132




6.1 – Cabo Coaxial
INCIDÊNCIA EM PROVA: baixa 
Consiste em um fio central de cobre, envolvido por uma blindagem metálica. Isolantes de plástico flexível separam os condutores internos e externos e outras  camadas  do  revestimento  que  cobrem  a malha  externa.  Esse  meio  de  transmissão  é  mais barato, relativamente flexível e muito resistente à interferência  eletromagnéticas  graças  à  malha  de proteção  que  possui.  Esse  cabo  cobre  distâncias maiores  que  o  cabo  de  par  trançado  e  utiliza  um conector chamado BNC.

Foi utilizado até meados da década de 90 em redes  de  computadores,  quando  começou  a ser substituído pelo cabo de par trançado. Ele ainda é utilizado em telecomunicações, basta dar uma olhadinha no decodificador da sua TV por  Assinatura.
O  cabo  que  chega  na  sua casa/prédio  e  que  entra  em  um  modem  é geralmente um cabo coaxial – ele é capaz de
transportar sinais de Internet e TV.

Professor, eu acabei de olhar aqui e não entra nenhum cabo coaxial no meu computador! Parabéns, você foi olhar! O Cabo Coaxial do seu Pacote de TV/Internet vem da rua, entra na sua casa e é conectado ao modem e do modem saem dois cabos: um cabo de par trançado, que vai para o seu computador;  e  um  cabo  coaxial,  que  vai  para  o  Decodificador  de  TV. Bacana?  Outro  ponto interessante  é  que ele é capaz de cobrir longas distâncias, apesar de possuir  uma  taxa de transmissão menor que a de um cabo de par trançado . Compreendido? Então, vamos seguir...

(FUB – 2015) O cabo coaxial, meio físico de comunicação, é resistente à água e a outras substâncias corrosivas, apresenta largura de banda muito maior que um par trançado, realiza conexões entre pontos a quilômetros de distância e é imune a ruídos elétricos.
_______________________ Comentários: no universo de redes de computadores, largura de banda é a taxa de transferência de dados em uma rede, ou seja, a quantidade de bits por segundo que uma rede é capaz de suportar; no universo de comunicação via rádio, utiliza-se hertz.
Hoje em dia, todos possuem redes banda larga, ou seja, uma rede capaz de suportar uma taxa muito alta de bits/s.

O Cabo Coaxial, apesar de realizar conexões entre pontos a quilômetros de distância, não é imune a ruídos elétricos (apesar de ser muito resistente) e apresenta uma largura de banda menor que a largura de banda de um Cabo de Par Traçado. Ademais, ele é apenas relativamente resistente a substâncias corrosivas. Ele não vai resistir a ácido sulfúrico, né? (Errado).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





29
132




6.2 – Cabo de Par Trançado INCIDÊNCIA EM PROVA: ALTA 


Consiste de quatro pares de fios trançados blindados ou não, e envolto de um revestimento externo flexível. Eles são trançados para diminuir a interferência eletromagnética externa e interna – quanto mais giros, menor a atenuação. Este é o cabo mais utilizado atualmente por ser o mais barato de todos e ser bastante flexível. Esse cabo cobre distâncias menores que o cabo coaxial e utiliza um conector chamado RJ-45 (Memorizem!).

Quando é blindado, ele é chamado de Cabo STP (Shielded Twisted Pair) e quando não é blindado, ele é chamado de Cabo UTP (Unshielded Twisted Pair). Galera, esse é aquele cabinho azul que fica atrás do seu computador ligado provavelmente a um roteador. Sabe aquele cabo do telefone fixo da sua casa? Ele é mais fininho, mas ele também é um cabo de par trançado. Aliás, nós temos várias categorias de cabo de par trançado:

CATEGORIA VELOCIDADE ou taxa de dados FREQUÊNCIA DISTÂNCIA MÁXIMA CAT3
Até 10 MBPS 16 MHz 100 Metros CAT4 Até 16 MBPS 20 MHz 100 Metros CAT5
Até 100 MBPS 100 MHz 100 Metros CAT5e
Até 1000 MBPS (1G) 100 MHz 100 Metros CAT6 Até 10000 MBPS (10G) 250 MHz 100 Metros CAT6A
Até 10000 MBPS (10G) 500 MHz 100 Metros CAT7 Até 10000 MBPS (10G) 600 MHz 100 Metros CAT7A Até 10000 MPBS (10G) 1000 MHz 100 Metros CAT8
Até 40000 MBPS (40G) 2000 MHz 100 Metros 
Os cabos de par trançado possuem quatro pares de fios, sendo alguns utilizados para transmissão e outros para recepção, permitindo uma comunicação full duplex (como já vimos, ocorre nos dois sentidos e ao mesmo tempo). Para facilitar a identificação, os pares são coloridos e a ordem dos fios  dentro  do  conector  é  padronizada.  Eles  podem  ser  utilizados  na  transmissão  de  sinais analógicos ou digitais.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





30
132




(MEC – 2014) As redes de microcomputadores implementadas para apoiar as atividades de negócio das empresas utilizam os padrões Ethernet e Fast Ethernet, empregando hub e  switch  como  equipamentos  e  cabo  de  par  trançado  UTP,  além  de  conectores padronizados internacionalmente.

Nesse caso, por padronização, os conectores utilizados na implementação dessas redes, são conhecidos pela sigla:

a) BNC.
b) USB.
c) RJ-45.
d) RJ-11.
e) RG-58.
_______________________ Comentários: conforme vimos em aula, o conector utilizado com cabo de par trançado UTP/STP é o Conector RJ-45 (Letra C).




























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





31
132




6.3 – Cabo de Fibra Óptica INCIDÊNCIA EM PROVA: média 


Consiste em uma Casca e um Núcleo (de vidro) para transmissão de luz. Possui capacidade de transmissão  virtualmente  infinita,  é  imune  a  interferências  eletromagnéticas  e  consegue  ligar distâncias maiores sem a necessidade de repetidores. Como desvantagens, podemos dizer que é incapaz de fazer curvas acentuadas, além de ter um custo de instalação e manutenção muito alto em relação ao par trançado. Entendido? Há dois tipos de fibra:
Monomodo e Multimodo.

A Fibra Multimodo leva o feixe de luz por vários modos ou
caminhos, por uma distância menor, com menores taxas de transmissão, mais imprecisa, diâmetro maior e alto índice de refração e atenuação, mas possui construção mais simples, é mais barata e utilizada em LANs.

A Fibra Monomodo leva o feixe de luz por um único modo ou caminho
,  por  uma  distância  maior,  com  maiores  taxas  de transmissão, mais precisa, diâmetro menor e baixo índice de refração e atenuação, mas possui construção mais complexa, é mais cara e utilizada em WANs.

(EMBASA – 2014) A fibra ótica é composta basicamente de um núcleo de cobre e uma casca de plástico ou fibra de vidro concêntricos entre si. A transmissão de dados por meio de  fibra  ótica  é  realizada  pelo  envio  de  um  sinal  de  luz  codificado  imune  a  ruídos eletromagnéticos.
_______________________ Comentários: conforme  vimos  em  aula,  a  fibra  óptica  consiste  em uma  casca  e  um  núcleo  de  vidro  e,  não  cobre,  para transmissão de luz. Por outro lado, é realmente imune a ruídos eletromagnéticos (Errado).






Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





32
132




7 – Equipamentos de Redes Galera,  chegou  a  hora  de  falar  rapidamente  sobre  os  principais  equipamentos  de  redes.  Vem comigo, rapidinho a gente mata esse assunto...

7.1 – Network Interface Card (NIC ou Placa de Rede) INCIDÊNCIA EM PROVA: baixíssima 


Galera, essa é a famosa Placa de Rede 4
! Se vocês olharem na parte de trás do gabinete de um computador, vocês a verão (provavelmente com o cabo azul de par trançado conectado a ela). Ela é o recurso de hardware mínimo que deverá estar instalado no computador para permitir uma comunicação bidirecional – transmissão e recebimento de dados – com os demais elementos da rede. Agora vejam que coisa interessante...


Você tem um CPF, que é um número único que te identifica. Por que? Porque não existe outra pessoa no mundo com esse mesmo número.
Da mesma forma, as Placas de Rede possuem um identificador  único  chamado  Endereço  MAC  (Medium  Access  Control)  –  é  como  se fosse  o número de série do dispositivo.
Esse endereço físico é representado por 48 bits, representados em hexadecimal e separados por dois-pontos (Ex: 00:1C:B3:09:85:15).

(UFMA – 2018) Para que um computador possa se conectar a uma LAN (Local Area Network) é necessário que ele possua um(a):

a) codificador.
b) webcam.
c) impressora.
d) placa de rede.
e) placa de som.
_______________________ 
4
As placas de rede podem também ser chamadas de Placas NIC. Além disso, a imagem à esquerda mostra uma placa de rede cabeada e a imagem à direita mostra uma placa de rede wireless.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





33
132




Comentários: conforme vimos em aula, trata-se de uma Placa de Rede (Letra D).

(UFRB – 2015) O hardware de computador, além da unidade central de processamento e  da  memória,  é  composto  de  dispositivos  de  entrada  e  saída,  que  permitem  a comunicação com o usuário. O dispositivo padrão de entrada é o teclado e o dispositivo padrão de saída é o monitor. Alguns dispositivos são chamados híbridos porque podem funcionar tanto como dispositivo de entrada e como de saída. Qual alternativa é um exemplo de dispositivo híbrido (de entrada e saída)?

a) Microfone.
b) Mouse.
c) Alto Falante.
d) Scanner.
e) Placa de rede.
_______________________ Comentários: conforme vimos em aula, a placa de rede permite uma comunicação bidirecional (transmissão e recebimento de dados). Logo, é um dispositivo híbrido de entrada/saída de dados (Letra E).

(UFBA – 2012) Uma placa de rede Wi-Fi é um dispositivo de entrada e saída.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita – dados entram e saem da placa de rede wi-fi (Correto).




















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





34
132




7.2 – Hub (Concentrador) INCIDÊNCIA EM PROVA: média 
Trata-se de um dispositivo para interligação de computadores que tem o objetivo de aumentar o alcance de uma rede local por meio da regeneração de sinais, porém recebe em uma única porta e retransmite para todas as outras. Este equipamento disponibiliza várias portas físicas para que os nós sejam interligados, por exemplo, através de cabos par trançado com conectores RJ-45. Atualmente, esse equipamento está obsoleto e quase não é mais comercializado.

O Hub é considerado um dispositivo “burro” por trabalhar apenas com broadcast. Como assim, professor?
Ao receber dados,
ele os distribui para todas as outras máquinas – ele não é capaz de transmitir dados somente para uma máquina específica , implicando que apenas uma máquina transmita de cada vez para evitar colisões. A transmissão broadcast faz com que uma rede com Hub possua uma topologia física de Estrela e uma topologia lógica de Barramento.

Em suma: o hub (concentrador) é um equipamento de rede que permite concentrar o tráfego de rede que provém de vários dispositivos e regenerar o sinal . O seu único objetivo é recuperar os dados que chegam a uma porta e enviá-los para todas as demais portas. Aliás, ele pode ter dezenas de portas – quantas forem necessárias para conectar os dispositivos de uma rede. A representação de um Hub é apresentada abaixo:


(Prefeitura de Jandira/SP – 2016) Numa rede de computadores, do tipo estrela, existe um dispositivo que permite transmitir dados a todos computadores conectados à rede ao mesmo tempo. Esse dispositivo é denominado tecnicamente de:

a) hub.
b) modem.
c) bridge.
d) firewall.
_______________________ Comentários: conforme vimos em aula, o dispositivo conhecido por trabalhar apenas com broadcast, isto é, transmitir dados a todos os computadores de uma rede ao mesmo tempo é o Hub (Letra A).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





35
132





(SEFAZ/PB – 2006) Dispositivo físico que tem por função básica apenas interligar os computadores  de  uma  rede  local.  Recebe  dados  vindos  de  um  computador  e  os transmite às outras máquinas. Conhece-se também por concentrador:

a) o parser.
b) o hub.
c) o router.
d) a bridge.
e) o gateway.
_______________________ Comentários: conforme vimos em aula, trata-se do Hub (Letra B).

(PC/PI – 2014) O equipamento que serve para interligar computadores em uma rede local, para compartilhamento de dados, é denominado de:

a) hub.
b) modem.
c) no-break.
d) impressora.
e) pendrive.
_______________________ Comentários: conforme vimos em aula, trata-se do Hub (Letra A).

(Câmara Municipal de Paraíso do Norte/PR – 2013) Marque a baixo a alternativa que corresponde  a  um  dispositivo  (hardware)  de  redes  de  computadores  que  permite  o compartilhamento de recursos.

a) Winzip
b) USP
c) Hub
d) NetBios
e) RJ45
_______________________ Comentários: conforme vimos em aula, trata-se do Hub (Letra C).





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





36
132




7.3 – Bridge (Ponte) INCIDÊNCIA EM PROVA: baixíssima 
Permite conectar segmentos de redes diferentes que podem ou não  utilizar  tecnologias/protocolos  de  enlace  distintos  (Ex:
Ethernet,  Token  Ring,  etc). O  que  é  um  segmento  de  rede? É simplesmente subdivisão de uma rede. Vejam abaixo que uma rede foi  separada  em  dois  segmentos:  Segmento  A  e  Segmento  B.
Como a rede foi segmentada, nós temos uma redução no tráfego e uma menor chances de colisões.

Como assim uma redução no tráfego? Galera, os dados transmitidos para um segmento agora são enviados apenas para os computadores específicos e, não, para todos os computadores da rede – como ocorria com  o  Hub!  Lembrem-se  que  o  Hub  envia  dados  para  todos computadores  da  rede  indiscriminadamente.  Logo  o  tráfego  na  rede reduz e a chance de colisões também.

As informações manipuladas por uma Bridge são chamadas de quadros ou frames – assim como no Switch.
Aliás, uma desvantagem das Bridges é que elas geralmente só possuem duas portas, logo só conseguem separar a rede em dois segmentos. Em contraste com o Switch, que veremos a seguir, que é conhecido como Bridge Multiporta por ter várias portas e suportar várias segmentações . A representação de uma Bridge é apresentada abaixo:



Em suma: uma bridge é um equipamento de rede que permite conectar redes diferentes que podem utilizar tecnologias/protocolos de enlace distintos em segmentos menores, permitindo filtrar os quadros de forma que somente passe para o outro segmento da bridge dados enviados para algum destinatário presente nele.
Em contraste com o hub, que envia dados em broadcast, a bridge é capaz de enviar dados em unicast – para um destinatário específico.
(CFM  –  2018  –  Adaptada) Uma  bridge  é  um  dispositivo  usado  para  conectar  dois segmentos de rede diferentes e enviar quadros de um segmento ao outro de forma transparente.
_______________________ Comentários: conforme vimos em aula, ela realmente conecta dois segmentes de rede diferentes. Além disso, ela envia quadros (dados) de um segmento a outro. Professor, o que é essa forma transparente? Transparente significa que não se enxerga! Sabe quando você vai aos Correios e paga para entregar um pacote na casa de alguém? Se o pacote vai de avião, navio ou carro não importa para você, logo o método de entrega é transparente para o cliente (ele não enxerga o método). No caso da questão, a Bridge envia quadros de um segmento ao outro de forma transparente, isto é, ela consegue enviar dados de um segmento para outro como se estivessem todos em um mesmo segmento sem problema algum (Correto).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





37
132




7.4 – Switch (Comutador) INCIDÊNCIA EM PROVA: média 



Também conhecido como comutador, o switch é uma evolução do hubs! Eles são inteligentes, permitindo fechar canais exclusivos de comunicação entre a máquina que está enviando e a que está recebendo –
em unicast  ou multicast.  Em  outras  palavras,  o  switch  –  diferente  do  hub  –  é  capaz  de  receber  uma informação de fora e enviá-la apenas ao destinatário. Ele não é como o hub, que recebia uma informação de fora e a repassava para todo mundo que estivesse na rede.

Hub é um amigo fofoqueiro: se ele recebe uma mensagem, ele conta para todo mundo. Switch é um amigo leal: se ele recebe uma mensagem, ele conta apenas para o destinatário daquela informação. Além disso, o Hub funciona apenas em uma via por vez (half-duplex) e o Switch funciona – em geral – em duas vias (full duplex). Dessa forma, a rede fica menos congestionada com o fluxo de informações e é possível estabelecer uma série de conexões paralelas.

Por  fim,  a  segmentação  realizada  pelo  dispositivo  possibilita  que  diferentes  pares  possam  conversar simultaneamente na rede, sem colisões. A transmissão para canais específicos faz com que uma rede com switch possua topologia física e lógica em estrela.
Ademais, um switch possui mais portas disponíveis que um hub ou uma ponte, o que – em uma rede com muitos computadores – faz a diferença na hora de distribuir o sinal de internet via cabo.


Em suma: um switch (comutador) é um equipamento de rede semelhante a uma ponte com múltiplas portas, capaz de analisar dados que chegam em suas portas de entrada e filtrá-los para repassar apenas às portas específicas de destino . Além disso, ele é capaz de funcionar em full duplex. A representação de um Switch é apresentada abaixo:



(Prefeitura de Araraquara/SP – 2017) Em uma rede de computadores, que é utilizada a topologia  em  estrela,  existe  a  necessidade  de  se  utilizar  o  equipamento  de  rede denominado em inglês como:

a) gateway   b) switch    c) modem   d) bridge _______________________ Comentários: conforme vimos em aula, trata-se do Switch (Letra B).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





38
132




7.5 – Router (Roteador) INCIDÊNCIA EM PROVA: ALTA 


Os roteadores são
equipamentos que permitem interligar várias redes e escolher a melhor rota para que a informação chegue ao destino. Esse dispositivo encaminha ou direciona pacotes de dados entre redes de computadores, geralmente funcionando como uma ponte entre redes diferentes. Hoje em dia, são muito comuns em residências para permitir que a Rede LAN doméstica possa acessar outra rede – em geral, a Internet. Entendido?

Talvez  você  tenha  um  na  sua  casa, é  aquele  geralmente  com  as  anteninhas  e  permite  que  você compartilhe a conexão de internet com dois ou mais aparelhos – ele é o principal responsável por controlar  o  tráfego  da Internet.  Pessoal,  roteadores  domésticos  geralmente  possuem  apenas  quatro portas,  então  você  pode  conectar  apenas  quatro  dispositivos  a  eles.  Em  uma  empresa  com  vários computadores, utilizam-se roteadores com mais portas ou conecta-se a um switch!

Nesse caso, o sinal da internet virá de seu provedor de acesso por meio de um cabo conectado ao roteador.
Como ele não possui portas suficientes, você pode conectar o roteador a um switch – que geralmente possui várias  portas.
Os  computadores  e  outros  dispositivos  (impressora, servidores,  etc)  podem  ser conectados ao switch! Por fim, você pode utilizar o seu roteador no modo Access Point, caso queira utilizá- lo somente para aumentar o sinal da rede wireless.

A imagem a seguir mostra uma configuração muito comum de redes locais domésticas. Temos um roteador responsável por compartilhar a internet com outros dispositivos. Como ele possui poucas portas e nós temos  seis  computadores,  essa  rede  foi  separada  em dois  segmentos  por  meio  de  dois  switches.
Roteadores conectam redes diferentes; switches segmentam uma mesma rede. Além disso, um switch forma uma rede entre os notebooks e um outro switch forma uma rede entre os computadores...
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





39
132






(Prefeitura de João Pessoa/PB – 2016) Um  equipamento  de  rede  que  permite  que computadores de uma rede possam se conectar a Internet é o:

a) HDCD.
b) pen drive.
c) roteador.
d) scanner.
e) VGA.
_______________________ Comentários: conforme  vimos  em  aula,  o  dispositivo  responsável  por  permitir  a  conectividade  entre  dispositivos  como computadores, smartphones, tablets, etc em uma Rede LAN com a internet é o Roteador (Letra C).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





40
132




7.6 – Access Point (Ponto de Acesso) INCIDÊNCIA EM PROVA: média 


Estamos na época dos combos! Hoje em dia, um Provedor de Internet é também um Provedor de TV a Cabo (Ex: NET/Claro, GVT/Vivo, etc). Imaginemos que você contrate um desses serviços:
um técnico virá até sua residência, fará alguns furos, passará um cabo coaxial branco pela parede e o conectará a um modem que estará na sala da sua casa – esse equipamento permitirá que você tenha acesso à Internet Banda Larga.

Nos  dias  atuais,  esse  modem  também  faz  a  função  de um  Roteador Wireless!  E,  assim,  você finalmente terá acesso sem fio e não terá que se preocupar em ligar cabo algum ao seu notebook.
No entanto, há um problema: quando o técnico foi embora, você percebeu que – ao se deslocar da sala e foi para o quarto – o sinal wireless no seu celular piorou vertiginosamente.
É aí que entra o
Access Point (em tradução livre, Ponto de Acesso).

Ele é um dispositivo de rede utilizado para estender a cobertura de redes de internet sem fio. O Access Point é o dispositivo que vai ajudar a manter o sinal na sala, cozinha, garagem, etc – ele pode ser compreendido como uma espécie de repetidor de sinal wireless. Façam um experimento social:
a próxima vez que vocês forem a algum local que ofereça wireless para o público geral, olhem para o teto ou para as paredes (Ex: Aeroporto, Universidade, Estádios, entre outros)!

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





41
132




Eu tenho total certeza que vocês encontrarão vários dispositivos como esses da imagem acima.
Façam esse experimento e me contem no fórum se vocês encontraram ou não! Bem, o que eles estão fazendo ali?
Eles estão estendendo, aumentando, distribuindo, repetindo o sinal wi-fi por todas as localidades. Dessa forma, todo mundo nesse local possui um ponto de acesso (em inglês, Access Point) à internet sem fio.

Por fim, é importante mencionar que o Access Point é apenas um extensor de sinal wi-fi. Dessa maneira,
ainda é necessário possuir um roteador, uma vez que o roteador é o responsável por conectar diversos dispositivos de uma rede local à internet. Em outras palavras, um roteador wireless pode até trabalhar como um Access Point, mas um Access Point não pode trabalhar como roteador. Bacana?



Qual é a diferença entre um Roteador e um Access Point?

Uma pergunta frequente no fórum de dúvidas é: qual é a diferença entre um Roteador e um Access Point? A função principal de um Roteador é conectar dispositivos de uma rede local à Internet. Já a função principal de um Access Point é oferecer acesso sem fio à internet, mas ele também pode ser utilizado para estender o alcance do sinal de internet.
Eventualmente  um  pode  realizar  algumas  funções  do  outro,  mas  são  dispositivos diferentes.

(Prefeitura de Araraquara/SP – 2018) Um Analista comprou um roteador wireless e o conectou por cabo em um switch para acessar a estrutura de rede cabeada. Isso permitiu que todos os dispositivos sem fio conectados nesse roteador tivessem acesso a todos os serviços disponíveis na rede cabeada, como por exemplo, acesso à internet. Nesse caso, o roteador foi configurado pelo Analista para operar no modo:

a) ponto-a-ponto.
b) access point.
c) bridge.
d) modem.
e) backbone.
_______________________ Comentários: conforme vimos em aula, trata-se do Access Point (Letra B).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





42
132




(MPE/CE – 2013) Na empresa em que Paulo trabalha, o link de internet banda larga é recebido em um modem Wi-Fi da marca Motorola SVG 1202 que permite que vários computadores utilizem a internet simultaneamente, compartilhando a velocidade. Isso torna possível conectar-se à internet de tablets, smartphones e notebooks. Porém, o alcance do sinal do modem Wi-Fi não atinge algumas áreas da empresa que necessitam de acesso à internet. Para resolver esse problema, Paulo sugeriu a utilização de um equipamento  que,  além  de  poder  ser  conectado  a  uma rede  cabeada  para  fornecer acesso sem fio a ela, também pode ser utilizado para estender o alcance do sinal do modem  Wi-Fi  para  as  áreas  da  empresa  que  precisam  de  acesso  à  internet.  O equipamento sugerido por Paulo é denominado:

a) access point.
b) hub.
c) switch.
d) filtro de linha.
e) bridge.
_______________________ Comentários: conforme vimos em aula, trata-se do Access Point (Letra A).

























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





43
132




7.7 – Modem
INCIDÊNCIA EM PROVA: média 


Galera, imaginem que eu preciso enviar um e-mail para o Prof. Renato!
Para que essa mensagem saia do meu computador e chegue no computador dele, é necessário que ela seja transmitida por um meio de comunicação . Pode ser através de fibras ópticas, ondas de rádio, entre outros – no entanto há uma alternativa interessante de infraestrutura que já existe na imensa maioria dos lugares. Qual, professor? A infraestrutura de linha telefônica!

Isso não é tão simples assim, porque os computadores possuem uma linguagem diferente da linguagem  dos  telefones.  Quando  eu  envio  um  e-mail  para  o  Prof.  Renato,  a mensagem  é convertida  em  um  conjunto  de  dígitos  binários  (Ex: 0111010001000111010).  Os  telefones  não conseguem entender essa linguagem porque eles utilizam sinais analógicos que, inclusive, não são entendidos por computadores. É como se um falasse húngaro e o outro aramaico!

Como resolver esse problema?
Evidentemente nós precisamos de um tradutor! E é aí que entra o papel do Modem (
Modulador/Demodulador). Esse dispositivo converterá os dígitos binários do meu  computador  em  sinais  analógicos  que  podem  ser  transmitidos  em  linhas  telefônicas;  e também converterá os sinais analógicos das linhas telefônicas em dígitos binários. Ficou mais fácil de entender agora? Então vamos ver a definição...

O Modem é um dispositivo eletrônico de entrada/saída de dados que modula um sinal digital em um sinal analógico a ser  transmitida  por  meio  de  uma  linha  telefônica  e que demodula o sinal analógico e o converte para o sinal digital original.
Hoje em dia, existem basicamente três tipos:
Acesso Discado, Modem ADSL e Cable Modem .

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





44
132




O Modem de Acesso Discado é inserido na placa-mãe do seu computador. Quem aí é mais velho sabe que antigamente a internet era bem lenta e muito cara! Sabe como eu fazia para me conectar à internet? Eu esperava passar de meia-noite (porque o minuto cobrado ficava bem mais barato), desconectava o cabo do telefone fixo e conectava esse mesmo cabo no modem de acesso discado na parte de trás do gabinete do computador. O telefone, é claro, parava de funcionar!

Depois disso, você abria um discador e tinha que fazer infinitas tentativas para conseguir se conectar! Quando você finalmente conseguia, você ficava todo feliz, mas demorava mais ou menos uns dois minutos para abrir qualquer página na internet e quando ela estava quase toda aberta... a conexão caía! É, criançada... a vida era um bocado mais difícil, mas era divertido! Deixa eu contar uma historinha que aconteceu comigo...

Naquela época, poucas pessoas tinham condição de possuir um celular. Se você quisesse falar com alguém, teria que ligar em um telefone fixo e torcer para que o destinatário estivesse no local. Minha irmã mais velha estava grávida de nove meses e eu – aos 13 anos – estava doido para que chegasse meia-noite,
assim eu poderia acessar à internet de graça e ler meus fóruns sobre o jogo que virou febre na época: Pokemon (vejam a imagem abaixo).

Como  vocês  sabem,  ao  se  conectar  utilizando  um Modem Dial-Up, o telefone ficava ocupado. Você não conseguiria ligar para ninguém e, se alguém te ligasse, ouviria o sinal de ocupado. Ocorre que a bolsa da minha irmã estourou e nem ela nem o esposo possuíam carro, logo ela ligou para minha mãe buscá-la. O que aconteceu?
Tu-tu-tu-tu-tu  –  sinal  de  ocupado  porque  eu  estava vendo meus fóruns. Tomei uma surra monumental: sim ou não?  Pois  é!  Ainda  bem  que  ela  conseguiu  outro transporte  e  meu  sobrinho  está  hoje  com  18  anos!
Finalmente, chegaram os Modens ADSL.

Eles ofereciam acesso em banda larga por meio de cabos ou wireless. Pessoal, era muito mais rápido (velocidade de download/upload) e não ocupavam o telefone, ou seja, você podia utilizar o telefone e a internet simultaneamente. Por fim, temos o Modem Cabeado (Cable Modem)! Eles não utilizam  as  linhas  telefônicas  –  eles  são  conectados  por  meio  de  cabos  coaxiais  normalmente fornecido pela sua fornecedora de TV a Cabo. Como é, professor?

Você tem NET ou GVT? Pois é, elas te oferecem serviços diferentes! Um serviço interessante é o combo: TV, Internet e Telefone! Em vez de utilizar três meios para te fornecer cada um desses serviços, ela transmite todos esses dados via cabo coaxial. Algumas vezes, esse modem virá com um roteador acoplado internamente; outras vezes, você terá que comprar um roteador e utilizar ambos para ter acesso à internet. Entendido? Então vamos seguir...


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





45
132




(Correios – 2011) O modem:

a) é um tipo de memória semicondutora não volátil.

b)  é  um  tipo  de  interface  paralela  que  permite  a  comunicação  sem  fio  entre  um computador e seus periféricos.

c) é um roteador wireless para redes sem fio.

d)  tem  função  de  garantir  o  fornecimento  ininterrupto  de  energia  elétrica  ao computador.

e) pode auxiliar na comunicação entre computadores através da rede telefônica.
_______________________ Comentários: conforme vimos em aula, o modem pode auxiliar na comunicação entre computadores através da rede telefônica (Letra E).

(DEPEN – 2013) Quais as características a tecnologia de conexão à Internet denominada ADSL:

a) Conexão permanente, custo fixo, linha telefônica liberada e velocidade maior do que as linhas tradicionais.

b) Conexão permanente, custo variável, linha telefônica liberada e velocidade maior do que as linhas tradicionais.

c) Conexão permanente, custo fixo, linha telefônica não liberada e velocidade maior do que as linhas tradicionais.

d) Conexão não-permanente, custo variável, linha telefônica liberada e velocidade igual às linhas tradicionais.

e) Conexão não-permanente, custo fixo, linha telefônica não liberada e velocidade igual às linhas tradicionais.
_______________________ Comentários: conexão permanente – ADSL permite que você se mantenha sempre conectado, em contraste com as linhas tradicionais (Ex: Dial-up) em que – para acessar a internet – precisa se conectar; custo fixo – ADSL possui um custo fixo, visto que você não paga mais por conta do horário, etc, em contraste com linhas tradicionais em que você paga valores adicionais a depender do horário; linha telefônica liberada – ADSL permite que se utilize a internet e o telefone simultaneamente, em contraste com linhas tradicionais em que você ou utiliza a internet ou utiliza o telefone; velocidade maior do que as linhas tradicionais – ADSL possui a grande vantagem de permitir uma velocidade (muito) maior do que as linhas tradicionais (Letra A).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





46
132




8 – Padrões de Redes Seus lindos... existe lá nos Estados Unidos um instituto bastante famoso chamado IEEE (Institute of Electrical and Electronics Engineers)! Trata-se da maior organização profissional do mundo dedicada ao avanço da tecnologia em benefício da humanidade. Esse tal de IEEE (lê-se “I3E”) mantém o Comitê 802, que é o comitê responsável por estabelecer padrões de redes de computadores .
Professor, o que seriam esses padrões de redes?

Padrões de Redes são uma especificação completamente testada que é útil e seguida por aqueles que trabalham com Internet – trata-se de uma regulamentação formal que deve ser seguida.
O
Padrão IEEE 802 é um grupo de normas que visa padronizar redes locais e metropolitanas nas camadas física e de enlace do Modelo OSI. Na tabela a seguir, é possível ver diversos padrões diferentes de redes de computadores:

PADRÃO NOME
IEEE 802.3
Ethernet (LAN)
5

IEEE 802.5
Token Ring (LAN)
IEEE 802.11 Wi-Fi (WLAN) IEEE 802.15
Bluetooth (WPAN)
IEEE 802.16 WiMAX (WMAN) IEEE 802.20 Mobile-Fi (WWAM) 
(UFMA – 2016) Considerando os padrões Ethernet em uso utilizados pela maioria das tecnologias  de  rede  local,  permitindo  que  a  integração  de  produtos  de  diferentes fabricantes funcionem em conjunto. Qual das alternativas diz respeito ao padrão 802.11?

a) Redes Token King
b) redes Wi-Fi
c) redes Cabeada
d) redes bluetooth
e) Redes WIMAX
_______________________ Comentários: conforme vimos em aula, o Padrão 802.11 se refere a Redes Wi-Fi (Letra B).






5
Para lembrar da numeração do Padrão Ethernet (que é o mais importante), lembre-se de: ETHERNET 
3TH3RN3T.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





47
132




8.1 – Padrão Ethernet (IEEE 802.3) INCIDÊNCIA EM PROVA: ALTA 
Ethernet é um conjunto de tecnologias e padrões que permite que dois ou mais computadores se comuniquem utilizando meios cabeados em uma Rede de Área Local (LAN). Dessa forma, eu gostaria que vocês me respondessem: (1) Vocês moram ou trabalham em um local com até cerca de 1000 m²? (2) No local que vocês moram ou trabalham, vocês possuem acesso à internet? (3) O acesso à internet se dá por algum cabo ligado ao seu computador?

Se vocês responderam afirmativamente para as três perguntas anteriores, isso significa que a rede de computadores de vocês é regida pela Ethernet. Bacana? Em sua forma mais simples, ela é um conjunto de computadores conectados a um único cabo comum. Quando um computador deseja transmitir dados a outro computador, ele traduz os dados em sinais elétricos e os envia pelo cabo – como mostra a imagem à esquerda.



Como vocês podem notar, como o cabo é compartilhado, todo computador que estiver conectado à rede conseguirá visualizar a transmissão de dados, mas não saberá se os dados eram destinados a  ele  ou  a  outro  computador.
Para  resolver  esse  problema,  a  Ethernet  requer  que cada computador tenha um único endereço de Media Access Address (MAC) – também chamado Endereço MAC.
Bacana?



Esse endereço único é colocado junto com os dados a serem transmitidos (como se fosse um prefixo).
Assim, computadores na rede continuam recebendo os dados, mas só os processam quando eles percebem que é o endereço deles que está contido no prefixo . Vejam acima que o
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





48
132




Computador A deseja enviar uma mensagem para o Computador F. Para tal, ele coloca o Endereço MAC do Computador F na mensagem, que será processada por esse computador e ignoradas pelos outros. Todo computador vem com seu Endereço MAC – que é único no mundo!

O termo genérico para essa abordagem vista acima é Carrier Sense Mutiple Access (CSMA), também conhecido como acesso múltiplo por portadora. Professor, o que é essa portadora? Nesse caso, é qualquer meio de transmissão compartilhado capaz de transmitir dados – cabos de cobre para Redes Ethernet ou o ar para Redes Wi-Fi. A taxa que um meio de transmissão pode transmitir dados é conhecida como Largura de Banda – vocês já devem ter ouvido falar!

Infelizmente, utilizar um meio de transmissão compartilhado  possui  uma  desvantagem:
quando  o  tráfego  na  rede  está  baixo, computadores podem simplesmente esperar que  ninguém  esteja  utilizando  o  meio  de transmissão  e  transmitir  seus  dados.  No entanto, à medida que o tráfego aumenta, a probabilidade   de   que   dois   ou   mais computadores  tentem  transmitir  dados  ao mesmo  tempo  também  aumenta.
Quando
isso ocorre, temos uma colisão!

A colisão deixa os dados todos ininteligíveis, como duas pessoas falando ao telefone ao mesmo tempo  –  ninguém  se  entende!  Felizmente,  computadores  podem  detectar  essas  colisões  ao “sentirem” os sinais elétricos no cabo de transmissão – chamado Collision Detection. A solução mais óbvia para resolver esse problema é a mesma para quando duas pessoas falam simultaneamente ao telefone:
parar a transmissão, esperar em silêncio e tentar novamente.

O problema é que o outro computador também vai tentar a mesma estratégia. Além disso, outros computadores da mesma rede podem perceber que o meio de transmissão está vazio e tentar enviar seus dados. Vocês percebem que isso nos leva a mais e mais colisões? Pois é, mas a Ethernet possui  uma  solução  simples  e  efetiva  para  resolver esse  problema.
Quando  um  computador detecta uma colisão, eles esperam um breve período de tempo antes de tentar novamente.

Esse período poderia ser, por exemplo, um segundo! Professor, se todos os computadores esperarem um segundo, isso não vai resultar no mesmo problema anterior? Você está esperto, meu caro! Isso é verdade, se todos esperarem um segundo para retransmitir, eles vão colidir novamente após um segundo. Para resolver esse problema, um período aleatório é adicionado: um computador espera 1,3 segundos; outro espera 1,5 segundos; e assim por diante.

Lembrem-se que – para o mundo dos computadores – essa diferença de 0,2 segundos é uma eternidade. Logo, o primeiro computador verá que o meio de transmissão não está sendo utilizado e pode transmitir seus dados. 0,2 segundos depois, o segundo computador verá que o meio de Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





49
132




transmissão não está sendo utilizado e poderá transmitir seus dados. Professor, calma aí, isso ajuda bastante, mas se tivermos muitos computadores não resolverá o problema!

Para resolver esse problema, nós temos mais um truque! Sabemos que se um computador detecta uma colisão, ele esperará um segundo mais um tempo aleatório. Se mesmo assim houver outra colisão, pode ser que a rede esteja congestionada, logo ele não esperará mais um segundo, esperará dois segundos. Se mesmo assim houver colisão, esperará quatro segundos.
Se continuar havendo colisões, esperará oito segundos, e assim por diante até conseguir transmitir.

Sabe quando sua internet está lenta?
Pode ser que o motivo seja o congestionamento do meio de transmissão por conta dessas colisões! Legal, não é?  Você,  meu  melhor  aluno,  vai  continuar argumentando  que  isso  não  resolve  o  problema  para  muitos  computadores.  Imaginem  uma universidade inteira com 1000 alunos acessando simultaneamente a rede local em um, e apenas um, cabo compartilhado. Complicado, não é?

Para  reduzir  o  número  de  colisões  e  melhorar  a  eficiência,  nós  precisamos  diminuir  a quantidade de dispositivos nos meios de transmissão compartilhados – chamado Domínio de Colisão. No nosso exemplo anterior, nós tínhamos seis computadores conectados em um único meio de transmissão compartilhado, logo nós tínhamos um único domínio de colisão. Para reduzir a probabilidade de colisões, nós podemos segmentar a rede em dois domínios de colisão.



Para  tal,  podemos  utilizar  um  dispositivo  chamado  Switch  –  visto  anteriormente.  Ele segmentará nossa rede em duas partes e será posicionado entre elas. Dessa forma, ele só passa dados para o outro domínio de colisão se a mensagem for destinada a algum computador presente nesse domínio de colisão. Como ele faz isso, professor? Ele guarda uma lista de Endereços MAC dos computadores de cada rede.

Dessa forma, se o Computador A deseja transmitir dados para o Computador C, o switch não encaminhará os dados para a outra rede – como mostra a imagem abaixo à esquerda. Da mesma forma, se o Computador E quiser transmitir dados para o Computador F ao mesmo tempo que o Computador A transmite dados para o Computador C, a rede estará livre e as duas transmissões poderão ocorrer simultaneamente – como mostra a imagem abaixo à direita.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





50
132






No entanto, se o Computador F quiser transmitir dados para o Computador A, o switch poderá atravessar os dados de uma rede para outra e ambas as redes estarão brevemente ocupadas.
Galera,  é  assim  que  as  grandes  redes  funcionam,  isto  é,  interconectando  dispositivos.
É
interessante mencionar que em redes grandes – como a Internet – existem geralmente diversos caminhos diferentes para transmitir dados de um local para outro. Agora vamos ver os padrões:



EVOLUÇÃO DOS PADRÕES ETHERNET PADRÃO (CABO COAXIAL) PADRÃO – TAXA DE TRANSMISSÃO - DISTÂNCIA Ethernet 10BASE-2 / 10 Mbps / 185 Metros Ethernet 10BASE-5 / 10 Mbps / 500 Metros 
EVOLUÇÃO DOS PADRÕES ETHERNET PADRÃO (CABO DE PAR TRANÇADO) PADRÃO – TAXA DE TRANSMISSÃO Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





51
132




Ethernet 10BASE-T / 10 Mbps Fast Ethernet 100BASE-T / 100 Mbps Gigabit Ethernet 1000BASE-T / 1000 Mbps 10G Ethernet 10GBASE-T / 10000 Mbps 

Como 1 bilhão = 1000 milhões, então 1G = 1000M. Dessa forma, fica mais fácil lembrar que a Gigabit Ethernet tem a velocidade de 1000Mbps e que a 10G Ethernet tem a velocidade de 10.000Mbps (lembrando também que MEGA (M) = Milhão e GIGA (G) = Bilhão.
(SEFAZ/RJ  –  2008) Uma  rede  de  microcomputadores  opera  com  base  no  padrão Ethernet IEEE-802.3 e utiliza o protocolo CSMA/CD. No momento em que uma colisão é detectada, as máquinas que estão transmitindo executam o seguinte procedimento:

a) aceleram o ritmo de transmissão.
b) param imediatamente de transmitir.
c) passam a transmitir em modo half-duplex.
d) retransmitem os frames que provocaram a colisão.
e) enviam pacotes de sincronismo para as demais máquinas.
_______________________ Comentários: conforme vimos em aula, a regra é parar imediatamente de transmitir e aguardar uma fração de tempo aleatória para reiniciar a transmissão (Letra B).

(TCE/CE – 2015) As taxas nominais de transmissão definidas em bits por segundo de 10M, 1000M, e 100M são, respectivamente, atribuídas aos padrões:

a) Fast Ethernet, Ethernet e Gigabit Ethernet;
b) Ethernet, Gigabit Ethernet e Fast Ethernet;
c) Gigabit Ethernet, Ethernet e Fast Ethernet;
d) Fast Ethernet, Ethernet e Gigabit Ethernet.
_______________________ Comentários: conforme vimos em aula, 10M é a taxa atribuída à Ethernet; 1000M é a taxa atribuída à Gigabit Ethernet; e 100M é a taxa atribuída a Fast Ethernet (Letra B).





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





52
132




8.2 – Padrão Token Ring (IEEE 802.5) INCIDÊNCIA EM PROVA: média 
O Padrão Token Ring é outro padrão cabeado e foi, até o início da década de 90, o principal concorrente do Padrão Ethernet, quando possuía taxa de transmissão de dados de 4 Mbps, comunicação unidirecional (chamada simplex), arquitetura ponto-a-ponto e topologia lógica em anel
. Por falar nisso, quando falamos em Topologia em Estrela, havia um risco de colisão – no Padrão Token Ring esse risco não existe!

Por que esse padrão se chama Token Ring? Isso ocorre basicamente porque cada estação de trabalho dessa rede de computadores se conecta com a adjacente até fechar um circuito fechado chamado Anel  (Ring).  Para  que  uma  estação  de  trabalho  possa  transmitir  dados  para  outra  estação  de trabalho,  ela  precisa  possuir  uma  espécie  de  envelope  chamado token  –  pronto, descobrimos
porque se chama Token Ring.

Processo de Funcionamento 
O token fica circulando pelo anel até que alguma estação de trabalho que deseje transmitir dados a outra estação de trabalho o capture. A partir desse momento, essa estação pode inserir seus dados  no  envelope  (token)  e  enviá-los  para  a  estação  adjacente,  que  os  envia  para  a  estação seguinte,  e  assim  por  diante  até  chegar  ao  destinatário  final.  Esse  destinatário  final  recebe  o envelope, captura os dados enviados e insere dentro do envelope um sinal de recebimento.

O envelope continua percorrendo o anel para a próxima estação, e a próxima, e a próxima, até chegar à estação que enviou os dados. Essa estação abre o envelope, verifica o sinal recebido, confirma que a estação de destino recebeu as informações enviadas e devolve o token para a rede  para  que  ele  continue  circulando  pelo  anel .  Quando  outra  estação  quiser  enviar  outra mensagem, é só capturar o token e fazer o mesmo processo. Assim, não há chances de colisões!

(TRE/GO – 2015) A topologia de uma rede refere-se ao leiaute físico e lógico e ao meio de conexão dos dispositivos na rede, ou seja, como estes estão conectados. Na topologia em anel, há um computador central chamado token, que é responsável por gerenciar a comunicação entre os nós.
_______________________ Comentários: conforme vimos em aula, em uma topologia em anel, não há um computador central. O token é um recurso do Padrão Token Ring que possui a função de permitir que uma estação de trabalho transmita dados por um canal sem o risco de colisões (Errado).






Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





53
132




8.3 – Padrão Wireless (IEEE 802.11) INCIDÊNCIA EM PROVA: ALTA 
A comunicação móvel está entre as tendências mais significativas, e os usuários esperam estar conectados à internet de forma contínua. A maioria dos hotéis oferece conexão online aos seus hóspedes, e as companhias aéreas agora disponibilizam serviços de internet em muitos de seus aviões.
A  demanda  por  comunicação  móvel  tem  despertado  interesse  pelas  tecnologias wireless, e muitos padrões wireless foram criados.

O Padrão Wireless – diferentemente dos padrões anteriores – não é cabeado. Logo, um usuário pode ficar conectado mesmo deslocando-se num perímetro geográfico mais ou menos vasto – redes sem fio fornece mobilidade aos usuários.
O Padrão Wireless se baseia em uma conexão que utiliza  ondas  de  rádio  e  define  uma  série  de  padrões  de  transmissão  e  codificação  para comunicações sem fio.


EVOLUÇÃO DO PADRÃO WIRELESS (802.11) PADRÃO  FREQUÊNCIA  TAXA DE TRANSMISSÃO IEEE 802.11b
2.4 Ghz 11 Mbps
IEEE 802.11a
5.0 Ghz 54 Mbps
IEEE 802.11g 2.4 Ghz 54 Mbps IEEE 802.11n
2.4 ou 5.0 Ghz 150, 300 até 600 Mbps IEEE 802.11ac 5.0 Ghz 500 Mbps, 1 Gbps ou + 
Assim como nas redes cabeadas, as redes  wireless (WLAN – Wireless LAN) também sofreram diversas evoluções. Observem a tabela apresentada acima: os padrões 802.11b e 802.11a surgiram simultaneamente,  porém  utilizaram  tecnologias  diferentes  – um não é evolução do outro.  O Padrão 802.11b entrou no mercado antes do Padrão 802.11a, se consolidando no mercado no início da década passada. Em seguida, veio o Padrão 802.11g...

Ele mantinha a compatibilidade com o Padrão 802.11b e sucedia ao Padrão 802.11n, permitindo
maiores  taxas  de  transmissão  e  permitindo  a  operação  em  duas  bandas  (Dual  Band)  de frequências
. Por que, professor? Porque alguns aparelhos domésticos como controle de garagem, micro-ondas e bluetooth 6
trabalham na frequência de 2.4Ghz – isso poderia causar problemas de interferência. Como alternativa, ele pode trabalhar em outra frequência de onda de rádio!

Por fim, o Padrão 802.11ac é uma novidade e pode vir a ser uma solução para tráfegos de altíssima velocidade, com taxas superiores a 1Gbps. Curiosidade: o nome Wi-Fi (WIreless-FIdelity) é uma marca comercial registrada baseada no Padrão Wireless IEEE 802.11, que permite a comunicação entre computadores em uma rede sem fio (vejam que o logo possui um TM – TradeMark). Toda tecnologia Wi-Fi é wireless, mas nem toda tecnologia wireless é Wi-Fi.

6
Se você usa teclado sem fio, provavelmente embaixo dele está informando a frequência 2.4 Ghz.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





54
132







Essa tecnologia pode utilizar transmissão Ad-hoc ou Infraestrutura:

a) Ad-Hoc: comunicação  direta  entre  equipamentos  e  válida  somente  naquele  momento, temporária, apresentando alcance reduzido (Ex: Bluetooth);
b) Infraestrutura: comunicação que faz uso de equipamento para centralizar fluxo da informação na WLAN (Ex: Access Point ou Hotspot) e permite um alcance maior (Ex: 500m).

(BB – 2007) Wi-Fi (Wireless Fidelity) refere-se a produtos que utilizam tecnologias para acesso sem fio à Internet, com velocidade que pode chegar a taxas superiores a 10 Mbps.
A  conexão  é  realizada  por  meio  de  pontos  de  acesso denominados  hot  spots.
Atualmente,  o  usuário  consegue  conectar-se  em  diferentes  lugares,  como  hotéis, aeroportos,  restaurantes,  entre  outros.  Para  que  seja  acessado  um  hot  spot,  o computador utilizado deve possuir a tecnologia Wi-Fi específica.
_______________________ Comentários: conforme vimos  em aula, está  tudo  impecável. Hotspot  é  simplesmente  o  nome  dado  ao local em  que  a tecnologia Wi-Fi está  disponível.  São  encontrados  geralmente em  locais  públicos,  tais como cafés,  restaurantes,  hotéis  e aeroportos,  onde  é  possível  se conectar à  Internet utilizando qualquer computador  portátil  que  esteja preparado  para  se comunicar com uma Rede Wi-Fi (Correto).

(SEFAZ/RJ – 2008) Cada vez mais a tecnologia wireless tem se tornado popular e sido mais utilizada em suporte à transmissão de dados. Um dos padrões tem as seguintes características:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





55
132





- funciona na freqüência de 2,4 GHz;

- oferece uma velocidade de 54 Mbps;

- baseia-se na compatibilidade com os dispositivos 802.11b;

- emprega autenticação WEP estática já aceitando outros tipos de autenticação como WPA (Wireless Protect Access) com criptografia dinâmica (método de criptografia TKIP e AES);

-  apresenta  os  mesmos  inconvenientes  do  padrão  802.11b,  que  são  as incompatibilidades com dispositivos de diferentes fabricantes e a alta interferência tanto na transmissão como na recepção de sinais, porque funcionam a 2,4 GHz equivalentes aos telefones móveis;

- apresenta como vantagens o baixo preço dos seus dispositivos, a largura de banda gratuita bem como a disponibilidade gratuita em todo o mundo;

- tem sido bastante utilizado na comunicação com notebooks em redes sem fio em curtas distâncias.

Esse padrão é conhecido como:

a) IEEE-802.11n.
b) IEEE-802.11a.
c) IEEE-802.11g.
d) IEEE-802.11j.
e) IEEE-802.11h.
_______________________ Comentários: conforme vimos em aula, trata-se do IEEE-802.11g (Letra C).











Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





56
132




8.4 – Padrão Bluetooth (IEEE 802.15) INCIDÊNCIA EM PROVA: baixa 
O Padrão Bluetooth tem o objetivo de integrar equipamentos periféricos. Utilizado em Rede WPAN (Wireless Personal Area Network) – eles padronizam uma rede de baixo custo, curto alcance, baixas taxas de transmissão e sem fio . Eles operam na faixa de 2.4 Ghz e são capazes de se conectar com até 7 dispositivos simultaneamente em uma rede piconet.

O Padrão Bluetooth possui uma Arquitetura Master/Slave. O que seria isso, professor? Você está num churrasco com os amigos e quer conectar seu celular em uma caixinha de som para colocar suas músicas para tocar. Quando você conecta o bluetooth do seu celular no bluetooth da caixinha, o seu celular está sendo exercendo o papel de Master (Mestre) e a caixinha de som está exercendo o papel de Slave (Escravo).

Um dispositivo mestre pode estar conectado a vários dispositivos escravos, mas um dispositivo escravo só pode estar conectado simultaneamente a um único dispositivo mestre. A caixinha de som não pode se conectar a dois celulares, se não ela não saberá a quem obedecer. Então, guardem essa informação:
um mesmo dispositivo pode ser mestre em determinado momento e escravo em outro, mas jamais poderá ser mestre e escravo simultaneamente .

PADRÃO BLUETOOTH – WPAN 802.15 CLASSE DISTÂNCIA
1 Até 100 Metros
2 Até 10 Metros
3 Até 1 Metro

(TRT/ES – 2013) Uma rede bluetooth possui alcance ilimitado e possibilita a conexão de componentes a um computador sem a utilização de fios.
_______________________ Comentários: conforme vimos em aula, possui alcance bastante limitado (Errado).

(CEFET/RJ – 2014) O Bluetooth é um(a):

a) padrão da instalação para redes Ethernet b) sistema de armazenamento não volátil de alta capacidade c) tecnologia de compressão de dados para redes sem fio d) tecnologia para comunicação sem fio de curta distância e) interface física para ligações entre computadores com par trançado _______________________ Comentários: conforme vimos em aula, trata-se de uma tecnologia para comunicação sem fio de curta distância (Letra D).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





57
132




8.5 – Padrão WiMAX (IEEE 802.16) INCIDÊNCIA EM PROVA: baixíssima 
O Padrão WiMAX especifica um padrão sem fio de alta velocidade para Redes Metropolitanas (WMAN),  criado  por  um  consórcio  de  empresas  para  promover  interoperabilidade  entre equipamentos. Seu raio de comunicação com o ponto de acesso pode alcançar até cerca de 40 km, sendo recomendável para prover acesso à internet banda larga a empresas e residências em que o acesso ADSL ou HFC se torna inviável por questões geográficas.

Opera em faixas licenciadas do espectro de frequência (2,5GHz, 3,5GHz, 10,5GHz), portanto é
necessário  que  empresas  adquiram  a  concessão  junto à  ANATEL  (Agência  Nacional  de Telecomunicações)  para  oferecer  esse  serviço.  A  potência  percebida  na  estação-base,  que oferecerá o serviço, pode ter uma grande variação, o que influencia a relação sinal/ruído e, por isso, a tecnologia possui três esquemas de modulação (QAM-64, QAM-16 e QPSK).

(EBSERH – 2017) Assinale a alternativa correta. O padrão IEEE 802.16 estabelece redes do tipo MAN (Metropolitan Area Network) sem fio, ou seja, WMAN (Wireless Metropolitan Area Network). Um exemplo prático desse tipo de rede é:

a) ADSL
b) GSM
c) LTE
d) WiMAX
e) HSPA
_______________________ Comentários: conforme vimos em aula, o Padrão IEEE 802.16 se trata do WiMAX (Letra D).

















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





58
132




INTERNET
1 - Conceitos Básicos INCIDÊNCIA EM PROVA: média 
A Internet é basicamente um vasto conjunto de redes de computadores diferentes que utilizam um padrão comum de comunicação e oferece um determinado conjunto de serviços.
Hoje é
muito comum o acesso à internet, mas vocês já pararam para pensar como tudo isso surgiu? Para entendê-la melhor, vamos contar um pouquinho dessa interessante história e vamos observar como e por que ela foi desenvolvida.

Tudo começa no final da década de 1950. Estávamos no auge da Guerra Fria entre EUA e URSS.
Vocês se lembram qual era o maior medo daquela época? Lembrem-se que a 2ª Guerra Mundial havia acabado  na  década  anterior  com  a  explosão  de  uma  bomba  atômica.
Dessa  forma,  o
Departamento de Defesa dos EUA decidiu que precisava de uma rede de controle e comando capaz de sobreviver inclusive a uma futura guerra nuclear com a União Soviética.


Nessa  época,  a  telefonia  pública  já  era  comum  na  vida  das  pessoas  e todas  as  comunicações militares  passavam  por  essa  rede  subterrânea  de  cabos  de  telefonia,  mas  ela  era  considerada vulnerável no caso de uma guerra. Por que? Porque essa rede funcionava de forma semelhante a uma  arquitetura  cliente/servidor  –  havia  centrais  telefônicas  espalhadas  por  todo  país.
Logo,
bastava destruir algumas dessas centrais e toda comunicação telefônica seria interrompida.

Em 1957, o mundo testemunhou um evento histórico para a humanidade: a União Soviética bateu os Estados Unidos na corrida espacial e lançou o primeiro satélite artificial do mundo – o Sputnik. O presidente  americano  Dwight  Eisenhower  ficou  com  muito  medo  de  perder  novas  batalhas tecnológicas para o país rival e criou uma organização única de pesquisas de defesa composta pelo Exército, Marinha e Aeronáutica chamada ARPA (Advanced Research Projects Agency).

Na  verdade,  essa  organização  não  possuía  cientistas  nem  laboratórios  –  era  basicamente  um escritório. No entanto, ela era capaz de oferecer concessões e contratos a universidades públicas ou  empresas  que  possuíssem  ideias  promissoras,  uma vez  que  se  tratava  de  uma  agência  de projetos de pesquisa avançada.
A ideia dessa organização era se manter sempre um passo à frente da União Soviética em tecnologia militar.

Durante os primeiros anos, a agência financiou diversos projetos diferente, mas em determinado momento seu diretor – Larry Roberts – se encantou novamente com a ideia de uma rede de controle e comando. Em 1969, algumas poucas universidades importantes concordaram em ingressar no projeto e começou a construir essa rede. Como se tratava de uma rede financiada pela ARPA, seu nome inicial foi ARPANET.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





59
132




(Prefeitura de Cajamar/SP – 2016) A Internet surgiu nos tempos da Guerra Fria com o nome de:

a) Extranet.
b) ArpaNet.
c) OnlyNet.
d) Unix.
_______________________ Comentários: conforme vimos em aula, trata-se da ArpaNet (Letra B).

Tudo  começou  bem  pequeno,  como  um  serviço  de  mensagens  entre  computadores  da Universidade  da  Califórnia,  Universidade  de  Stanford  e  a  Universidade  de  Utah.  Nas  décadas seguintes, os cientistas e engenheiros adicionaram diversos outros recursos e serviços que ainda hoje  compõem  o  que  fazemos  na  Internet.
A  primeira  grande  inovação  da  ARPANET  foi  a comutação por pacotes! Vamos falar um pouco sobre comutação antes de seguir nossa história.



Antigamente havia um emprego que hoje em dia não existe mais: telefonista! Quem aí já ouviu falar? Pois é! Naquela época, quando alguém queria ligar para um amigo, era necessário ligar primeiro para uma central telefônica. Nesse local, havia centenas de operadoras que recebiam a sua ligação, perguntavam para quem você queria ligar, e só então conectavam você ao telefone do seu amigo
7
. Essa comunicação funcionava por meio da comutação por circuito!

7
Curiosidade: em 1935 foi realizada a primeira ligação telefônica que circundava o planeta – ela demorou 3h25min apenas para tocar no destinatário.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





60
132





Professor, não entendi! Vamos observar com mais atenção a imagem! Temos cinco operadoras com fones de ouvido e microfones. Na frente delas, é possível ver um painel com pequenos buracos e cabos plugados em alguns desses buracos. Em todo telefone, saía um cabo e passava por debaixo da terra por quilômetros e quilômetros até chegar a uma central telefônica.
Esses cabos que vocês estão vendo são os mesmos cabos conectados aos telefones residenciais.

Pois bem... quando você queria telefonar para o seu amigo, você falava primeiro com a operadora por meio do cabo que saía da sua casa até a central telefônica. Ela perguntava com quem você queria falar e simplesmente plugava o cabo telefônico da sua casa ao cabo telefônico da casa do seu amigo. Pronto!
A partir desse momento vocês possuíam a reserva de um canal de comunicação dedicado e poderiam conversar sem interferências.

É claro que se outra pessoa estivesse tentando te ligar, você não conseguiria atendê-la porque você está com o seu canal de comunicação ocupado/reservado. Pois bem... isso que nós acabamos de descrever se chama comutação por circuito. Professor, o que significa esse termo comutação?
No
contexto de telecomunicações, é o processo de interligar dois ou mais pontos. No caso da telefonia, as centrais telefônicas comutam ou interligam terminais.

Observem que a comutação por circuito estabelece um caminho fim a fim dedicado, reservando um canal de comunicação temporariamente, para que dados de voz sejam transmitidos. Nesse caso, a informação de voz sempre percorre a mesma rota e sempre chega na mesma ordem.
O processo
de  comutação  por  circuito  possui  uma  fase  de  estabelecimento  da  conexão,  uma  fase  de transferência de dados e uma fase de encerramento da conexão.

Galera, eu vou contar uma coisa surpreendente para vocês agora! Vocês acreditam que ainda hoje a telefonia funciona por meio da comutação de circuitos?
Pois... é claro que não precisamos mais de operadores  porque  os  circuitos  são  capazes  de  se  mover  automaticamente  em  vez  de manualmente.
Legal, mas a comutação por circuito é completamente inviável na internet. Por que, Diegão? Cara, vamos lá...

O  principal problema  é  o  desperdício  de  recursos!
Poxa... quando um dispositivo de  origem estabelece uma conexão com um dispositivo de destino, fecha-se uma conexão e ambas as linhas permanecem dedicadas mesmo que não esteja havendo comunicação. Imaginem que eu estou falando com um amigo no telefone, mas estou apertado para ir ao banheiro! Se eu passar meia hora no banheiro, a linha continuará reservada mesmo sem eu estar utilizando.

Além  disso,  a  comutação  por  circuito  só  permite  que  eu  telefone  para  uma  única  pessoa simultaneamente – eu não consigo conversar com dois amigos simultaneamente. Já imaginaram se a internet funcionasse assim?  Nesse  caso,  seu  computador  só  poderia  se  conectar a  um  único dispositivo ao mesmo tempo.
Seria impossível acessar dois sites simultaneamente – você teria que fechar um site para poder acessar outro.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





61
132




Além disso, o tráfego na internet é muito inconstante. Por exemplo: você começa a estudar uma aula de informática em nosso site, depois você sai para comer, depois você volta e entra em um site para ouvir uma música relaxante. Vocês percebem que o perfil de utilização é totalmente diferente?
Se utilizássemos a comutação por circuito na internet, você sairia para comer e deixaria a linha reservada mesmo sem a estar utilizando, desperdiçando recursos.



Algumas vezes, por questão de segurança ou por questão de relevância, é necessário manter uma linha  exclusiva  e  dedicada.  Por  essa  razão,  forças armadas,  bancos  e  outras  organizações  que possuem processos de alta criticidade mantêm linhas ou circuitos dedicados para conectar seus centros de dados como mostra a imagem anterior.
Voltando à história: a ARPANET trouxe um novo paradigma chamado Comutação por Pacotes. Como funcionava?

Vamos falar uma analogia com uma empresa de entrega. Vamos supor que se John deseja enviar uma carta para David.
Em vez de ter uma estrada dedicada entre a cidade de John e a cidade de David, eles poderiam utilizar as diferentes rotas possíveis entre as duas cidades.
Exemplo: um
caminhão poderia pegar a carta e transportá-la apenas de Indianapolis para Chicago. Ao chegar nessa cidade, ela poderia ir consultar a melhor rota e levaria de Chicago para Minneapolis.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





62
132





Em seguida, a rota seria de Minneapolis para Billings; e finalmente de Billings até Missoula – como mostra a imagem abaixo à esquerda. Ao parar em cada cidade, o motorista do caminhão poderia perguntar na estação de correio da cidade qual era a melhor rota até chegar ao destino final.
A parte
mais  interessante  dessa  abordagem  é  que  ela  pode  utilizar  rotas  diferentes,  tornando  a comunicação mais confiável e tolerante a falhas.

Como assim, professor? Imaginem que haja uma tempestade de neve na cidade de Minneapolis que congestionou absolutamente todas as vias. Não tem problema – o motorista do caminhão poderia utilizar outra rota passando por Omaha – como mostra a imagem acima à direita.
Voltando para o
mundo  das  redes  de  computadores,  não  há  necessidade  de  uma  conexão  estabelecer previamente uma rota dedicada para a transmissão de dados.

Na comutação por pacotes, há uma malha de nós conectados ponto-a-ponto em que cada nó verifica a rota de menor custo para entrega da informação. Como assim, Diego? O caminho de menor custo é o caminho mais rápido entre dois pontos. Nas imagens anteriores, nós temos dois caminhos entre dois pontos. O primeiro é até mais curto, mas está congestionado – logo, o segundo caminho tem menor custo porque é o caminho mais rápido entre dois pontos.

Quem aí já usou o Waze? Por vezes, você já sabe o caminho entre seu trabalho e sua casa e você sabe que ele é o caminho mais curto. No entanto, ainda assim é interessante utilizar o Waze. Por que?
Porque se houver um acidente no percurso, o caminho mais curto em distância pode ser mais lento em tempo do que eventualmente um caminho mais longo em distância.
O software sugerirá um caminho mais distante, mas que você chegará mais rápido.


Agora  tem  outro  ponto  interessante  sobre  esse  tipo de  comutação!  Por  vezes,  os  dados transmitidos são grandes demais ao ponto de eventualmente obstruir uma rede completamente (Ex: envio de um arquivo de 100Mb).
A comutação por pacotes trouxe uma ideia genial: dividir as informações em pequenos pedaços chamados de pacotes.
Logo, em vez de enviar o arquivo integral, você o divide em milhares de pacotinhos. O que tem de genial nisso, professor?

Galera... se eu fragmento ou segmento uma informação em milhares de pacotes, eu posso enviá-los  separadamente  de  modo  que  cada  um  possa  percorrer  uma  rota  totalmente diferente. Professor, está muito complexo! Vamos voltar ao exemplo dos correios: imagine que eu preciso enviar um relatório de 100 páginas para outro estado, mas que os correios só permitam o envio de 10 páginas por envelope.

Não tem problema! Eu posso dividir meu relatório em dez pacotes de dez páginas e fazer dez envios diferentes. Como os correios vão entregar os pacotes separadamente, cada pacote pode percorrer uma rota até o destino final. E digo mais: pode ser que as dez primeiras páginas cheguem por  último  e  as  últimas  dez  páginas  cheguem  primeiro.  Cara...  acontece  quase  igualzinho  no contexto de internet.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





63
132




Quando se envia dados pela internet, não é possível prever o caminho percorrido pelo pacote até chegar ao seu destino final.
Cada pacote enviado pode seguir por uma rota diferente chegando  em ordem  diferente  da  ordem  enviada  (claro  que, após  todos  os  pacotes chegarem,  o  arquivo  é  remontado na forma original). Pessoal, deixa eu contar uma coisa para vocês:
nós só temos internet hoje em dia por conta dessa ideia genial...

A comutação por pacotes permite aproveitar melhor os canais de transmissão de dados de modo que sua utilização seja compartilhada pelos usuários da forma mais eficiente e tolerante a falhas possível.  Ela  utiliza  um  tipo  de  transmissão store-and-forward,  em  que  o  pacote  recebido  é armazenado por um equipamento e encaminhado ao próximo destino. Em cada equipamento, o pacote recebido tem um endereço de destino, que possibilita indicar o caminho final.

Pessoal... os engenheiros testaram a comutação por pacotes e foi um sucesso, mas – com o passar dos anos – a quantidade de novos computadores e dispositivos conectados à rede começou a aumentar e surgiu um problema. Nós vimos que o equipamento que recebe e armazena o pacote era  responsável  por  encaminhá-lo  ao  próximo  destino.  No  entanto,  isso  implicava  que  todo computador deveria manter uma lista atualizada do endereço de outros computadores da rede.

E se a lista não estivesse atualizada? Esse equipamento não saberia para onde enviar ou enviaria o pacote para um local que não existia mais, entre outras possibilidades.
Com o aumento da
quantidade de computadores na rede, era cada vez mais comum que computadores mudassem seu endereço e a atualização para os outros computadores da rede não era tão rápida. Como eles resolveram esse problema, Diego? Os caras eram sinistros...


Mapa da Arpanet em 1974 Em 1973, eles decidiram abolir esse sistema em que cada dispositivo possuía uma lista de endereços dos outros e escolheram a Universidade de Stanford como uma espécie de registro central oficial de endereços. Em 1978, já havia mais de cem computadores conectados à Arpanet por todo Estados Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





64
132




Unidos e até Inglaterra. Nos anos seguintes, começaram a surgir redes semelhantes à Arpanet em diferentes lugares do mundo com mais computadores.

Legal, professor! É legal, mas originou alguns problemas. Cada rede criada formatava seus pacotes de maneira diferente, então – apesar de ser possível conectar redes diferentes – isso causava uma dor de cabeça. Para resolver esse problema, a solução foi utilizar um conjunto de protocolos comuns de comunicação chamado TCP/IP.
O que é um protocolo, professor? Basicamente é uma convenção que controla e possibilita conexões, comunicações e transferências de dados.

Professor, você pode explicar de outra forma?
Claro, vamos fazer uma analogia! Se eu comprar um notebook e ele vier com uma tomada de cinco pinos, eu não conseguirei utilizá-lo. Se ele funcionar em 110v, eu não conseguirei utilizá-lo em Brasília. Se eu comprar um mouse sem fio para utilizar com  o  notebook,  mas  eles  operarem  em  faixas  de  frequência  diferentes,  eu  também  não conseguirei utilizá-los.

No primeiro caso, eu ainda posso comprar um adaptador; no segundo caso, eu ainda posso comprar um transformador; mas no terceiro caso, não há nada a se fazer. O que vocês podem concluir de tudo isso? É possível concluir que se os fabricantes de equipamentos não conversarem entre si, haverá sérios problemas de comunicação de dados.
Por essa razão, foram criados protocolos comuns de comunicação, sendo o conjunto mais utilizado chamado de TCP/IP.

Quando duas ou mais redes se conectam utilizando a pilha de protocolos TCP/IP, fica bem mais fácil conectá-las.  O  conjunto  de  redes  de  computadores  que  utilizam  esses  protocolos  e  que consiste em milhões de empresas privadas, públicas, acadêmicas e de governo, com alcance local ou global e que está ligada a uma grande variedade de tecnologias de rede é também conhecida popularmente como...
INTERNET
Atualmente, a internet oferece uma infinidade de serviços disponibilizados! Dentro os principais serviços, os mais conhecidos são:

SERVIÇOS DESCRIÇÃO
World Wide Web (WWW) Trata-se do serviço de visualização de páginas web organizadas em sites em que milhares de pessoas possuem acesso instantâneo a uma vasta gama de informação online em hipermídia que podem ser acessadas via navegador – é o serviço mais utilizado na Internet. Em geral, esse serviço utiliza protocolos como HTTP e HTTPS.
CORREIO ELETRÔNICO
Trata-se do serviço de composição, envio e recebimento de mensagens eletrônicas entre partes de uma maneira análoga ao envio de cartas – é anterior à criação da Internet. Utiliza tipicamente um modo assíncrono de comunicação que permite a Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





65
132




troca  de  mensagens  dentro  de  uma  organização.  Em  geral,  esse  serviço  utiliza protocolos como POP3, IMAP e SMTP.
ACESSO REMOTO
Trata-se do serviço que permite aos usuários facilmente se conectarem com outros computadores, mesmo que eles estejam em localidades distantes no mundo. Esse acesso remoto pode ser feito de forma segura, com autenticação e criptografia de dados, se necessário.  Em geral, esse serviço utiliza protocolos como SSH e TELNET.
TRANSFERÊNCIA DE ARQUIVOS Trata-se do serviço de tornar arquivos disponíveis para outros usuários por meio de downloads  e  uploads.  Um  arquivo  de  computador  pode ser  compartilhado  ou transferido com diversas pessoas através da Internet, permitindo o acesso remoto aos usuários. Em geral, esse serviço utiliza protocolos como FTP e P2P.

Esses são os serviços principais, mas existem muitos outros oferecidos via Internet (Ex: grupos de discussão, mensagens instantâneas, bate-papo, redes sociais, computação em nuvem, etc).

(Câmara  de  Juiz  de  Fora/MG  –  2018) A  possibilidade  de  redigir,  enviar  e  receber mensagens de correio eletrônico é uma realidade criada já na fase inicial da ARPANET (precursora da Internet) e é imensamente popular.
_______________________ Comentários: conforme vimos em aula, é um serviço anterior à Internet e que já surgiu na fase inicial da ArpaNet (Correto).

(Ministério da Integração – 2012) Os serviços de Internet mais populares e difundidos são:

a) Wide Worring Web, correio eletrônico, sequenciamento de arquivos, login remoto e desktop remoto.

b)  World  Wide  Web,  correio  eletrônico,  transferência  de  arquivos,  login  remoto  e desktop remoto.

c) World Wide Web, comutação de servidores, transferência de arquivos, login remoto e debugging remoto.

d) World Wide Wedge, correio eletrônico, transferência de endereços, controle remoto e desktop local.

e) Wood Wide Weed, controle eletrônico, transferência de arquivos, login remoto e backup remoto.
_______________________ Comentários: conforme vimos em aula, os serviços mais comuns são World Wide Web, Correio Eletrônico, Transferência de Arquivos, Login Remoto e Desktop Remoto (Letra B).


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





66
132




2 – Web (WWW)
INCIDÊNCIA EM PROVA: baixa 


Web  é  uma  contração  do  termo  World  Wide  Web  (WWW). Ah, professor... você tá falando de internet, não é? Não! Muito cuidado porque são coisas diferentes! A internet é uma rede mundial de  computadores  que  funciona  como  uma  estrutura  que  transmite  dados  para  diferentes aplicações
(Instagram, Skype, Spotify, etc). A Web é maior dessas aplicações – uma gigantesca aplicação distribuída rodando em milhões de servidores no mundo inteiro usando navegadores.

Professor, ainda não entendi a diferença entre Internet e Web!
Galera, a internet é a plataforma que permite a execução de diversas aplicações e a web é simplesmente uma delas. Podemos dizer que se você está acessando por meio de um navegador, trata-se de uma aplicação web. Caso contrário,  é  somente  outra  aplicação  que  roda  na  internet  (Ex:  Jogos,  BitTorrent,  Photoshop, Microsoft Outlook, entre outros).


World Wide Web
(WWW)
Microsoft
Outlook
BitTorrent
SPOTIFY
World of
Warcraft
...
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





67
132





Vamos  falar  um  pouco  agora  sobre  as  gerações  da  web.  Pessoal,  as  gerações  da  web  não  se excluem, elas se sobrepõem. Vamos vê-las em detalhes:

2.1 – Web 0.0

Em março de 1989, a World Wide Web teve a primeira especificação composta pelo Protocolo HTTP e a Linguagem HTML lançada por Tim Berners-Lee
. Sim, se utilizamos a web atualmente, devemos agradecer a esse  senhor  aqui  do lado!  Até  então,  a  web  era  uma fonte  de  acesso  a informações, onde páginas de hipertexto (textos com links), de conteúdo estático, escritas por jornalistas e outros profissionais eram publicadas em Servidores Web e podiam apenas ser lidas pelos demais usuários. Galera, vocês querem conhecer a primeira página web da história? Segue o link abaixo:


http://info.cern.ch/hypertext/WWW/TheProject.html 



Em 1991, a página web acima era a única do mundo; em 1994, já havia 2.738 páginas web – inclusive o
Yahoo!;  em  1998,  já  havia  2.410.067  páginas  web  –  inclusive  o Google;  em  2001,  já  havia 29.254.370  páginas  web  –  inclusive  a Wikipedia;  em  2005,  já  havia  64.780.617  páginas  web  – inclusive o
Youtube; em 2008, já havia 172.338.776 páginas web – inclusive o Dropbox; e em 2018, temos 1.805.260.010 páginas web – inclusive o Estratégia Concursos!

2.2 – Web 1.0

A Web 1.0 foi marcada por sites com conteúdos estáticos, produzidos maioritariamente por empresas e instituições, com pouca interatividade entre os internautas.
Altavista, Geocities, Yahoo, Cadê, Hotmail eram as grandes estrelas da internet. Era caracterizada pela baixa interação do usuário, permitindo pouca ou nenhuma interação – como por exemplo – deixar comentários ou manipular e criar conteúdos.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





68
132





As tecnologias e métodos da Web 1.0 ainda são utilizadas para a exibição de conteúdos como leis e manuais. Essa geração foi marcada pela produção centralizada de conteúdos – como os diretórios e portais (Ex: UOL, ZAZ, Terra, AOL).
Nesse contexto, o usuário era responsável pela navegação e localização de conteúdos relevantes por sua própria conta tendo predominantemente uma atuação passiva em um processo onde poucos produzem e muitos consomem.

Era algo muito parecido com o modelo de broadcasting da indústria midiática como TV, rádio, jornais e revistas – sua grande virtude foi a democratização do acesso à informação.

2.3 – Web 2.0

Esse termo foi criado em 2003 para designar uma segunda geração de comunidades e serviços baseados na plataforma web. Não há grandes mudanças tecnológicas, mas – sim – um foco maior na forma como a web é encarada pelos usuários e desenvolvedores . Os programas e
protocolos são os mesmos, porém o foco passa para a integração dos usuários junto às informações dos sites, sendo marcada por páginas que permitem ao próprio usuário inserir conteúdo.

A Web 2.0 também foi a revolução dos blogs e chats, das mídias sociais colaborativas, das redes sociais e do conteúdo produzido pelos próprios internautas .  Nesse  momento,  a  internet  se popularizou em todo o mundo, e começou a abranger muito mais do que algumas empresas para se  tornar  obrigatória  para  qualquer  um  que  queira  ter  sucesso  no  mercado.  São  exemplos:
Facebook; Google+; Linkedin; Instagram; Tumblr; Youtube; Blogs; Wikis; entre outros.

Os sites criados para esse momento da internet já não são estáticos e possuem um layout claramente focado no consumidor e também na usabilidade dos buscadores. Nesse momento, a navegação mobile e uso de aplicativos já tem forte presença no dia-a-dia das pessoas. Outra recomendação é a utilização de uma combinação de tecnologias já existentes (Web Services, AJAX, etc) e de uso simplificado que aumentem a velocidade e a facilidade de uso de aplicações web.

Busca-se ampliar o conteúdo existente na Internet para permitir que usuários comuns publiquem e consumam informação de forma rápida e constante.
A Web 2.0 em contraste à Web 1.0, tem seu conteúdo  gerado  predominantemente  por  seus  usuários  em  um  processo  onde  muitos produzem e todos consomem.
Nesse contexto, houve uma demanda por avanços tecnológicos em mecanismos de busca devido do imenso volume de conteúdo produzido.

2.4 – Web 3.0

Permite que palavras e figuras sejam organizadas de várias fontes diferentes para tornar a vida de seus usuários mais simples. Seu propósito é permitir que o usuário acesse informações com menos cliques ou reúna interesses de maneira intuitiva. A Web 3.0 é composta de dados onipresentes, conectados e capazes de serem reagrupados sob demanda. Capaz de oferecer uma inteligência simulada, busca entender o que o usuário deseja através de algoritmos semânticos.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





69
132




3 – Internet das Coisas (IoT) INCIDÊNCIA EM PROVA: baixa 
Agora vamos falar rapidamente sobre o assunto do futuro que tem começado a cair em concurso público: Internet of Things (IoT) – também conhecida como Internet das Coisas. Como é que é, professor?
Galera, pensem rapidinho em todos os seus objetos que possuem acesso à internet: computador, notebook, tablet, smartphone, relógio, entre outros. Beleza, esses são os mais comuns em nosso dia-a-dia mesmo.
Porém, vocês conseguem pensar em outros?



A câmera de segurança da portaria do seu prédio?
Ela tem acesso à internet! A Smart TV que você assiste aquele filminho bacana na Netflix? Ela tem acesso à internet! Quem curte jogar um videogame de vez em quando?
Ele  tem  acesso  à  internet! Galera,  isso  porque  estamos  no  Brasil.  Em  outros  países  mais desenvolvidos,  já  existem  outras  coisas:  geladeiras,  máquina  de  lavar  roupa,  forno  de  micro-ondas, termostato, alarme de incêndio, sistema de som e iluminação, etc.

Galera,  isso  não  significa  que  seja  possível  baixar  uma  aula  de  informática  no  site  do  Estratégia Concursos usando sua geladeira! A proposta, na verdade, é que a conectividade auxiliará esses objetos a ficarem mais eficientes em seus contextos específicos. Agora vamos parar de pensar na nossa casa e vamos pensar no mundo: isso tem aplicabilidades em agropecuária, hospitais, escolas, fábricas, transporte público, lojas, serviços públicos, logística, etc.

Professor, quais tecnologias são utilizadas?
Existem basicamente três componentes: dispositivos, redes de comunicação e sistemas de controle . Nós acabamos de ver acima os dispositivos. Em geral, eles são Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





70
132




equipados com microchips, sensores ou outros recursos de comunicação e monitoramento. As redes de comunicação também são conhecidas: em geral, trata-se do Wi-Fi, Bluetooth, NFC, 4G, etc. Não basta que o dispositivo se conecte à internet ou troque informações com outros objetos.


Esses dados precisam ser processados, ou seja, devem ser enviados a um sistema que os trate. Qual?
Aí  depende  da  aplicação!  Imagine  uma  casa  que  tem  monitoramento  de  segurança,  controle  de temperatura ambiente e gerenciamento de iluminação integrados. Os dados de câmeras, alarmes contra incêndio, aparelhos de ar condicionado, lâmpadas e outros itens são enviados para um sistema que controla cada aspecto.

Esse sistema pode ser um serviço nas nuvens, o que garante o acesso a ele a partir de qualquer lugar.
Entendido? Então vamos fazer alguns exercícios e vamos partir para cima da Intranet...

(ABIN – 2018) Redes wi-fi e Bluetooth podem ser utilizadas para IoT, já NFC (Near Field Communication) não atende a demandas de IoT.
_______________________ Comentários: conforme vimos em aula, podem ser utilizados Wi-fi, Bluetooth e também NFC (Errado).

(ABIN – 2018) Em uma residência, caracteriza uma solução de IoT a instalação de um detector de fumaças capaz de gerar alertas em caso de fumaça e ser acionado, a partir de um smartphone, para iniciar um mecanismo de reação.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).




















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





71
132




4 – Tecnologias de Acesso 
Galera, até o início da década de noventa, só quem sabia o que era internet eram pesquisadores ligados a universidades, ao governo ou à indústria. No entanto, quando um físico chamado Tim Berners-Lee criou a Web (WWW), houve uma mudança nessa realidade e a internet ganhou milhões de novos usuários sem a menor pretensão acadêmica.
O serviço de disponibilização de páginas web facilitou e popularizou bastante o uso da internet.

Junto  com  o  primeiro  navegador  da  história  (chamado  Mosaic),  a  web  tornou  possível  a configuração  de  diversas  páginas  web  contendo  informações,  textos,  imagens,  sons  e  vídeos disponíveis através de links para outras páginas. Clicando em um link, o usuário é repentinamente transportado para a página indicada por esse link.
Com o passar dos anos, foram criadas muitas páginas em um período de tempo muito curto.

Grande parte desse crescimento foi impulsionado por empresas denominadas Provedores de Serviços  da  Internet  (ISP  –  Internet  Service  Provider).
Essas  empresas  oferecem  a  usuários individuais a possibilidade de se conectar à Internet, obtendo assim acesso aos diversos serviços fornecidos. Essas empresas reuniram milhões de novos usuários, alterando completamente o perfil de usuário sendo utilizada como um serviço de utilidade pública (como a telefonia).

Vamos detalhar isso melhor! A internet pode ser fornecida por meio de satélites, ondas de rádio ou uma rede de milhares de cabos de fibra óptica terrestres ou submarinos, que conectam diversos países, respondendo por 80% de toda a comunicação.
Essa infraestrutura de redes – que forma a espinha dorsal da internet – é chamada de Backbone. Ela possui alto velocidade, desempenho e interliga várias redes, garantindo o fluxo da informação por dimensões continentais .

Diego, quem constrói esses backbones? Eles são construídos por provedores de serviço de internet, que  administram troncos  de  longo  alcance com  o  objetivo  de  fornecer  acesso  à internet  para diversas outras redes. Em geral, eles pertencem a companhias telefônicas de longa distância (Ex:
Embratel) ou a governos nacionais (Ex: Rede Nacional de Ensino e Pesquisa – RNP), que vendem o
acesso para Provedores de Serviço de Internet (ISP – Internet Service Provider) .



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





72
132




Os provedores de internet nacionais mais conhecidos atualmente são: NET/CLARO, GVT/VIVO e SKY. Por sua vez, esses provedores de internet vendem o acesso a provedores menores ou a usuários  comuns.  Na  imagem  anterior,  é  possível  visualizar  os  maiores  troncos  de  backbones espalhados pelo mundo entre os continentes e também os troncos de backbones brasileiros. Notem que eles podem ser terrestres ou submarinos.

Existem  três  níveis  de  hierarquia  entre  provedores de  acesso: ISP  Nível  1  tem  cobertura internacional, conectando países ou continentes; ISP Nível 2 tem cobertura nacional, conectando um ou mais ISP Nível 1 e oferecendo serviços a vários ISP Nível 3; e ISP Nível 3 tem cobertura regional – conectando um ou pessoas, casas, escritórios ou conectando provedores locais (aquele que só existe na sua cidade especificamente).



(Correios – 2011) Redes de acesso situadas na borda da Internet são conectadas ao restante da rede segundo uma hierarquia de níveis de ISPs (Internet service providers).
Os ISPs de nível 1 estão no nível mais alto dessa hierarquia:
_______________________ Comentários: conforme vimos em aula, as redes de acesso situadas na borda da internet realmente são conectadas ao restante da rede segundo uma hierarquia de níveis de ISP (Internet Service Provider). Além disso, conforme vimos na figura acima, os ISP Nível 1 estão realmente no topo dessa hierarquia (Correto).

Dito isso, os enlaces que conectam as redes de acesso residenciais aos ISP Nível 3 ou Locais podem ser de diferentes tipos, em função da tecnologia e meios físicos. Os mais conhecidos são:

4.1 – Dial-Up
INCIDÊNCIA EM PROVA: média 
Trata-se de uma conexão discada através de um modem e uma linha de telefonia analógica fixa .
Era a maneira mais popular de acesso da década de 90, hoje encontra-se em desuso. Apresenta um alto custo de implementação e baixas taxas de transmissão. Galera, era muito lento! No máximo, Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





73
132




você conseguia taxas de até 56Kbps. E hoje em dia você reclama da taxa de 20Mbps (ou 20000Kbps) do seu 4G. Quem aí tem mais de 30 anos sabe do que eu estou falando! :) 
4.2 – ISDN (Integrated Services Digital Network) INCIDÊNCIA EM PROVA: baixíssima 
Trata-se de uma linha telefônica transformada em dois canais de mesma velocidade, em que era possível usar voz e dados simultaneamente – cada um ocupando um canal de transmissão .
Era  possível  também  utilizar  os  dois  canais  para  voz  ou  para  dados.  Na  prática,  permitia videoconferências (um canal para voz e outro para vídeo) desde que os dois assinantes possuíssem o serviço ISDN.

4.3 – ADSL (Asymmetric Digital Subscriber Line) INCIDÊNCIA EM PROVA: média 
Trata-se da conexão de banda larga oferecida por empresas de telefonia fixa. Embora utilize a mesma infraestrutura da telefonia, a transmissão de dados ocorria em frequências das de voz, permitindo – portanto – o uso da internet sem ocupar o telefone. Por se tratar de uma Linha de Assinante  Digital
Assimétrica,  as  taxas  de  download  e  de  upload  são  diferentes  –  sendo  a velocidade de download maior que a de upload.

4.4 – Acesso Via Cabo (HFC e Cable Modem) INCIDÊNCIA EM PROVA: baixíssima 
Trata-se da conexão híbrida de banda larga via cabos de concessionárias de TV a Cabo (NET, GVT, OI, etc). Essa tecnologia emprega uma técnica conhecida como HFC (Hybrid Fiber-Coaxial) que cria redes metropolitanas (MANs) com backbones de fibra ótica e interconecta as residências a partir  de  cabos  coaxiais  e  modens  a  cabo  (Cable-Modem).  Possui  taxa  de  transmissão  de  até 38Mbps por canal utilizado.

4.5 – PLC (Power Line Communication) INCIDÊNCIA EM PROVA: baixíssima 
Trata-se da tecnologia em que a mesma tomada que fornece energia elétrica também oferece banda larga através de um modem específico . Ela busca competir com o ADSL e o acesso via cabo, apresentando  como  vantagem  a  portabilidade,  pois  basta  plugar  o  modem  em  uma  tomada compatível com o serviço para se obter o acesso. No Brasil, embora o serviço seja autorizado pelas agências responsáveis, os investimentos foram baixos por questões estratégicas.

4.6 – Telefonia Celular INCIDÊNCIA EM PROVA: baixa 
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





74
132




Trata-se da tecnologia de acesso à internet via rede de telefonia celular. Foi construída baseada em diferentes gerações da tecnologia, quais sejam:

GERAÇÃO DESCRIÇÃO
1ª Geração (1G)
Esses telefones foram os primeiros celulares a serem utilizados, que foram introduzidos em 1982 e concluídos no início de 1990. Era usado para serviços de voz e era baseado em tecnologia chamada Advanced Mobile Phone System (AMPS).

2ª GERAÇÃO (2G)
Utilizando tecnologia digital TDMA, CDMA ou GSM, passou a ser adotado no Brasil em 2002,  oferecendo  –  além  de  telefonia  –  a  possibilidade  de  mensagens  de  texto  SMS, chamada  em  espera,  identificação  de  chamadas,  teleconferência,  etc.  O  Padrão  GSM (Global System for Mobile Communications) foi padronizado na Europa.
2ª GERAÇÃO (2,5G)
Utilizando tecnologia digital GPRS, foi o primeiro sistema de acesso à Internet através de rede celular realmente útil. Apresentava taxas de transmissão similares às de um acesso discado, mas devido à enorme latência na transmissão e ao grande volume de pacotes perdidos e retransmitidos acaba tendo um resultado bastante inferior.
3ª geração (3g)
Utilizando  tecnologia  digital  UMTS,  oferece  banda  larga  através  da  telefonia  celular.
Sucessor natural do GSM, o UMTS foi o resultado da padronização de várias tecnologias 3G,  permitindo  a  transmissão  de  dados  e  totalmente compatível  com  GSM  para transmissão de voz. Atualmente oferece taxas de até 14,4 Mbps.
4ª geração (4g)
utilizando tecnologia digital LTE (Long Term Evolution), foi disponibilizada no Brasil a partir de 2013, tendo sido implementada com o objetivo de melhorar o padrão UMTS, oferecendo taxas de  100  Mbps  a 1 Gbps – sendo  também  compatível  com o  padrão  GSM.  Nessa tecnologia, são esperados picos de até 120Mbps.

(AGU – 2014) ADSL é um tipo de conexão:

a) sem fio.
b) para acesso a HDs externos.
c) para TVs.
d) de banda larga.
_______________________ Comentários: conforme vimos em aula, trata-se de um tipo de conexão de banda larga (Letra D).

(BRB – 2011) O acesso à Internet em alta velocidade por meio de conexão dial-up, via linha telefônica, também conhecido como serviço ADSL, dispensa o uso de modem, visto que, nesse caso, a conexão ocorre diretamente a partir de infraestrutura das empresas de telefonia fixa ou móvel (celular).
_______________________ Comentários: conforme vimos em aula, o serviço ADSL não se dá por meio de conexão dial-up, via linha telefônica. Ademais, ele necessita do uso de um Modem ADSL (diferente do modem convencional para acesso discado), porém que não precisa converter o sinal de digital para analógico porque o sinal é sempre digital (Asymetric Digital Subscriber Line). Por fim, ele ocorre a partir da infraestrutura das empresas de telefonia fixa e, não, móvel (Errado).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





75
132




RESUMO

DEFINIÇÃO
Uma  rede  é  um  conjunto  de  terminais,  equipamentos, meios  de  transmissão  e  comutação  que  interligados possibilitam a prestação de serviços.

TIPO SIGLA DESCRIÇÃO DISTÂNCIA PERSONAL

AREA NETWORK
PAN
Rede  de  computadores  pessoal  (celular,  tablet, notebook, entre outros).
De alguns centímetros a alguns poucos metros.
LOCAL

AREA NETWORK
LAN
Rede  de  computadores  de  lares,  escritórios, prédios ou campus.
De algumas centenas de metros a alguns quilômetros.
METROPOLITAN

AREA NETWORK
MAN
Rede de computadores entre uma matriz e filiais em uma cidade.
Cerca de algumas dezenas de quilômetros.
WIDE

AREA NETWORK
WAN
Rede de computadores entre cidades, países ou até continentes.
De algumas dezenas a milhares de quilômetros.

TIPO de rede DESCRIÇÃO PONTO A PONTO
Também chamada de Rede Par-a-Par, é o modelo de rede mais simples de ser montado. Nesse modelo, todas as máquinas podem compartilhar dados e periféricos umas com as outras. Essas redes são comuns em residências e entre filiais de empresas, porque demandam um baixo custo, são facilmente configuráveis e possibilitam altas taxas de velocidade de conexão.

CLIENTE/

SERVIDOR
É um modelo de redes mais complexo, porém mais robusto e confiável. Nesse modelo, existe uma máquina especializada, dedicada e geralmente remota, respondendo rapidamente aos pedidos vindos dos demais computadores da rede – o que aumenta bastante o desempenho de algumas tarefas. É a escolha natural para redes grandes, como a Internet – que funciona tipicamente a partir do Modelo Cliente/Servidor.




TOPOLOGIA
BARRAMENTOESTRELA
ANELMALHA
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





76
132




TIPO DE TOPOLOGIA DESCRIÇÃO FÍSICA Exibe o layout (disposição) dos links e nós de rede.
LÓGICA
Exibe o fluxo ou percurso dos dados na rede.

TIPO REPRESENTAÇÃO DESCRIÇÃO BARRAMENTO
(BUS)

Todas as estações ficam ligadas ao mesmo meio de transmissão, isto é, um único cabo (chamado backbone) em que os nós se ligam através de conectores. Há maior facilidade na instalação e economia de cabeamento, mas não há isolamento de falhas – uma ruptura no cabo implica a interrupção da comunicação.


ANEL (RING)

Cada dispositivo possui uma conexão ponto-a-ponto com outros dois dispositivos conectados lado a lado, e fazendo uso de uma comunicação com transmissão unidirecional (simplex). Nesse caso, a mensagem circula o anel, sendo regenerada e  retransmitida  a  cada  nó,  passando  pelo  dispositivo  de  destino  que  copia  a informação enviada, até retornar ao emissor original. Nesse momento, o link é liberado para que possa ser utilizado pelo nó seguinte.
ESTRELA
(STAR)

As estações estão ligadas a um nó central controlador, pelo qual passam todas as mensagens,  não  havendo  tráfego  direto  entre  os  dispositivos.  O  enlace  entre estações e o nó central é Ponto-a-Ponto. É a topologia mais usada atualmente por facilitar a adição de novas estações e a identificação ou isolamento de falhas, em que – se uma conexão se romper – não afetará a comunicação de outras estações.

MALHA
(MESH)

Cada estação possui um link ponto a ponto dedicado com transmissão bidirecional (duplex)  entre  cada  uma  das  demais  estações.  Em  outras  palavras,  todos  os computadores estão interligados entre si, de modo que caso haja uma ruptura em algum cabo, não cai a rede inteira, somente o nó conectado a esse cabo.



TIPO REPRESENTAÇÃO DESCRIÇÃO SIMPLEX

Uma comunicação é dita simplex quando há um transmissor de mensagem, um receptor de mensagem e esses papéis nunca se invertem no período de transmissão.
HALF-DUPLEX

Uma  comunicação  é  dita  half-duplex  quando  temos  um transmissor e um receptor, sendo que ambos podem transmitir e receber dados, porém nunca simultaneamente.
FULL-DUPLEX

Uma  comunicação  é  dita  full-duplex  quando  temos  um transmissor e um receptor, sendo que ambos podem transmitir e receber dados simultaneamente.

TIPO REPRESENTAÇÃO DESCRIÇÃO UNICAST

Uma mensagem só pode ser enviada para um destino. Grosso modo, quando você envia uma mensagem no Whatsapp   para Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





77
132




uma  pessoa  específica,  você  está  enviando  uma  mensagem unicast.
MULTICAST

Uma  mensagem  é enviada  para  um  grupo de destino.  Grosso modo, quando você cria uma lista de transmissão no Whatsapp com um grupo de pessoas e os envia uma mensagem, você está enviando uma mensagem multicast.
BROADCAST

Uma mensagem é enviada para todos os destinos. Grosso modo, quando  você  cria  uma  lista de  transmissão  no  Whatsapp  com todos os  seus  contatos  e  os  envia  uma  mensagem,  você  está enviando uma mensagem broadcast.

TIPO DE MEIO DESCRIÇÃO GUIADO
Trata-se da transmissão por cabos ou fios de cobre, onde os dados transmitidos são convertidos em sinais elétricos que propagam pelo material condutor. Exemplo: cabos coaxiais, cabos de par traçado, fibra óptica, entre outros.
NÃO-GUIADO
Trata-se  da  transmissão  por  irradiação  eletromagnética,  onde  os  dados  transmitidos  são irradiados  através  de  antenas  para  o  ambiente.  Exemplo:  ondas  de  rádio,  infravermelho, bluetooth e wireless.



TIPO REPRESENTAÇÃO DESCRIÇÃO CABO COAXIAL

Consiste  em  um  fio  central  de  cobre,  envolvido  por uma  blindagem metálica. Isolantes de plástico flexível separam os condutores internos e externos e outras camadas do revestimento que cobrem a malha externa.
Esse meio de transmissão é mais barato, relativamente flexível e muito resistente à interferência eletromagnéticas graças à malha de proteção que  possui.  Esse  cabo  cobre  distâncias  maiores  que o  cabo  de  par trançado e utiliza um conector chamado BNC.
CABO DE PAR
TRANÇADO

Consiste de quatro pares de fios trançados blindados ou não, e envolto de um revestimento externo flexível. Eles são trançados para diminuir a interferência  eletromagnética  externa  e  interna  –  quanto  mais  giros, maior a atenuação. Este é o cabo mais utilizado atualmente por ser o mais barato de todos e ser bastante flexível. Esse cabo cobre distâncias menores  que  o  cabo  coaxial  e  utiliza  um  conector  chamado  RJ-45 (Memorizem!).
CABO DE FIBRA
ÓPTICA

Consiste em uma Casca e um Núcleo (de vidro) para transmissão de luz.
Possui  capacidade  de  transmissão  virtualmente  infinita,  é  imune  a interferências eletromagnéticas e consegue ligar distâncias maiores sem a necessidade de repetidores. Como desvantagens, podemos dizer que é incapaz de fazer curvas acentuadas, além de ter um custo de instalação e Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





78
132




manutenção muito alto em relação ao par trançado. Há dois tipos de fibra: Monomodo e Multimodo.

CATEGORIA VELOCIDADE ou taxa de dados FREQUÊNCIA DISTÂNCIA MÁXIMA CAT3
Até 10 MBPS 16 MHz 100 Metros CAT4 Até 16 MBPS 20 MHz 100 Metros CAT5
Até 100 MBPS 100 MHz 100 Metros CAT5e
Até 1000 MBPS (1G) 100 MHz 100 Metros CAT6 Até 10000 MBPS (10G) 250 MHz 100 Metros CAT6A
Até 10000 MBPS (10G) 500 MHz 100 Metros CAT7 Até 10000 MBPS (10G) 600 MHz 100 Metros CAT7A Até 10000 MPBS (10G) 1000 MHz 100 Metros CAT8
Até 40000 MBPS (40G) 2000 MHz 100 Metros 
PLACA DE REDE HUB (CONCENTRADOR) BRIDGE (PONTE) 

Equipamento    de    rede    de comunicação bidirecional (entrada e saída de dados) conectado à placa- mãe do computador. Toda placa de rede possui um número identificador chamado Endereço MAC (48 Bits).
Dispositivo  de  rede  capaz  de aumentar  o  alcance  de  uma  rede local por meio da regeneração de sinais. É capaz de trabalhar apenas com broadcast, isto é, ao receber um pacote de dados, distribui para todas as máquinas da rede.

Equipamento capaz de separar uma rede   em   segmentos   menores, reduzindo  as  chances  de  colisões quando  várias  máquinas  desejam transmitir dados ao mesmo tempo.
São  dispositivos  capazes  de  enviar dados para máquinas específicas.

SWITCH (COMUTADOR) ROUTER (ROTEADOR) ACCESS POINT 



Equipamento    semelhante    às Bridges,  no  entanto  possuem  mais portas. Em contraste com hubs, são capazes  de  enviar  transmitir dados para  máquinas  específicas  (unicast ou  multicast).  Por  segmentarem  a Equipamento    que    permite interligar  redes  distintas  e  são capazes  de  escolher  as  melhores rotas para transmissão de pacotes de   dados.   É   o   dispositivo responsável    por    interligar dispositivos de uma rede local (Ex:
Equipamento que permite estender a cobertura  de  uma  rede  sem  fio  de algum   local   (Ex:   aeroporto, universidade, estádios, etc). Ainda é necessário utilizar um roteador para se  conectar  à  internet,  apesar  de Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





79
132




rede,   reduzem   as   colisões   e diminuem o fluxo de informações.

Computador, Notebook, Smartphone,  Impressora,  etc)  à internet.
existirem  roteadores  que  fazem  o papel de Access Point.
MODEM (MODULADOR/DEMODULADOR) 
Trata-se de um dispositivo capaz de converter sinais digitais em sinais analógicos e vice-versa, em geral por meio de uma linha telefônica. Os três modelos principais são: Acesso Discado; Modem ADSL; e Cable Modem.

PADRÕES DE REDES OU ARQUITETURA DE INTERCONEXÃO Trata-se de um conjunto de padrões de arquitetura de interconexão de redes de computadores (LAN, MAN ou WAN).

PADRÃO NOME
IEEE 802.3
Ethernet (LAN)
IEEE 802.5
Token Ring (LAN)
IEEE 802.11 Wi-Fi (WLAN) IEEE 802.15
Bluetooth (WPAN)
IEEE 802.16 WiMAX (WMAN) IEEE 802.20 Mobile-Fi (WWAM) 
PADRÃO ETHERNET (IEEE 802.3) Arquitetura  de  interconexão  de  redes  locais  baseada  no  envio  de  pacotes  de  dados.  Possui  comunicação bidirecional (duplex), mecanismos de detecção de colisões e topologia em estrela.

EVOLUÇÃO DOS PADRÕES ETHERNET PADRÃO (CABO COAXIAL) PADRÃO – TAXA DE TRANSMISSÃO - DISTÂNCIA ETHERNET 10BASE-2 / 10 Mbps / 185 Metros ETHERNET 10BASE-5 / 10 Mbps / 500 Metros EVOLUÇÃO DOS PADRÕES ETHERNET PADRÃO (CABO DE PAR TRANÇADO) PADRÃO – TAXA DE TRANSMISSÃO ETHERNET 10BASE-T / 10 Mbps FAST ETHERNET 100BASE-T / 100 Mbps GIGABIT ETHERNET 1000BASE-T / 1000 Mbps 10G ETHERNET 10GBASE-T / 10000 Mbps 
PADRÃO TOKEN RING (IEEE 802.5) Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





80
132




Arquitetura de conexão redes locais cabeada atualmente em desuso. Possui comunicação unidirecional (simplex), arquitetura ponto-a-ponto e topologia lógica em anel.

PADRÃO WIRELESS (IEEE 802.11) Arquitetura de conexão de redes locais sem fio que define um conjunto de padrões de transmissão e codificação para comunicações não cabeadas.

EVOLUÇÃO DO PADRÃO WIRELESS (802.11) PADRÃO  FREQUÊNCIA  TAXA DE TRANSMISSÃO IEEE 802.11b 2.4 Ghz 11 Mbps IEEE 802.11a
5.0 Ghz 54 Mbps
IEEE 802.11g 2.4 Ghz 54 Mbps IEEE 802.11n
2.4 ou 5.0 Ghz 150, 300 até 600 Mbps IEEE 802.11ac
5.0 Ghz 500 Mbps, 1 Gbps ou + 
PADRÃO BLUETOOTH (IEEE 802.15) O Padrão Bluetooth tem o objetivo de integrar equipamentos periféricos. Utilizado em Rede WPAN (Wireless Personal Area Network) – eles padronizam uma rede de baixo custo, curto alcance, baixas taxas de transmissão e sem fio.

PADRÃO WIMAX (IEEE 802.16) O Padrão WiMAX especifica um padrão sem fio de alta velocidade para Redes Metropolitanas (WMAN), criado por um consórcio de empresas para promover interoperabilidade entre equipamentos. Seu raio de comunicação com o ponto de acesso pode alcançar até cerca de 40 km, sendo recomendável para prover acesso à internet banda larga a empresas e residências em que o acesso ADSL ou HFC se torna inviável por questões geográficas.

internet
A Internet é basicamente um vasto conjunto de redes de computadores diferentes que utilizam um padrão comum de comunicação e oferece um determinado conjunto de serviços.

Principais SERVIÇOS  DESCRIÇÃO World Wide Web
(WWW)
Trata-se do serviço de visualização de páginas web organizadas em sites em que milhares de  pessoas  possuem  acesso  instantâneo a  uma  vasta  gama de  informação online  em hipermídia que podem ser acessadas via navegador – é o serviço mais utilizado na Internet.
Em geral, esse serviço utiliza protocolos como HTTP e HTTPS.
CORREIO ELETRÔNICO
Trata-se do serviço de composição, envio e recebimento de e-mails entre partes de uma maneira análoga ao envio de cartas – é anterior à criação da Internet. Utiliza tipicamente um modo assíncrono de comunicação que permite a troca de mensagens dentro de uma organização. Em geral, esse serviço utiliza protocolos como POP3, IMAP e SMTP.
ACESSO REMOTO
Trata-se  do  serviço  que  permite  aos  usuários  facilmente  se  conectarem  com  outros computadores, mesmo que eles estejam em localidades distantes no mundo. Esse acesso remoto pode ser feito de forma segura, com autenticação e criptografia de dados, se necessário.  Em geral, esse serviço utiliza protocolos como SSH e TELNET.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





81
132




TRANSFERÊNCIA DE
ARQUIVOS
Trata-se  do  serviço  de  tornar  arquivos  disponíveis para  outros  usuários  por  meio  de downloads e uploads. Um arquivo de computador pode ser compartilhado ou transferido com diversas pessoas através da Internet, permitindo o acesso remoto aos usuários. Em geral, esse serviço utiliza protocolos como FTP e P2P.

WORLD WIDE WEB (WWW) A Web é uma aplicação que é executada na Internet – trata-se de uma série de páginas web que podem ser acessadas por meio de um navegador web.

INTERNET DAS COISAS
Trata-se do conceito que se refere à interconexão digital de objetos físicos cotidianos entre si e com usuários por meio de sensors ou softwares capazes de transmitir dados pela internet 
TECNOLOGIA de acesso DESCRIÇÃO Dial-Up
Conexão discada através de um modem e uma linha de telefonia fixa. Era a maneira mais popular  de  acesso  da  década  de  90,  hoje  encontra-se  em  desuso.  Apresenta  como características um alto custo (telefonia, provedor) e baixas taxas de transmissão, taxas de até 56 Kbps (banda estreita).
ISDN
Linha telefônica transformada em dois canais de mesma velocidade, em que era possível usar voz e dados simultaneamente – cada um ocupando um canal. Era possível também utilizar os dois canais para voz ou para dados. Na prática, permitia videoconferências desde que os dois assinantes possuíssem o serviço ISDN.
ADSL
Conexão de Banda Larga oferecida por empresas de telefonia fixa. Embora utilize a mesma infraestrutura da telefonia discada (cabos), a transmissão de dados ocorria em frequências mais altas que as de voz, permitindo, portanto, o uso simultâneo da Internet e do telefone convencional.
HDF e CABLE MODEM
Conexão de Banda Larga via cabos de concessionárias de TV a Cabo (NET, GVT, OI, etc).
Emprega uma técnica conhecida como HFC (Hybrid Fiber-Coaxial), em que cria Redes Metropolitanas (MANs) com Backbones de fibra ótica e interconecta as residências a partir de cabos coaxiais e modens a cabo (Cable-Modem).
PLC
Tecnologia em que a mesma tomada que fornece energia elétrica também passa a oferecer banda larga através de um modem específico. Essa tecnologia tem como objetivo competir com o ADSL e o acesso via Cabo, apresentando como vantagem a portabilidade, pois basta plugar o modem em uma tomada compatível com o serviço para se obter o acesso.
TELEFONIA CELULAR
Tecnologia que permite o acesso à internet via redes 2G, 3G, 4G, entre outros.





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





82
132




MAPA MENTAL

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





83
132





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





84
132





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





85
132




QUESTÕES COMENTADAS - FCC 
1. (FCC / SEGEP-MA / Auxiliar de Fiscalização Agropecuária) Há uma correta associação entre o problema e a sua solução usando o tipo correto de rede de computadores em:

a)  Uma empresa possui dois escritórios em uma mesma cidade e deseja que os computadores permaneçam interligados. Para isso deve-se utilizar uma LAN − Local Area Network que conecta diversas máquinas dentro de dezenas de quilômetros.

b)  Uma empresa possui um enorme volume de dados e precisa interligar o servidor principal aos outros computadores. Para permitir esta conexão deve-se utilizar uma SAN − Servidor Area Network que conecta diversas máquinas a um servidor central.

c)  Há  diversos  dispositivos  em  uma  residência  que  precisam  se  comunicar  dentro  de  uma distância  bastante  limitada.  Para  isso  deve  ser  utilizada  uma  rede  PAN  −  Private  Area Network, que utiliza tecnologias como Wi-Fi e bluetooth.

d)  Deseja-se conectar redes de escritórios de uma mesma empresa ou de vários campi de universidades. A melhor solução é utilizar uma WLAN − Wireless Local Area Network, a versão wireless (sem fio) de uma LAN que alcança centenas de quilômetros.

e)  Uma  empresa  presta  serviços  online  24  horas  para  países  localizados  em  diferentes continentes. Deve-se utilizar uma WAN − Wide Area Network, que vai além da MAN − Metropolitan  Area  Network,  conseguindo  alcançar  uma  área  maior,  como  um  país  ou mesmo um continente.

Comentários:

(a) Errado, deve-se utilizar uma MAN; (b) Errado, SAN (Storage Area Network) é uma rede para armazenamento de dados; (c) Errado, PAN é Personal Area Network e, não, Private Area Network.
Ademais, PAN usa apenas bluetooth; (d) Errado, a WLAN alcança centenas de metros – o ideal para o caso seria uma MAN; (e) Correto. A WAN (Wide Area Network) resolveria o problema.

Gabarito: Letra E

2. (FCC / DPE-RS / Técnico em Segurança - 2017) Considere uma rede de computadores instalada e em funcionamento que é caracterizada pelo seu alcance local, por se tratar de uma rede interna de curto alcance. De acordo com sua extensão geográfica, essa rede é classificada como:

a) Metropolitan Area Network − MAN.
b) Local Area Network − LAN.
c) Wide Area Network − WAN.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





86
132




d) Storage Area Network − SAN.
e) Popular Area Network − PAN.

Comentários:


Alcance local, rede interna e curto alcance... só pode ser uma Rede de Área Local (LAN).

Gabarito: Letra B

3. (FCC / ARTESP / Especialista em Regulação de Transporte - 2017)  Considere  a  seguinte situação hipotética: um usuário recebe o sinal de Internet no seu computador desktop através de  um  modem  de  banda  larga  que  também  é  roteador  wireless,  ligado  diretamente  ao computador por um cabo ethernet. Apesar de todos os equipamentos serem atuais e terem sido instalados recentemente, em determinado momento a Internet para de funcionar e aparece um símbolo de falha no ícone da rede da barra de tarefas.

Um conjunto de possíveis problemas relacionados a esta situação e ações para resolvê-los é elencado abaixo.

I. O cabo ethernet de par trançado pode ter se desconectado ou ficado frouxo, em decorrência do usuário movimentar o gabinete ou o modem. É recomendável que o usuário verifique a conexão do cabo, tanto no modem quanto no gabinete do computador.

II. O modem pode não estar funcionando bem em decorrência, por exemplo, de sobrecarga no tráfego de informações. É recomendável que o usuário desligue o modem e ligue-o novamente após  alguns  segundos,  para  que  ele  seja  reiniciado e  o  seu  funcionamento  normal  seja restaurado.

III. O adaptador de rede pode estar desativado, o driver pode estar desatualizado ou a placa de rede pode estar danificada. É recomendável que o usuário atualize o driver do adaptador de rede,  ative-o,  caso  esteja  desativado,  ou  providencie  a  troca  da  placa  de  rede, caso  esteja danificada.

IV. O cabo ethernet coaxial pode ter se rompido devido ao seu núcleo de alumínio ser bastante sensível, principalmente nas proximidades dos conectores RJ-35 usados para fazer a ligação ao modem e ao gabinete do computador. É recomendável que o usuário faça uma verificação visual para saber se o cabo está rompido.

São problemas e ações corretas que podem ser tomadas para tentar resolvê-los o que consta APENAS em:

a) I, II e III.
b) I, III e IV.
c) III e IV.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





87
132




d) I e II.
e) II e IV.

Comentários:


(I)  Correto.  O  Cabo  de  Par-Trançado  pode  ter  sofrido  algum  problema  em  decorrência  de movimentações. Caso você fique sem internet algum dia, recomendo que verifique esse cabo.

(II)  Correto.  Se  o  modem  estiver  sofrendo  com  sobrecarga  de  recomendações,  é  realmente recomendável desligá-lo, esperar alguns segundos e religá-lo.

(III) Correto. Adaptador de Rede é qualquer dispositivo que permita a conexão a uma rede. A Placa de Rede é um tipo de Adaptador de Rede. Dito isso, ambos podem estar danificados ou desativados, e o driver pode estar desatualizado. É recomendável verificar todas essas opções.

(IV) Errado. O Cabo Ethernet Coaxial pode ter realmente se rompido, mas ele não possui um núcleo de alumínio, é de cobre. Ademais, ele utiliza conectores BNC (Cabos de Par Trançado utilizam conectores RJ-45 ou RJ-11).

Gabarito: Letra A

4. (FCC / DPE-RR / Técnico em Informática - 2015) A velocidade de transmissão 100 Mbit/s do Fast-Ethernet é alcançada com uma largura de banda de 31,25 MHz. Dessa forma, só é possível atender esta banda requerida com os cabos de par trançado de categoria:

a)  5 ou superior
b)  5a ou superior
c)  6a
d)  5e ou 6e
e)  6 ou superior

Comentários:

CATEGORIA VELOCIDADE ou taxa de dados FREQUÊNCIA DISTÂNCIA MÁXIMA CAT3 Até 10 MBPS 16 MHz 100 Metros CAT4
Até 16 MBPS 20 MHz 100 Metros CAT5 Até 100 MBPS 100 MHz 100 Metros CAT5e
Até 1000 MBPS (1G) 100 MHz 100 Metros CAT6
Até 10000 MBPS (10G) 250 MHz 100 Metros CAT6A Até 10000 MBPS (10G) 500 MHz 100 Metros CAT7
Até 10000 MBPS (10G) 600 MHz 100 Metros CAT7A Até 10000 MPBS (10G) 1000 MHz 100 Metros Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





88
132




CAT8
Até 40000 MBPS (40G) 2000 MHz 100 Metros 
Conforme  vimos  em  aula,  só  é  possível  atender  a  banda  requerida  por  meio  de  cabos de  par trançado  de  Categoria  5  ou  superior.  Notem  que  ele atinge  velocidades  de  até  1000  Mbps  e Frequência de até 100 Mhz.

Gabarito: Letra A

5. (FCC / DPE-RR / Técnico em Informática - 2015) Com relação ao meio de propagação do sinal, as fibras óticas podem ser classificadas em monomodo e multimodo. As fibras multimodo:

a)  são usadas principalmente em LANs, pois têm um baixo custo e apresentam alto índice de refração quando comparadas com outras fibras.
b)  apresentam  desvantagem  no  alinhamento  dos  núcleos  nas  emendas  e  conectores  em relação às fibras monomodo.
c)  possuem  o  diâmetro  do  seu  núcleo  menor  se  comparado  com  o  núcleo  de  uma  fibra monomodo.
d)  têm taxas de transmissão mais altas, quando comparadas às fibras ópticas monomodo.
e)  são mais utilizadas em enlaces intercontinentais, nacionais e metropolitanos, devido à sua baixa atenuação para longas distâncias.

Comentários:

(a) Correto, são utilizadas principalmente em LANs, porque são mais baratas e apresentam alto índice de refração – o que causa um pouco mais de perdas e atenuação; (b) Errado, como o núcleo tem um diâmetro maior (como mostrado na figura da teoria), as emendas e os conectores que podem ser utilizados são mais fáceis de alinhar; (c) Errado, possuem diâmetro do seu núcleo maior (como mostrado na figura da teoria); (d) Errado, têm taxas de transmissão menores; (e) Errado, são utilizados em  redes locais.  Para  enlaces  intercontinentais,  recomenda-se  a  utilização  de  fibras monomodo – que possuem baixo índice de refração e atenuação.

Gabarito: Letra A

6. (FCC / TRE-RS / Auditor Público Externo - Engenharia Civil - Conhecimentos Básicos - 2014) Atualmente,  grande  parte  das  instalações  físicas  de  redes  de  computadores  é  realizada utilizando a tecnologia Ethernet com cabos de pares trançados. Neste tipo de instalação, 
a)  um defeito em um dos computadores conectados não afeta o funcionamento da rede.
b)  utilizam-se menos cabos do que em uma instalação semelhante utilizando cabos coaxiais.
c)  são disponibilizadas maior largura de banda e velocidade do que permitem os cabos de Fibra Óptica podem disponibilizar.
d)  o conector utilizado nas terminações dos cabos é denominado UTP.
e)  a topologia de rede estabelecida é do tipo Barramento.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





89
132





Comentários:

Essa questão dá margem para interpretações! Para resolvê-la, temos que inferir que se trata de uma Topologia  em  Estrela,  que  –  apesar  de  ser  a  mais  comum  –  não  é  obrigatória  na  Tecnologia Ethernet.

(a) Correto, cada nó possui uma conexão ponto-a-ponto com o nó central. Logo, um defeito em um dos computadores não afetará o funcionamento da rede como um todo; (b) Errado, não existe nenhuma relação entre tipo e quantidade de cabos; (c) Errado, cabos de fibra óptica podem oferecer larguras de banda infinitamente maiores; (d) Errado. UTP é um tipo de cabo de par trançado – o conector se chama RJ-45; (e) Errado, a topologia de rede estabelecida é do tipo Estrela.

Gabarito: Letra A

7. (FCC / TRT - 1ª REGIÃO (RJ) / Analista Judiciário – Área Administrativa / 2013) Sabendo que uma intranet utiliza a infraestrutura de rede da empresa e fazendo uso das informações contidas no texto, considere que o computador de Paulo pode se comunicar com o computador servidor do Tribunal porque os recursos necessários estão fisicamente localizados em um raio de até 500 metros dentro do prédio do Tribunal, incluindo o computador de Paulo e o servidor. Isso significa que a rede utilizada é do tipo.

a)  WAN
b)  CAN
c)  LAN
d)  MAN
e)  ADSL

Comentários:

O texto introdutório é muito grande e irrelevante para responder à questão. Se recursos estão fisicamente localizados em um raio de até 500 metros, trata-se de uma Rede Local (LAN).

Gabarito: Letra C

8. (FCC / SPPREV / Analista em Gestão Previdenciária - 2012) A topologia de uma rede de comunicação  refere-se  à  forma  com  que  os  enlaces  físicos  e  os  nós  de  comutação  estão organizados, determinando os caminhos físicos existentes e utilizáveis entre quaisquer pares de estações conectadas a essa rede.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





90
132






A denominação correta da Figura 1 é:

a)  Anel.
b)  Hierárquica
c)  Malha
d)  Barramento
e)  Estrela

Comentários:

Pessoal, a figura acima trata da Topologia em Barramento.

Gabarito: Letra D

9. (FCC / INSS / Técnico do Seguro Social - 2012) Pedro trabalha em uma pequena imobiliária cujo escritório  possui  cinco  computadores  ligados  em  uma  rede  com  topologia  estrela.  Os computadores nessa rede são ligados por cabos de par trançado a um switch (concentrador) que filtra e encaminha pacotes entre os computadores da rede, como mostra a figura abaixo.

Certo dia, Pedro percebeu que não conseguia mais se comunicar com nenhum outro computador da rede. Vários são os motivos que podem ter causado esse problema, EXCETO:

a)  O cabo de rede de um dos demais computadores da rede pode ter se rompido.
b)  A placa de rede do computador de Pedro pode estar danificada.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





91
132




c)  A porta do switch onde o cabo de rede do computador de Pedro está conectado pode estar danificada.
d)  O cabo de rede que liga o computador de Pedro ao switch pode ter se rompido.
e)  Modificações  nas  configurações  do  computador  de Pedro  podem  ter  tornado  as configurações de rede incorretas.

Comentários:

(a) Errado, caso um cabo de rede de um dos demais computadores da rede se rompa, não afetará o restante da rede; (b) Correto, a placa de rede pode estar danificada; (c) Correto, a porta do Switch pode realmente estar danificada; (d) Correto, o cabo que liga especificamente o computador do Pedro ao Switch pode ter se rompido; (e) Correto, pode ter havido modificações nas configurações do computador de Pedro.

Gabarito: Letra A

10. (FCC / MPE-RS / Agente Administrativo - 2008) Os dispositivos de rede de computadores que são interconectados física e logicamente para possibilitar o tráfego de informações pelas redes compõem layouts denominados.

a)  Protocolos.
b)  Topologias.
c)  Roteamentos.
d)  Arquiteturas.
e)  Cabeamento.

Comentários:

Conforme vimos em aula, a questão trata das topologias.

Gabarito: Letra B

11. (FCC / TRT-PE / Analista Administrativo - 2018) Um Analista comprou um roteador wireless e o conectou por cabo em um switch para acessar a estrutura de rede cabeada. Isso permitiu que todos os dispositivos sem fio conectados nesse roteador tivessem acesso a todos os serviços disponíveis na rede cabeada, como por exemplo, acesso à internet. Nesse caso, o roteador foi configurado pelo Analista para operar no modo:

a)  ponto-a-ponto.
b)  access point.
c)  bridge.
d)  modem.
e)  backbone.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





92
132





Comentários:

Se você tem um roteador na sua casa, mas tem partes dela em que o sinal wireless está fraco, você tem duas opções: comprar um Access Point, que estenderá o sinal da sua rede; ou, se você tiver um roteador velhinho que não esteja sendo usado, você pode utilizá-lo no Modo Access Point e ele funcionará exatamente igual a um.

Gabarito: Letra B

12. (FCC / SEGEP-MA / Técnico de Fiscalização Agropecuária - 2018) A tecnologia de rede de computadores:

a)  WiMax foi desenvolvida para funcionar em redes locais, tendo curto alcance, justamente o oposto do Wi-Fi, que foi desenvolvido para funcionar em redes metropolitanas. As duas tecnologias atuam de forma complementar.

b)  Wi-Fi permite o acesso à internet da casa ou da empresa de um usuário através de ondas do tipo bluetooth. O usuário poderá acessar a internet a até 1 km do aparelho receptor.

c)  3G é uma das possibilidades de conexão de computadores usando banda larga sem fio. O sistema  permite  que  voz,  dados  e  imagens  sejam  transmitidos  e  acessados  em  alta velocidade, via satélite.

d)  Wi-Fi não precisa de cabeamento, pois o sinal de internet chega, por infravermelho, até o roteador através da infraestrutura sem fio da rede telefônica ou da TV a cabo.

e)  WiMax  é  uma  evolução  da  Wi-Fi,  sendo  uma  tecnologia  que  permite  acesso  sem  fio  à internet.

Comentários:


(a) Errado, a questão inverteu os conceitos.

(b) Errado, são ondas eletromagnéticas de rádio e de curto alcance.

(c) Errado, ela realmente oferece conexão banda larga, mas não via satélite, é via antena.

(d) Errado, o sinal chega no roteador por meio de cabos e um Access Point ou um Roteador Wireless o difundem via wi-fi.

(e) Correto. Questão perfeita!

Gabarito: Letra E
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





93
132





13. (FCC / METRÔ-SP / Oficial Logística de Almoxarifado - 2018) Em uma empresa há um modem, que também é roteador, que recebe o sinal de Internet e o distribui por cabo e via wireless para computadores e dispositivos móveis dos funcionários. Como esse roteador não possui portas suficientes  para  ligar  por  cabos  outros  5  computadores,  um  técnico  sugeriu  utilizar  um equipamento  que,  ligado  ao  roteador,  poderá  oferecer  portas  suficientes  para  ligar  outros computadores do escritório, permitindo, inclusive, acesso à Internet. O equipamento sugerido foi um:

a)  switch.
b)  hub usb.
c)  dmz.
d)  proxy.
e)  vnc bridge.

Comentários:

Um roteador geralmente possui apenas quatro portas. Se você tiver cinco computadores, já não é possível conectá-los todos via cabo no roteador. Para resolver esse problema, é comum a utilização de um Switch, que é capaz de segmentar a rede e conectar dezenas de computadores via cabo.

Gabarito: Letra A

14. (FCC / SEGEP-MA / Fiscal Estadual Agropecuário - 2018)  Uma  agência  recebe  o  sinal  da internet via cabo de fibra ótica em um modem, que está ligado a um dispositivo que funciona como um ponto de encontro, distribuindo o sinal da internet para todos os computadores e permitindo que eles se comuniquem por cabos de rede. Nesta situação, esse dispositivo é:

a)  switch.
b)  web server.
c)  firewall.
d)  hub USB.
e)  dmz server.

Comentários:

Galera,  o  Switch  é  o  dispositivo  capaz  de  distribuir  o  sinal  de  Internet  e  permitir  que  eles  se comuniquem por meio de cabos.

Gabarito: Letra A

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





94
132




15. (FCC / TRE-SP / Técnico Judiciário - Área Administrativa - 2012) Para que o computador de uma residência possa se conectar à Internet, utilizando a rede telefônica fixa, é indispensável o uso de um hardware chamado:

a)  hub.
b)  Modem.
c)  Acess point.
d)  Adaptador 3G.
e)  Switch.

Comentários:

O modem é o dispositivo que se conecta à Internet por meio de uma rede de telefonia fixa.

Gabarito: Letra B

16. (FCC / SEE-MG / Especialista em Educação - Supervisão Pedagógica- 2012) É usado para centralizar um ponto de acesso para Internet em uma rede e/ou criar uma rede de computadores com ou sem cabos para conectá-los. Pode ser utilizado em lugares como aeroportos e escolas com redes sem fio.

O texto refere-se ao dispositivo de redes chamado:

a)  Switch.
b)  Roteador wireless.
c)  WI-FI hub.
d)  Cable modem wireless.

Comentários:

Se o dispositivo é utilizado para centralizar um ponto de acesso para Internet em uma rede, ele pode ser um Roteador Wireless ou um Access Point. No entanto, a questão diz que ele pode criar uma rede de computadores com ou sem cabos para conectá-los, logo não pode ser um Access Point, porque ele só tem a função de centralizar um ponto de acesso ou estender a cobertura de uma rede sem fio.

Gabarito: Letra B

17. (FCC / TRT - 4ª REGIÃO (RS) / Técnico Judiciário - Área Administrativa- 2011) Numa rede LAN (Local Area Network), o recurso de hardware mínimo que deverá estar instalado no computador para permitir a comunicação com os demais elementos da rede é:

a)  o teclado.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





95
132




b)  o hub.
c)  o cartão de memória.
d)  o switch.
e)  a placa de rede.

Comentários:

Conforme  vimos  em  aula,  trata-se  da  Placa  de  Rede, que  é  o  recurso  a  ser  instalado  no  seu computador para permitir a comunicação com os demais elementos.

Gabarito: Letra E

18. (FCC / INFRAERO / Técnico de Segurança do Trabalho - 2011) Sobre a infraestrutura para uma Intranet, considere:

I. Wireless é um padrão específico de uma tecnologia de redes sem fio.
II. Wi-Fi refere-se genericamente à transmissão de dados sem a utilização de meios físicos.
III. WLAN é uma rede local sem fio para fazer conexão com a Internet ou entre os dispositivos da rede.

Está correto o que se afirma em:

a)  I, apenas.
b)  III, apenas.
c)  I e II, apenas.
d)  II e III, apenas.
e)  I, II e III.

Comentários:

(I) Errado. Wi-Fi é um padrão específico, uma marca comercial registrada; (II) Errado. Wireless refere-se genericamente à transmissão de dados sem a utilização de meios físicos; (III) Correto. A WLAN (Wireless Local Area Network) é uma rede local sem fio para fazer conexão com a Internet ou entre os dispositivos da rede.

Gabarito: Letra B

19. (FCC / TRE-TO / Analista Judiciário - Área Administrativa - 2011) Os dispositivos que têm como principal função controlar o tráfego na Internet são denominados:

a) Switches.
b) Comutadores.
c) Roteadores.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





96
132




d) Firewalls.
e) Web servers.

Comentários:

A questão trata dos roteadores – eles são os responsáveis por controlar o tráfego na Internet. São aquelas anteninhas que permite que você compartilhe a conexão de internet com dois ou mais aparelhos.  Firewalls  têm  a  função  de  filtrar  o  tráfego  de  pacotes,  mas  não  o  controlar!  Não confundam filtrar com controlar o tráfego: fitrar é o ato de decidir que pacotes podem ou não entrar e sair da rede; controlar é o ato de definir que caminho (rota) deve ser tomada pelos pacotes para chegarem ao seu destino. Quem controla o tráfego são os roteadores que são dispositivos utilizados para interligar redes.

Gabarito: Letra C

20. (FCC  /  TRE-AL  /  Analista  Judiciário  -  Área  Judiciária  -  2010)  Ao  compartilhar  pastas  e impressoras entre computadores, evitando que pessoas não autorizadas possam acessar os arquivos pela Internet, pode-se montar a rede usando um firewall, baseado em hardware, por meio do dispositivo denominado:

a) Hub
b) Switch
c) Roteador
d) Repetidor
e) Cross-over

Comentários:

Os roteadores permitem compartilhar dados entre computadores em uma rede. Ressaltando que um firewall é um dispositivo de uma rede que aplica políticas de segurança a um determinado ponto de uma rede.

Gabarito: Letra C

21. (FCC / SEFAZ-SC / Auditor Fiscal da Receita Estadual - 2018) O Auditor Fiscal foi designado para  especificar  a  aquisição  de  um  dispositivo  de  rede  de  computadores  para  realizar  a interconexão e a comunicação entre uma rede Ethernet e uma rede Token-Ring. O dispositivo especificado pelo Auditor deve ser:

a) Hub.
b) Firewall.
c) Switch.
d) Roteador.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





97
132




e) Bridge.

Comentários:

Nós sabemos que o equipamento que permite conectar segmentos de redes diferentes que podem ou não utilizar tecnologias/protocolos de enlace distintos (Ex: Ethernet, Token Ring, etc) é a Bridge (Ponte). O Switch – apesar de ser considerado uma bridge multiportas – não permite interconectar tecnologias/protocolos de enlace distintos.

Gabarito: Letra E
























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





98
132




LISTA DE QUESTÕES – FCC 
1. (FCC / SEGEP-MA / Auxiliar de Fiscalização Agropecuária) Há uma correta associação entre o problema e a sua solução usando o tipo correto de rede de computadores em:

a)  Uma empresa possui dois escritórios em uma mesma cidade e deseja que os computadores permaneçam interligados. Para isso deve-se utilizar uma LAN − Local Area Network que conecta diversas máquinas dentro de dezenas de quilômetros.

b)  Uma empresa possui um enorme volume de dados e precisa interligar o servidor principal aos outros computadores. Para permitir esta conexão deve-se utilizar uma SAN − Servidor Area Network que conecta diversas máquinas a um servidor central.

c)  Há  diversos  dispositivos  em  uma  residência  que  precisam  se  comunicar  dentro  de  uma distância  bastante  limitada.  Para  isso  deve  ser  utilizada  uma  rede  PAN  −  Private  Area Network, que utiliza tecnologias como Wi-Fi e bluetooth.

d)  Deseja-se conectar redes de escritórios de uma mesma empresa ou de vários campi de universidades. A melhor solução é utilizar uma WLAN − Wireless Local Area Network, a versão wireless (sem fio) de uma LAN que alcança centenas de quilômetros.

e)  Uma  empresa  presta  serviços  online  24  horas  para  países  localizados  em  diferentes continentes. Deve-se utilizar uma WAN − Wide Area Network, que vai além da MAN − Metropolitan  Area  Network,  conseguindo  alcançar  uma  área  maior,  como  um  país  ou mesmo um continente.

2. (FCC / DPE-RS / Técnico em Segurança - 2017) Considere uma rede de computadores instalada e em funcionamento que é caracterizada pelo seu alcance local, por se tratar de uma rede interna de curto alcance. De acordo com sua extensão geográfica, essa rede é classificada como:

a) Metropolitan Area Network − MAN.
b) Local Area Network − LAN.
c) Wide Area Network − WAN.
d) Storage Area Network − SAN.
e) Popular Area Network − PAN.


3. (FCC / ARTESP / Especialista em Regulação de Transporte - 2017)  Considere  a  seguinte situação hipotética: um usuário recebe o sinal de Internet no seu computador desktop através de  um  modem  de  banda  larga  que  também  é  roteador  wireless,  ligado  diretamente  ao computador por um cabo ethernet. Apesar de todos os equipamentos serem atuais e terem sido instalados recentemente, em determinado momento a Internet para de funcionar e aparece um símbolo de falha no ícone da rede da barra de tarefas.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





99
132





Um conjunto de possíveis problemas relacionados a esta situação e ações para resolvê-los é elencado abaixo.

I. O cabo ethernet de par trançado pode ter se desconectado ou ficado frouxo, em decorrência do usuário movimentar o gabinete ou o modem. É recomendável que o usuário verifique a conexão do cabo, tanto no modem quanto no gabinete do computador.

II. O modem pode não estar funcionando bem em decorrência, por exemplo, de sobrecarga no tráfego de informações. É recomendável que o usuário desligue o modem e ligue-o novamente após  alguns  segundos,  para  que  ele  seja  reiniciado e  o  seu  funcionamento  normal  seja restaurado.

III. O adaptador de rede pode estar desativado, o driver pode estar desatualizado ou a placa de rede pode estar danificada. É recomendável que o usuário atualize o driver do adaptador de rede,  ative-o,  caso  esteja  desativado,  ou  providencie  a  troca  da  placa  de  rede, caso  esteja danificada.

IV. O cabo ethernet coaxial pode ter se rompido devido ao seu núcleo de alumínio ser bastante sensível, principalmente nas proximidades dos conectores RJ-35 usados para fazer a ligação ao modem e ao gabinete do computador. É recomendável que o usuário faça uma verificação visual para saber se o cabo está rompido.

São problemas e ações corretas que podem ser tomadas para tentar resolvê-los o que consta APENAS em:

a) I, II e III.
b) I, III e IV.
c) III e IV.
d) I e II.
e) II e IV.


4. (FCC / DPE-RR / Técnico em Informática - 2015) A velocidade de transmissão 100 Mbit/s do Fast-Ethernet é alcançada com uma largura de banda de 31,25 MHz. Dessa forma, só é possível atender esta banda requerida com os cabos de par trançado de categoria:

a)  5 ou superior
b)  5a ou superior
c)  6a
d)  5e ou 6e
e)  6 ou superior

5. (FCC / DPE-RR / Técnico em Informática - 2015) Com relação ao meio de propagação do sinal, as fibras óticas podem ser classificadas em monomodo e multimodo. As fibras multimodo:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





100
132





a)  são usadas principalmente em LANs, pois têm um baixo custo e apresentam alto índice de refração quando comparadas com outras fibras.
b)  apresentam  desvantagem  no  alinhamento  dos  núcleos  nas  emendas  e  conectores  em relação às fibras monomodo.
c)  possuem  o  diâmetro  do  seu  núcleo  menor  se  comparado  com  o  núcleo  de  uma  fibra monomodo.
d)  têm taxas de transmissão mais altas, quando comparadas às fibras ópticas monomodo.
e)  são mais utilizadas em enlaces intercontinentais, nacionais e metropolitanos, devido à sua baixa atenuação para longas distâncias.
6. (FCC / TRE-RS / Auditor Público Externo - Engenharia Civil - Conhecimentos Básicos - 2014) Atualmente,  grande  parte  das  instalações  físicas  de  redes  de  computadores  é  realizada utilizando a tecnologia Ethernet com cabos de pares trançados. Neste tipo de instalação, 
a)  um defeito em um dos computadores conectados não afeta o funcionamento da rede.
b)  utilizam-se menos cabos do que em uma instalação semelhante utilizando cabos coaxiais.
c)  são disponibilizadas maior largura de banda e velocidade do que permitem os cabos de Fibra Óptica podem disponibilizar.
d)  o conector utilizado nas terminações dos cabos é denominado UTP.
e)  a topologia de rede estabelecida é do tipo Barramento.

7. (FCC / TRT - 1ª REGIÃO (RJ) / Analista Judiciário – Área Administrativa / 2013) Sabendo que uma intranet utiliza a infraestrutura de rede da empresa e fazendo uso das informações contidas no texto, considere que o computador de Paulo pode se comunicar com o computador servidor do Tribunal porque os recursos necessários estão fisicamente localizados em um raio de até 500 metros dentro do prédio do Tribunal, incluindo o computador de Paulo e o servidor. Isso significa que a rede utilizada é do tipo.

a)  WAN
b)  CAN
c)  LAN
d)  MAN
e)  ADSL

8. (FCC / SPPREV / Analista em Gestão Previdenciária - 2012) A topologia de uma rede de comunicação  refere-se  à  forma  com  que  os  enlaces  físicos  e  os  nós  de  comutação  estão organizados, determinando os caminhos físicos existentes e utilizáveis entre quaisquer pares de estações conectadas a essa rede.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





101
132






A denominação correta da Figura 1 é:

a)  Anel.
b)  Hierárquica
c)  Malha
d)  Barramento
e)  Estrela

9. (FCC / INSS / Técnico do Seguro Social - 2012) Pedro trabalha em uma pequena imobiliária cujo escritório  possui  cinco  computadores  ligados  em  uma  rede  com  topologia  estrela.  Os computadores nessa rede são ligados por cabos de par trançado a um switch (concentrador) que filtra e encaminha pacotes entre os computadores da rede, como mostra a figura abaixo.

Certo  dia,  Pedro  percebeu  que  não  conseguia  mais  se  comunicar  com  nenhum  outro computador da rede. Vários são os motivos que podem ter causado esse problema, EXCETO:

a)  O cabo de rede de um dos demais computadores da rede pode ter se rompido.
b)  A placa de rede do computador de Pedro pode estar danificada.
c)  A porta do switch onde o cabo de rede do computador de Pedro está conectado pode estar danificada.
d)  O cabo de rede que liga o computador de Pedro ao switch pode ter se rompido.
e)  Modificações  nas  configurações  do  computador  de Pedro  podem  ter  tornado  as configurações de rede incorretas.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





102
132




10. (FCC / MPE-RS / Agente Administrativo - 2008) Os dispositivos de rede de computadores que são interconectados física e logicamente para possibilitar o tráfego de informações pelas redes compõem layouts denominados.

a)  Protocolos.
b)  Topologias.
c)  Roteamentos.
d)  Arquiteturas.
e)  Cabeamento.

11. (FCC / TRT-PE / Analista Administrativo - 2018) Um Analista comprou um roteador wireless e o conectou por cabo em um switch para acessar a estrutura de rede cabeada. Isso permitiu que todos os dispositivos sem fio conectados nesse roteador tivessem acesso a todos os serviços disponíveis na rede cabeada, como por exemplo, acesso à internet. Nesse caso, o roteador foi configurado pelo Analista para operar no modo:

a)  ponto-a-ponto.
b)  access point.
c)  bridge.
d)  modem.
e)  backbone.

12. (FCC / SEGEP-MA / Técnico de Fiscalização Agropecuária - 2018) A tecnologia de rede de computadores:

a)  WiMax foi desenvolvida para funcionar em redes locais, tendo curto alcance, justamente o oposto do Wi-Fi, que foi desenvolvido para funcionar em redes metropolitanas. As duas tecnologias atuam de forma complementar.

b)  Wi-Fi permite o acesso à internet da casa ou da empresa de um usuário através de ondas do tipo bluetooth. O usuário poderá acessar a internet a até 1 km do aparelho receptor.

c)  3G é uma das possibilidades de conexão de computadores usando banda larga sem fio. O sistema  permite  que  voz,  dados  e  imagens  sejam  transmitidos  e  acessados  em  alta velocidade, via satélite.

d)  Wi-Fi não precisa de cabeamento, pois o sinal de internet chega, por infravermelho, até o roteador através da infraestrutura sem fio da rede telefônica ou da TV a cabo.

e)  WiMax  é  uma  evolução  da  Wi-Fi,  sendo  uma  tecnologia  que  permite  acesso  sem  fio  à internet.

13. (FCC / METRÔ-SP / Oficial Logística de Almoxarifado - 2018) Em uma empresa há um modem, que também é roteador, que recebe o sinal de Internet e o distribui por cabo e via wireless para Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





103
132




computadores e dispositivos móveis dos funcionários. Como esse roteador não possui portas suficientes  para  ligar  por  cabos  outros  5  computadores,  um  técnico  sugeriu  utilizar  um equipamento  que,  ligado  ao  roteador,  poderá  oferecer  portas  suficientes  para  ligar  outros computadores do escritório, permitindo, inclusive, acesso à Internet. O equipamento sugerido foi um:

a)  switch.
b)  hub usb.
c)  dmz.
d)  proxy.
e)  vnc bridge.

14. (FCC / SEGEP-MA / Fiscal Estadual Agropecuário - 2018)  Uma  agência  recebe  o  sinal  da internet via cabo de fibra ótica em um modem, que está ligado a um dispositivo que funciona como um ponto de encontro, distribuindo o sinal da internet para todos os computadores e permitindo que eles se comuniquem por cabos de rede. Nesta situação, esse dispositivo é:

a)  switch.
b)  web server.
c)  firewall.
d)  hub USB.
e)  dmz server.

15. (FCC / TRE-SP / Técnico Judiciário - Área Administrativa - 2012) Para que o computador de uma residência possa se conectar à Internet, utilizando a rede telefônica fixa, é indispensável o uso de um hardware chamado:

a)  hub.
b)  Modem.
c)  Acess point.
d)  Adaptador 3G.
e)  Switch.

16. (FCC / SEE-MG / Especialista em Educação - Supervisão Pedagógica- 2012) É usado para centralizar um ponto de acesso para Internet em uma rede e/ou criar uma rede de computadores com ou sem cabos para conectá-los. Pode ser utilizado em lugares como aeroportos e escolas com redes sem fio.

O texto refere-se ao dispositivo de redes chamado:

a)  Switch.
b)  Roteador wireless.
c)  WI-FI hub.
d)  Cable modem wireless.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





104
132





17. (FCC / TRT - 4ª REGIÃO (RS) / Técnico Judiciário - Área Administrativa- 2011) Numa rede LAN (Local Area Network), o recurso de hardware mínimo que deverá estar instalado no computador para permitir a comunicação com os demais elementos da rede é:

a)  o teclado.
b)  o hub.
c)  o cartão de memória.
d)  o switch.
e)  a placa de rede.

18. (FCC / INFRAERO / Técnico de Segurança do Trabalho - 2011) Sobre a infraestrutura para uma Intranet, considere:

I. Wireless é um padrão específico de uma tecnologia de redes sem fio.
II. Wi-Fi refere-se genericamente à transmissão de dados sem a utilização de meios físicos.
III. WLAN é uma rede local sem fio para fazer conexão com a Internet ou entre os dispositivos da rede.

Está correto o que se afirma em:

a)  I, apenas.
b)  III, apenas.
c)  I e II, apenas.
d)  II e III, apenas.
e)  I, II e III.

19. (FCC / TRE-TO / Analista Judiciário - Área Administrativa - 2011) Os dispositivos que têm como principal função controlar o tráfego na Internet são denominados:

a) Switches.
b) Comutadores.
c) Roteadores.
d) Firewalls.
e) Web servers.

20. (FCC  /  TRE-AL  /  Analista  Judiciário  -  Área  Judiciária  -  2010)  Ao  compartilhar  pastas  e impressoras entre computadores, evitando que pessoas não autorizadas possam acessar os arquivos pela Internet, pode-se montar a rede usando um firewall, baseado em hardware, por meio do dispositivo denominado:

a) Hub
b) Switch
c) Roteador
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





105
132




d) Repetidor
e) Cross-over

21. (FCC / SEFAZ-SC / Auditor Fiscal da Receita Estadual - 2018) O Auditor Fiscal foi designado para  especificar  a  aquisição  de  um  dispositivo  de  rede  de  computadores  para  realizar  a interconexão e a comunicação entre uma rede Ethernet e uma rede Token-Ring. O dispositivo especificado pelo Auditor deve ser:

a) Hub.
b) Firewall.
c) Switch.
d) Roteador.
e) Bridge.



























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





106
132




GABARITO – FCC
1. LETRA E
2. LETRA B
3. LETRA A
4. LETRA A
5. LETRA A
6. LETRA A
7. LETRA C
8. LETRA D
9. LETRA A
10. LETRA B
11. LETRA B
12. LETRA E
13. LETRA A
14. LETRA A
15. LETRA B
16. LETRA B
17. LETRA E
18. LETRA B
19. LETRA C
20. LETRA C
21. LETRA E













Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





107
132




QUESTÕES COMENTADAS – BANCAS DIVERSAS 
1. (CESGRANRIO / CEFET-RJ – 2014) Os tipos de rede digital podem ser classificados em função dos seus alcances geográficos. A rede com alcance de até 500 metros, utilizada em escritórios ou andares de um edifício, é denominada rede local e é conhecida pela sigla:

a)  LAN
b)  RAN
c)  CAN
d)  MAN
e)  WAN

Comentários:

Apesar de a questão ter mencionado um alcance de até 500 metros, não se atenham tanto a medidas precisas. Pensem sempre em uma variação de valores.

Gabarito: Letra A

2. (CESGRANRIO / TRANSPETRO – 2011) 


A figura acima mostra uma topologia típica de uma rede industrial de comunicação onde todos os  dispositivos  compartilham  o  mesmo  meio  físico  de  comunicação.  O  controle  pode  ser centralizado  ou  distribuído.  Além  de  possuir  alto  poder  de  expansão,  nós  com  falha  não prejudicam necessariamente os demais. Qual a topologia descrita?

a)  Anel.
b)  Barramento.
c)  Ponto-a-Ponto.
d)  Árvore.
e)  Estrela.

Comentários:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





108
132




Como todos os dispositivos compartilham o mesmo meio físico de comunicação, com alto poder de expansão e cuja falha em um nó não prejudicam necessariamente os demais, trata-se da Topologia em Barramento.

Gabarito: Letra B

3. (CESGRANRIO  /  PETROBRAS  –  2011)  Uma  das  desvantagens  da  utilização  de  redes  de computadores com topologia em estrela é que, em caso de:

a)  desconexão de uma estação, todas as demais estarão também desconectadas da rede.
b)  alto tráfego de dados, a velocidade será bastante reduzida.
c)  falha do dispositivo central, toda a rede será paralisada.
d)  erros de conexão, o isolamento desses erros torna-se difícil e)  colisões de dados, todos os equipamentos serão afetados.

Comentários:

Em uma rede com topologia em estrela, caso haja falha no dispositivo central, toda a rede será prejudicada.

Gabarito: Letra C

4. (CESGRANRIO / CEFET-RJ – 2014) O Bluetooth é um(a):

a)  padrão da instalação para redes Ethernet.
b)  sistema de armazenamento não volátil de alta capacidade.
c)  tecnologia de compressão de dados para redes sem fio.
d)  tecnologia para comunicação sem fio de curta distância.
e)  interface física para ligações entre computadores com par trançado.

Comentários:

O bluetooth é uma tecnologia para comunicação sem fio de curta distância. Nenhum dos outros itens faz o menor sentido!

Gabarito: Letra D

5. (CESGRANRIO / Banco do Brasil – 2014) Uma pessoa contratou um serviço de acesso à Internet via cabo. O tipo de serviço contratado dá direito a apenas um ponto de acesso, embora ela precise de mais três. Durante uma conversa com um de seus amigos, ela ficou sabendo que o problema  poderia  ser  facilmente  resolvido,  bastando,  para  tal,  que  ela  comprasse  um equipamento para disponibilizar uma rede sem fio em sua casa. Esse equipamento deverá ser conectado ao aparelho ao qual foi conectado o cabo que recebe os sinais enviados pela empresa Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





109
132




responsável pelo serviço. Posteriormente, o aparelho, que deverá ser comprado, irá retransmitir esses sinais, via Wi-Fi, para os demais computadores da casa, interconectando, assim, as duas redes.

O equipamento que essa pessoa deve comprar chama-se:

a)  usb
b)  modem
c)  bluetooth
d)  roteador
e)  adaptador de rede 
Comentários:

A questão afirma que esse equipamento deverá ser conectado ao aparelho ao qual foi conectado o cabo que recebe os sinais enviados pela empresa responsável pelo serviço. Em outras palavras, ele deve ser conectado ao modem. Ademais, a questão afirma que ele retransmitirá sinais, via wi-fi, para os demais computadores da casa, interconectando duas redes.

Isso é claramente uma funcionalidade do roteador. Os roteadores são equipamentos que permitem interligar várias redes e escolher a melhor rota para que  a informação chegue ao destino. Ele permite que você compartilhe a internet que veio do modem e é responsável por controlar o tráfego da internet.

Gabarito: Letra D

6. (CESGRANRIO / Banco da Amazônia – 2013) As redes de computadores caracterizam-se pelo compartilhamento de recursos lógicos e físicos, por meio de sistemas de comunicação. Entre os recursos físicos de uma rede, NÃO se incluem os:

a)  modems
b)  repetidores
c)  softwares
d)  transceptores
e)  switches

Comentários:

Nós já falamos bastante de Modem e Switches. Sobram: Repetidores, Software e Transceptores.
Um repetidor nada mais é que um dispositivo que recebe um sinal e o repete. Não falamos em transceptores, mas eles são dispositivos que recebem um tipo de sinal e o convertem em outro. No entanto, não precisávamos falar nada disso para resolver a questão. Bastava perceber que ela fala em recursos
físicos. E nós sabemos que softwares não são recursos físicos, mas lógicos.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





110
132




Gabarito: Letra C

7. (CESGRANRIO / CMB – 2012) Os softwares navegadores são ferramentas de internet utilizadas para a interação dos usuários com a rede mundial. Para que essa interação seja possível, é necessário fazer uma conexão à internet por um dos diversos meios de acesso disponíveis aos usuários.

O  meio  de  acesso  no  qual  o  usuário  utiliza  um  modem  e  uma  linha  de telefonia  fixa para conectar-se com a internet é o:

a)  dial up
b)  rádio
c)  satélite
d)  wi-fi
e)  cabo coaxial

Comentários:

A utilização de um modem e uma linha de telefonia fixa poderia ser Dial-Up ou ADSL. Como a questão só trouxe a opção Dial-Up, ela é a correta!

Gabarito:
Letra A

8. (CESGRANRIO / PETROBRAS – 2011) Dentro dos padrões da IEEE, qual a velocidade máxima de transmissão, em Mbps, de um Acess Point Wireless que utilize a tecnologia 802.11b?

a)  11
b)  25
c)  32
d)  47
e)  54

Comentários:

EVOLUÇÃO DO PADRÃO WIRELESS (802.11) PADRÃO  FREQUÊNCIA  TAXA DE TRANSMISSÃO IEEE 802.11b 2.4 Ghz 11 Mbps 
O Padrão IEEE 802.11b possui Velocidade/Taxa de Transmissão de 11 Mbps.

Gabarito: Letra A

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





111
132




9. (SOUSÂNDRADE / CRC-MA – 2010) Considere um arranjo de dois ou mais computadores conectados fisicamente por meio de cabos. Dentre as palavras abaixo, selecione aquela que melhor descreve esse cenário.

a) Rede
b) WAN
c) Wireless
d) Ponto de Acesso
e) Servidor

Comentários:

Vamos relembrar o conceito básico de redes: conjunto de dispositivos conectados por links de comunicação. Logo, um arranjo de dois ou mais computadores conectados fisicamente por meio de cabos é uma rede.

Gabarito: Letra A

10. (PUC-PR / TCE-MS  – 2013) Para  a  instalação  de  uma  rede  de  computadores,  utilizando  a topologia estrela, é necessário utilizar equipamentos que interligam e concentram os cabos de rede conectados aos computadores, impressoras e outros dispositivos que compartilhem esse meio de comunicação. Entre esses equipamentos de concentração de cabos, um deles é capaz de realizar a comunicação entre os dispositivos de modo mais inteligente, evitando replicação desnecessária  de  informação.  Ele  faz  isso  memorizando  os  endereços  dos  equipamentos conectados a cada porta, estabelecendo canais independentes de comunicação. Qual o nome desse dispositivo?

a) Switch.
b) Hub.
c) Placa de rede.
d) Replicador.
e) Gateway.


Comentários:

(a) Correto. Switch é um equipamento que permite a conexão física de cabos provenientes de diversos  nós,  memorizando  endereços  conectados  a  cada  porta  e  estabelecendo  canais independentes de comunicação; (b) Errado. Hub não é um dispositivo inteligente, entre outras características; (c) Errado. Placa de Rede é um dispositivo cuja função é adequar o formato dos dados para que estes possam ser transmitidos a um computador de uma rede através de um cabo ou através de tecnologia sem fio; (d) Errado. Esse dispositivo não existe; (e) Errado. Gateway é um equipamento que permite a comunicação entre duas aplicações diferentes, como duas redes que utilizem protocolos diferentes e o compartilhamento de conexão da internet entre várias estações.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





112
132




Gabarito: Letra A

11. (FUNRIO / CBM-GO – 2016) A topologia de rede na qual toda a informação passa de forma obrigatória por uma estação central inteligente, sendo que esta central deve conectar cada estação da rede e distribuir o tráfego, é denominada de:

a) linear.
b) barramento.
c) estrela.
d) token
e) anel.

Comentários:

(a) Errado. Nessa topologia, o tráfego passa por todos os elementos e, não somente, por uma estação central que distribui o tráfego (em completo desuso);

(b)  Errado.  Nessa  topologia,  cada  computador  está  ligado  a  um  barramento  central  e,  não, diretamente um ao outro – como na topologia linear;

(c) Correto. Nessa topologia, as estações estão ligadas através de uma conexão ponto-a-ponto dedicada a um nó ou estação central controladora, pela qual passam todas as mensagens;

(d) Errado. Essa tecnologia pode utilizar topologia em estrela ou anel, no entanto somente um computador transmite uma mensagem por vez – aquele que possui o token;

(e) Errado. Essa topologia definitivamente não possui uma estação central inteligente capaz de conectar todas as estações e distribuir o tráfego.

Gabarito: Letra C

12. (FUNRIO / Prefeitura de Mesquita – 2016) As redes de computadores cabeadas com acesso à internet seguem os padrões Fast Ethernet/Gigabit Ethernet e são implementadas por meio da topologia estrela. Em tal topologia, são usados conectores conhecidos pela sigla RJ-45, cuja imagem está representada na seguinte opção:

a)
b)
c)
d)
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





113
132




e)

Comentários:

(a) Errado, trata-se de um Conector PS2 – utilizado antigamente para conectar basicamente mouse e teclado;

(b) Correto, trata-se de um Conector RJ-45 – utilizado para conectar cabos de par trançado a uma placada de rede;

(c)  Errado,  trata-se  de  um  Conector  USB  –  utilizado  para  conectar  diversos  dispositivos  ao computador;

(d) Errado, trata-se de um Conector HDMI – utilizado para conectar dispositivos de áudio e/ou vídeo;

(e) Errado, trata-se de um Conector BNC – utilizado para conectar sinais de TV e algumas redes de computador (está em desuso).

Gabarito:
Letra B

13. (FUNRIO / MDIC – 2009) "Computadores compartilhando seus recursos através de sinais de rádio sem o uso de cabos ou fios". O texto descreve um(a):

a) Intranet.
b) Backbone.
c) Internet.
d) Access Point.
e) Wireless Lan.

Comentários:

(a)  Errado,  Intranet  é  uma  rede  de  computadores  privada  que  utiliza  a  mesma  tecnologia  da internet;

(b) Errado, Backbone (em inglês, espinha dorsal) é a infraestrutura central que interliga grandes redes de alto desempenho;

(c) Errado, Internet é a rede mundial de computadores, em que seu uso típico não se trata de uso de sinais de rádio sem o uso de cabos ou fios;

(d) Errado, Access Point é um dispositivo que permite a conexão de uma rede sem fio. Não se trata – portanto – de computadores compartilhando recursos;

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





114
132




(e) Correto, Wireless LAN (WLAN) é uma rede de computadores compartilhando seus recursos através de sinais de rádio sem o uso de cabos ou fios.

Em outras palavras, é uma Rede Local Sem Fio. Para que os dispositivos se comuniquem, são utilizadas ondas de rádio. Portanto, trata-se do Wireless LAN.

Gabarito: Letra E

14. (IDECAN / Câmara Municipal de Coronel Fabriciano/MG – 2017) Sobre as topologias de rede, analise a seguinte afirmativa: “implementada para prover a maior proteção possível contra interrupções de serviço. Nessa topologia cada host tem suas próprias conexões com todos os outros hosts”. Assinale a alternativa correta acerca dessa afirmativa.

a) Anel.
b) Malha.
c) Estrela.
d) Barramento.

Comentários:

Maior proteção contra interrupções de serviço; e cada host tem suas próprias conexões com todos os outros hosts; ambas são características da topologia de malha.

Gabarito:
Letra B

15. (IDECAN  /  Câmara  Municipal  de  Coronel  Fabriciano/MG  –  2017) “É  constituído  por  um condutor interno cilíndrico, no qual é injetado o sinal, envolvido por outro condutor externo. O condutor interno é separado do externo por um elemento isolante. Envolvendo o conjunto há uma capa externa (blindagem) que evita irradiação e captação de sinais.” Trata-se de:

a) Fibra óptica.
b) Cabo coaxial.
c)  Cabo de rede STP (Shielded Twisted Pair).
d) Cabo de rede UTP (Unshieded Twisted Pair).

Comentários:

Meio de transmissão constituído por um condutor interno cilíndrico e envolvido por um condutor externo; separado por elemento isolante; envolve blindagem que evita irradiação e captação de sinais; tudo nos remete ao cabo coaxial. Lembrando que ele é capaz de cobrir longas distâncias, apesar de possuir uma taxa de transmissão menor que a de um cabo de par trançado.

Gabarito: Letra B
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





115
132





16. (IDECAN / UERN – 2016) Em Redes de Computadores o termo Topologia é utilizado para descrever como uma rede é organizada fisicamente. Algumas topologias são mais utilizadas, dependendo  do  tipo  de  arquitetura  que  se  deseja  utilizar.  Outras  são  mais  conhecidas exatamente  pela  sua  ampla  utilização.  “Uma  dessas  topologias  tem  como  característica  a condição de que cada dispositivo possui um link ponto a ponto dedicado a cada um dos demais dispositivos. Neste caso, o termo dedicado significa que esse link transporta dados apenas entre esses dois dispositivos que ele conecta.” Trata-se de:

a) Anel.
b) Malha.
c) Estrela.
d) Barramento.


Comentários:

Cada  dispositivo  possui  um  link  ponto-a-ponto  dedicado  a  cada  um  dos  demais  dispositivos?
Transporta dados apenas entre esses dois dispositivos? Ambas são características da topologia em malha.

Gabarito: Letra B

17. (IBFC / DPE/PR – 2017) Leia a frase abaixo referente aos conceitos de ambiente de Redes de Computadores:

“Uma  rede  tipicamente  __________é  a  própria  Internet  pelo  fato  de  abranger  uma  área geográfica global, interligando países e continentes. Por outro lado, a _________se refere a redes pequenas restritas a uma pequena área geográfica, normalmente é a rede em um prédio comercial, em um escritório ou em uma residência que abriga dispositivos que compartilham dados e recursos entre si. “.

Assinale a alternativa que completa correta e respectivamente as lacunas:

a) LAN - WAN
b) MAN - PAN
c) PAN - MAN
d) WAN - LAN


Comentários:

A WAN é uma Rede de Área Ampla. Quando uma empresa possui filiais em cidades ou países diferentes, ela pode criar uma WAN. Um ótimo exemplo de WAN é Internet! Sim, a Internet é uma WAN. Por outro lado, temos a LAN que é uma Rede de Área Local. Quem aí já foi a uma Lan House?
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





116
132




O nome já dá a dica, trata-se de uma LAN. A rede da sua casa também, assim como a rede do andar de um prédio ou de um órgão, ou até mesmo a rede de uma pequena faculdade é uma LAN.

Gabarito: Letra D

18. (IBFC / PC/CE – 2014) A rede de computador que interliga dispositivos numa rede local sem fios é denominada, tecnicamente, por:

a) Wi-Fi
b) Ethernet
c) Banda Larga
d) WAN


Comentários:

Questão bem tranquila! Uma das tecnologias mais usadas hoje em dia é o Wi-Fi, ou rede sem fio, que é utilizada para a transmissão de dados sem a necessidade de cabos.

Gabarito: Letra A

19. (IBFC / Câmara Municipal de Araraquara – 2017) Assinale, das alternativas abaixo, a única que Não  identifica  corretamente  um  dispositivo  básico  de  hardware  aplicado  em  redes  de computadores:

a) switch
b) browser
c) repetidor
d) modem


Comentários:

(a) Errado, o switch (também chamado de comutador) é considerado com uma evolução do HUB!
É um dispositivo capaz de receber uma informação de fora e enviá-la apenas ao destinatário; (b) Correto. O browser é o que conhecemos como navegador, tal como o Google Chrome, o Internet Explorer, etc; (c) Um repetidor nada mais é que um dispositivo que recebe um sinal e o repete. São utilizados para ampliar o sinal da rede wi-fi; (d) Errado. O modem é um dispositivo eletrônico de entrada/saída de dados que modula um sinal digital em um sinal analógico a ser transmitida por meio de uma linha telefônica e que demodula o sinal analógico e o converte para o sinal digital original.

Gabarito: Letra B

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





117
132




20. (FACET / Câmara Municipal de Uiraúna – 2016) As topologias das redes de computadores são as estruturas físicas dos cabos, computadores e componentes. Qual alternativa abaixo descreve a Topologia Ponto-a-ponto?

a)  Modelo  utilizado  nas  primeiras  conexões  feitas  pelas  redes  Ethernet,  se  trata  de computadores conectados em formato linear, cujo cabeamento é feito em sequência;

b) Modelo atualmente utilizado em automação industrial e na década de 1980 pelas redes Token Ring da IBM.

c) Modelo em que existe um ponto central (concentrador) para a conexão, geralmente um hub ou switch;

d) Quando as máquinas estão interconectadas por pares através de um roteamento de dados;

e)  Quando  as  máquinas  estão  interconectadas  por  um mesmo  canal  através  de  pacotes endereçados (unicast, broadcast e multicast).

Comentários:

(a) Errado, a questão trata da Topologia em Barramento; (b) Errado, a questão trata da Topologia em Anel; (c) Errado, a questão trata da Topologia em Estrela; (d) Correto, pero no mucho! Galera, ponto-a-ponto  é  uma  arquitetura  de  conexão  e,  não, uma  topologia.  Fazendo  vista  grossa,  a arquitetura  (chamada  de  topologia)  ponto-a-ponto  é realmente  quando  as  máquinas  estão interconectadas por pares através de um roteamento de dados; (e) Errado, isso não é topologia – é a forma de envio ou difusão de dados.

Gabarito: Letra D

21. (INAZ DO PARÁ / CORE-SP – 2019) A Internet se configura no mundo de hoje como uma das principais  ferramentas  de  comunicação  do  planeta.  Aponte  a  alternativa  que  apresenta conteúdo  correto  sobre  a  história  dessa  importante fonte  de  informação  dos  dias contemporâneos.

a) No final da década de 70, uma agência americana de projetos de pesquisa criou a base da estrutura de comunicação de dados que mais tarde se transformaria na Internet.

b) O tráfego eficiente de dados na grande rede somente começou a dar resultados positivos a partir da utilização do conjunto de protocolos de referência TCP/IP, desenvolvido no início da década de 70.

c)  A  Fundação  Nacional  da  Ciência,  instituição  americana  de  pesquisa  em  tecnologia, desenvolveu uma rede comercial chamada FNCNET, que mais tarde faria parte da configuração da Internet.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





118
132





d) Sua origem está fundamentada na implantação de uma rede experimental de computadores de longa distância, chamada ARPANET, formada por um conjunto de laboratórios americanos de pesquisa.

e)  Somente  foi  possível  consolidar  a  criação  da  Internet  após  a  adequada  junção  de  redes paralelas como a Intranet e a Extranet 
Comentários:

(a) Errado, foi criada no final da década de 60; (b) Errado, foi desenvolvido no início da década de 80; (c) Errado, essa fundação jamais existiu; (d) Correto, era uma rede experimental criada por um conjunto de laboratórios de pesquisas de universidades e era inicialmente chamada de ARPANET;
(e) Errado, não faz o menor sentido e foram criadas posteriormente.

Obs: cobrar data é uma das coisas mais absurdas que eu já vi em provas de concurso!

Gabarito: Letra D

22. (CONSULPLAN / Pref. de Pirapora – 2019) Qual o conceito de INTERNET?

a)  É  uma  rede  global  de  computadores,  interligada  por  equipamentos  e  protocolos  de comunicação.
b) Conjunto de regras que os equipamentos envolvidos no processo de comunicação deve seguir para que a ligação entre os mesmos permaneça estável.
c) Representação gráfica das informações.
d) Linhas e colunas com funções para trabalhar com números.

Comentários:

(a)  Correto,  é  realmente  uma  rede  global  de  computadores  interligada  por  equipamentos  e protocolos; (b) Errado, essa é a definição de protocolos de comunicação; (c) Errado, não faz o menor sentido; (d) Errado, essa é a definição de planilha eletrônica.

Gabarito: Letra A

23. (CONSULPLAN / Pref. de Resende – 2019) Podemos dizer que internet é um conjunto de redes interligadas através de Backbones que é o termo principal utilizado para:

a) Interpretar as páginas da web.
b) Enviar mensagens instantâneas pelos sites.
c) Solicitar informação em qualquer lugar do mundo por meio de sites.
d) Identificar a rede principal pela qual os dados de todos os clientes da Internet passam.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





119
132





Comentários:

A internet pode ser fornecida por meio de satélites, ondas de rádio ou uma rede de milhares de cabos de fibra óptica terrestres ou submarinos, que conectam diversos países, respondendo por 80% de toda a comunicação. Essa infraestrutura de redes – que forma a espinha dorsal da internet –  é  chamada  de backbone.  Ela  possui  alto  velocidade,  desempenho  e  interliga  várias  redes, garantindo o fluxo da informação por dimensões continentais. Todos os dados da Internet passam por essa infraestrutura de redes principal chamada backbone.

Gabarito: Letra D

24. (DÉDALUS / CORE/RJ – 2019) A Arpanet foi a propulsora do (a):

a) Windows.
b) Linux.
c) Internet.
d) Apple.
e) Google.

Comentários:

A Arpanet foi a propulsora da... Internet.

Gabarito: Letra C

25. (OBJETIVA / Prefeitura de Jaú – 2019) “Rede mundial que interliga computadores. Começou no final  dos  anos  60,  com  objetivos  militares,  e  se  caracteriza  por  ser  uma  rede  altamente descentralizada. É comumente chamada de www ou web”. Essa descrição refere-se a:

a) Intranet.
b) Link.
c) HTTP.
d) Internet


Comentários:

Rede mundial? Interliga computadores? Começou no final da década de 70? Tinha objetivos militares?
É uma rede altamente descentralizada? Tudo isso nos remete à Internet. Ao final, a questão afirma que é comumente chamada de www ou web. Sim, isso é verdadeiro, mas é errado! Internet e Web são conceitos completamente diferentes.

Gabarito:
Letra D
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





120
132





26. (AOCP / UNIR – 2018) O acesso à Internet só é possível por intermédio de uma entidade denominada provedor de acesso, o qual conecta o usuário à grande rede.

Comentários:

Perfeito! É realmente necessário contratar um provedor de acesso para se conectar à Internet.

Gabarito: Correto

27. (INAZ DO PARÁ / CREFITO – 2018) A grande rede ou internet foi criada pelos norte-americanos no tempo da guerra fria, esta tecnologia interliga computadores que compartilham dados entre si. Qual a rede que deu origem a internet?

a) BBS
b) ETHERNET
c) ARPANET
d) INTRANET
e) URL.

Comentários:

A rede que deu origem a Internet era a ARPANET! Professor, por que a questão foi anulada? Não faço ideia, porque a banca não divulgou.

Gabarito: Anulada

28. (CRESCER-GM / Prefeitura de Lourdes – 2017) "É um conglomerado de redes locais espalhadas pelo mundo". Essa é a definição de:

a) Intranet.
b) Internet.
c) Extranet.
d) LAN.

Comentários:

Conglomerado de redes locais espalhadas pelo mundo é a definição de... Internet.

Gabarito: Letra B

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





121
132




29. (EXATUS-AJ  /  TER-SC  –  2016) É  um  conglomerado  de  redes  locais,  interconectadas e espalhadas  pelo  mundo  inteiro,  através  do  protocolo  de  internet  facilitando  o  fluxo  de informações espalhadas por todo o globo terrestre.

a) Intranet.
b) LAN.
c) Internet.
d) Extranet:

Comentários:

Mais  uma  vez!  Conglomerado  de  redes  locais,  interconectadas  e  espalhadas  pelo  mundo  é  a definição de... Internet.

Gabarito: Letra C

30. (FEPESE / CELESC – 2016) Como é conhecida a estrutura mundial de redes que pode  ser acessada por todos os usuários com acesso controlado por protocolos?

a) Força
b) Internet
c) Convenção
d) Hard reset
e) TCP/IP.

Comentários:

Estrutura mundial de redes cujo acesso é controlado por protocolos? Trata-se da Internet!

Gabarito: Letra B

31. (FUNRIO  /  UFRB  –  2015) O  hardware  de  computador,  além  da  unidade  central  de processamento e da memória, é composto de dispositivos de entrada e saída, que permitem a comunicação com o usuário. O dispositivo padrão de entrada é o teclado e o dispositivo padrão de saída é o monitor. Alguns dispositivos são chamados híbridos porque podem funcionar tanto como dispositivo de entrada e como de saída. Qual alternativa é um exemplo de dispositivo híbrido (de entrada e saída)?

a) Microfone.
b) Mouse.
c) Alto Falante.
d) Scanner.
e) Placa de rede.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





122
132





Comentários:

A placa de rede permite uma comunicação bidirecional (transmissão e recebimento de dados).
Logo, é um dispositivo híbrido de entrada/saída de dados.

Gabarito:
Letra E

32. (FEC / MPA – 2010) Das opções seguintes, aquela que contém apenas tecnologias de acesso à Internet é:

a) Dial-up, ISDN,3G e Firewire.
b) ISDN, Firewire, ADSL e 3G.
c) 3G, Dial-up, Firewire e ADSL.
d) ADSL, ISDN, Dial-up e 3G.
e) Firewire, ADSL, Dial-up e ISDN.

Comentários:

A única opção que contém apenas tecnologias de acesso à Internet é ADSL, ISDN, Dial-up e 3G.

Gabarito:
Letra D

33. (MGS / MGS – 2015) O que é a Internet?

a) Uma rede de computadores.
b) Vários computadores interligados c) Uma rede mundial de computadores d) Uma rede mundial de celulares 

Comentários:

A Internet é a rede (mundial) de computadores! Logo, a questão possui duas respostas, mas temos que responder a mais correta: é uma rede mundial de computadores.

Gabarito:
Letra C





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





123
132




LISTA DE QUESTÕES – BANCAS DIVERSAS 
1. (CESGRANRIO / CEFET-RJ – 2014) Os tipos de rede digital podem ser classificados em função dos seus alcances geográficos. A rede com alcance de até 500 metros, utilizada em escritórios ou andares de um edifício, é denominada rede local e é conhecida pela sigla:

a)  LAN
b)  RAN
c)  CAN
d)  MAN
e)  WAN

2. (CESGRANRIO / TRANSPETRO – 2011) 


A figura acima mostra uma topologia típica de uma rede industrial de comunicação onde todos os dispositivos compartilham o mesmo meio físico de comunicação. O controle pode ser centralizado ou  distribuído.  Além  de  possuir  alto  poder  de  expansão,  nós  com  falha  não  prejudicam necessariamente os demais. Qual a topologia descrita?

a)  Anel.
b)  Barramento.
c)  Ponto-a-Ponto.
d)  Árvore.
e)  Estrela.

3. (CESGRANRIO  /  PETROBRAS  –  2011)  Uma  das  desvantagens  da  utilização  de  redes  de computadores com topologia em estrela é que, em caso de:

a)  desconexão de uma estação, todas as demais estarão também desconectadas da rede.
b)  alto tráfego de dados, a velocidade será bastante reduzida.
c)  falha do dispositivo central, toda a rede será paralisada.
d)  erros de conexão, o isolamento desses erros torna-se difícil e)  colisões de dados, todos os equipamentos serão afetados.

4. (CESGRANRIO / CEFET-RJ – 2014) O Bluetooth é um(a):
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





124
132





a)  padrão da instalação para redes Ethernet.
b)  sistema de armazenamento não volátil de alta capacidade.
c)  tecnologia de compressão de dados para redes sem fio.
d)  tecnologia para comunicação sem fio de curta distância.
e)  interface física para ligações entre computadores com par trançado.

5. (CESGRANRIO / Banco do Brasil – 2014) Uma pessoa contratou um serviço de acesso à Internet via cabo. O tipo de serviço contratado dá direito a apenas um ponto de acesso, embora ela precise de mais três. Durante uma conversa com um de seus amigos, ela ficou sabendo que o problema  poderia  ser  facilmente  resolvido,  bastando,  para  tal,  que  ela  comprasse  um equipamento para disponibilizar uma rede sem fio em sua casa. Esse equipamento deverá ser conectado ao aparelho ao qual foi conectado o cabo que recebe os sinais enviados pela empresa responsável pelo serviço. Posteriormente, o aparelho, que deverá ser comprado, irá retransmitir esses sinais, via Wi-Fi, para os demais computadores da casa, interconectando, assim, as duas redes.

O equipamento que essa pessoa deve comprar chama-se:

a)  usb
b)  modem
c)  bluetooth
d)  roteador
e)  adaptador de rede 
6. (CESGRANRIO / Banco da Amazônia – 2013) As redes de computadores caracterizam-se pelo compartilhamento de recursos lógicos e físicos, por meio de sistemas de comunicação.

Entre os recursos físicos de uma rede, NÃO se incluem os:

a)  modems
b)  repetidores
c)  softwares
d)  transceptores
e)  switches

7. (CESGRANRIO / CMB – 2012) Os softwares navegadores são ferramentas de internet utilizadas para a interação dos usuários com a rede mundial. Para que essa interação seja possível, é necessário fazer uma conexão à internet por um dos diversos meios de acesso disponíveis aos usuários.

O  meio  de  acesso  no  qual  o  usuário  utiliza  um  modem  e  uma  linha  de telefonia  fixa para conectar-se com a internet é o:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





125
132




a)  dial up
b)  rádio
c)  satélite
d)  wi-fi
e)  cabo coaxial

8. (CESGRANRIO / PETROBRAS – 2011) Dentro dos padrões da IEEE, qual a velocidade máxima de transmissão, em Mbps, de um Acess Point Wireless que utilize a tecnologia 802.11b?

a)  11
b)  25
c)  32
d)  47
e)  54

9. (SOUSÂNDRADE / CRC-MA – 2010) Considere um arranjo de dois ou mais computadores conectados fisicamente por meio de cabos. Dentre as palavras abaixo, selecione aquela que melhor descreve esse cenário.

a) Rede
b) WAN
c) Wireless
d) Ponto de Acesso
e) Servidor

10. (PUC-PR / TCE-MS  – 2013) Para  a  instalação  de  uma  rede  de  computadores,  utilizando  a topologia estrela, é necessário utilizar equipamentos que interligam e concentram os cabos de rede conectados aos computadores, impressoras e outros dispositivos que compartilhem esse meio de comunicação. Entre esses equipamentos de concentração de cabos, um deles é capaz de realizar a comunicação entre os dispositivos de modo mais inteligente, evitando replicação desnecessária  de  informação.  Ele  faz  isso  memorizando  os  endereços  dos  equipamentos conectados a cada porta, estabelecendo canais independentes de comunicação. Qual o nome desse dispositivo?

a) Switch.
b) Hub.
c) Placa de rede.
d) Replicador.
e) Gateway.

11. (FUNRIO / CBM-GO – 2016) A topologia de rede na qual toda a informação passa de forma obrigatória por uma estação central inteligente, sendo que esta central deve conectar cada estação da rede e distribuir o tráfego, é denominada de:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





126
132




a) linear.
b) barramento.
c) estrela.
d) token
e) anel.

12. (FUNRIO / Prefeitura de Mesquita – 2016) As redes de computadores cabeadas com acesso à internet seguem os padrões Fast Ethernet/Gigabit Ethernet e são implementadas por meio da topologia estrela. Em tal topologia, são usados conectores conhecidos pela sigla RJ-45, cuja imagem está representada na seguinte opção:

a)
b)
c)
d)
e)

13. (FUNRIO / MDIC –  2009) "Computadores compartilhando seus recursos através de sinais de rádio sem o uso de cabos ou fios". O texto descreve um(a):

a) Intranet.
b) Backbone.
c) Internet.
d) Access Point.
e) Wireless Lan.

14. (IDECAN / Câmara Municipal de Coronel Fabriciano/MG – 2017) Sobre as topologias de rede, analise a seguinte afirmativa: “implementada para prover a maior proteção possível contra interrupções de serviço. Nessa topologia cada host tem suas próprias conexões com todos os outros hosts”. Assinale a alternativa correta acerca dessa afirmativa.

a) Anel.
b) Malha.
c) Estrela.
d) Barramento.

15. (IDECAN  /  Câmara  Municipal  de  Coronel  Fabriciano/MG  –  2017) “É  constituído  por  um condutor interno cilíndrico, no qual é injetado o sinal, envolvido por outro condutor externo. O condutor interno é separado do externo por um elemento isolante. Envolvendo o conjunto há uma capa externa (blindagem) que evita irradiação e captação de sinais.” Trata-se de:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





127
132





a) Fibra óptica.
b) Cabo coaxial.
c)  Cabo de rede STP (Shielded Twisted Pair).
d) Cabo de rede UTP (Unshieded Twisted Pair).

16. (IDECAN / UERN – 2016) Em Redes de Computadores o termo Topologia é utilizado para descrever como uma rede é organizada fisicamente. Algumas topologias são mais utilizadas, dependendo  do  tipo  de  arquitetura  que  se  deseja  utilizar.  Outras  são  mais  conhecidas exatamente  pela  sua  ampla  utilização.  “Uma  dessas  topologias  tem  como  característica  a condição de que cada dispositivo possui um link ponto a ponto dedicado a cada um dos demais dispositivos. Neste caso, o termo dedicado significa que esse link transporta dados apenas entre esses dois dispositivos que ele conecta.” Trata-se de:

a) Anel.
b) Malha.
c) Estrela.
d) Barramento.


17. (IBFC / DPE/PR – 2017) Leia a frase abaixo referente aos conceitos de ambiente de Redes de Computadores:

“Uma  rede  tipicamente  __________é  a  própria  Internet  pelo  fato  de  abranger  uma  área geográfica global, interligando países e continentes. Por outro lado, a _________se refere a redes pequenas restritas a uma pequena área geográfica, normalmente é a rede em um prédio comercial, em um escritório ou em uma residência que abriga dispositivos que compartilham dados e recursos entre si. “.

Assinale a alternativa que completa correta e respectivamente as lacunas:

a) LAN - WAN
b) MAN - PAN
c) PAN - MAN
d) WAN - LAN


18. (IBFC / PC/CE – 2014) A rede de computador que interliga dispositivos numa rede local sem fios é denominada, tecnicamente, por:

a) Wi-Fi
b) Ethernet
c) Banda Larga
d) WAN


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





128
132




19. (IBFC / Câmara Municipal de Araraquara – 2017) Assinale, das alternativas abaixo, a única que Não  identifica  corretamente  um  dispositivo  básico  de  hardware  aplicado  em  redes  de computadores:

a) switch
b) browser
c) repetidor
d) modem


20. (FACET / Câmara Municipal de Uiraúna – 2016) As topologias das redes de computadores são as estruturas físicas dos cabos, computadores e componentes. Qual alternativa abaixo descreve a Topologia Ponto-a-ponto?

a)  Modelo  utilizado  nas  primeiras  conexões  feitas  pelas  redes  Ethernet,  se  trata  de computadores conectados em formato linear, cujo cabeamento é feito em sequência;

b) Modelo atualmente utilizado em automação industrial e na década de 1980 pelas redes Token Ring da IBM.

c) Modelo em que existe um ponto central (concentrador) para a conexão, geralmente um hub ou switch;

d) Quando as máquinas estão interconectadas por pares através de um roteamento de dados;

e)  Quando  as  máquinas  estão  interconectadas  por  um mesmo  canal  através  de  pacotes endereçados (unicast, broadcast e multicast).

21. (INAZ DO PARÁ / CORE-SP – 2019) A Internet se configura no mundo de hoje como uma das principais  ferramentas  de  comunicação  do  planeta.  Aponte  a  alternativa  que  apresenta conteúdo  correto  sobre  a  história  dessa  importante fonte  de  informação  dos  dias contemporâneos.

a) No final da década de 70, uma agência americana de projetos de pesquisa criou a base da estrutura de comunicação de dados que mais tarde se transformaria na Internet.

b) O tráfego eficiente de dados na grande rede somente começou a dar resultados positivos a partir da utilização do conjunto de protocolos de referência TCP/IP, desenvolvido no início da década de 70.

c)  A  Fundação  Nacional  da  Ciência,  instituição  americana  de  pesquisa  em  tecnologia, desenvolveu uma rede comercial chamada FNCNET, que mais tarde faria parte da configuração da Internet.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





129
132




d) Sua origem está fundamentada na implantação de uma rede experimental de computadores de longa distância, chamada ARPANET, formada por um conjunto de laboratórios americanos de pesquisa.

e)  Somente  foi  possível  consolidar  a  criação  da  Internet  após  a  adequada  junção  de  redes paralelas como a Intranet e a Extranet 
22. (CONSULPLAN / Pref. de Pirapora – 2019) Qual o conceito de INTERNET?

a)  É  uma  rede  global  de  computadores,  interligada  por  equipamentos  e  protocolos  de comunicação.
b) Conjunto de regras que os equipamentos envolvidos no processo de comunicação deve seguir para que a ligação entre os mesmos permaneça estável.
c) Representação gráfica das informações.
d) Linhas e colunas com funções para trabalhar com números.

23. (CONSULPLAN / Pref. de Resende – 2019) Podemos dizer que internet é um conjunto de redes interligadas através de Backbones que é o termo principal utilizado para:

a) Interpretar as páginas da web.
b) Enviar mensagens instantâneas pelos sites.
c) Solicitar informação em qualquer lugar do mundo por meio de sites.
d) Identificar a rede principal pela qual os dados de todos os clientes da Internet passam.

24. (DÉDALUS / CORE/RJ – 2019) A Arpanet foi a propulsora do (a):

a) Windows.
b) Linux.
c) Internet.
d) Apple.
e) Google.

25. (OBJETIVA / Prefeitura de Jaú – 2019) “Rede mundial que interliga computadores. Começou no final  dos  anos  60,  com  objetivos  militares,  e  se  caracteriza  por  ser  uma  rede  altamente descentralizada. É comumente chamada de www ou web”. Essa descrição refere-se a:

a) Intranet.
b) Link.
c) HTTP.
d) Internet

26. (AOCP / UNIR – 2018) O acesso à Internet só é possível por intermédio de uma entidade denominada provedor de acesso, o qual conecta o usuário à grande rede.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





130
132




27. (INAZ DO PARÁ / CREFITO – 2018) A grande rede ou internet foi criada pelos norte-americanos no tempo da guerra fria, esta tecnologia interliga computadores que compartilham dados entre si. Qual a rede que deu origem a internet?

a) BBS
b) ETHERNET
c) ARPANET
d) INTRANET
e) URL.

28. (CRESCER-GM / Prefeitura de Lourdes – 2017) "É um conglomerado de redes locais espalhadas pelo mundo". Essa é a definição de:

a) Intranet.
b) Internet.
c) Extranet.
d) LAN.

29. (EXATUS-AJ  /  TER-SC  –  2016) É  um  conglomerado  de  redes  locais,  interconectadas e espalhadas  pelo  mundo  inteiro,  através  do  protocolo  de  internet  facilitando  o  fluxo  de informações espalhadas por todo o globo terrestre.

a) Intranet.
b) LAN.
c) Internet.
d) Extranet:

30. (FEPESE / CELESC – 2016) Como é conhecida a estrutura mundial de redes que pode  ser acessada por todos os usuários com acesso controlado por protocolos?

a) Força
b) Internet
c) Convenção
d) Hard reset
e) TCP/IP.

31. (FUNRIO  /  UFRB  –  2015) O  hardware  de  computador,  além  da  unidade  central  de processamento e da memória, é composto de dispositivos de entrada e saída, que permitem a comunicação com o usuário. O dispositivo padrão de entrada é o teclado e o dispositivo padrão de saída é o monitor. Alguns dispositivos são chamados híbridos porque podem funcionar tanto como dispositivo de entrada e como de saída. Qual alternativa é um exemplo de dispositivo híbrido (de entrada e saída)?

a) Microfone.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





131
132




b) Mouse.
c) Alto Falante.
d) Scanner.
e) Placa de rede.

32. (FEC / MPA – 2010) Das opções seguintes, aquela que contém apenas tecnologias de acesso à Internet é:

a) Dial-up, ISDN,3G e Firewire.
b) ISDN, Firewire, ADSL e 3G.
c) 3G, Dial-up, Firewire e ADSL.
d) ADSL, ISDN, Dial-up e 3G.
e) Firewire, ADSL, Dial-up e ISDN.

33. (MGS / MGS – 2015) O que é a Internet?

a) Uma rede de computadores.
b) Vários computadores interligados c) Uma rede mundial de computadores d) Uma rede mundial de celulares 





















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





132
132




GABARITO – BANCAS DIVERSAS 
1. LETRA A
2. LETRA B
3. LETRA C
4. LETRA D
5. LETRA D
6. LETRA C
7. LETRA A
8. LETRA A
9. LETRA A
10. LETRA A
11. LETRA C
12. LETRA B
13. LETRA E
14. LETRA B
15. LETRA B
16. LETRA B
17. LETRA D
18. LETRA A
19. LETRA B
20. LETRA D
21. LETRA D
22. LETRA A
23. LETRA D
24. LETRA C
25. LETRA D
26. CORRETO
27. ANULADA
28. LETRA B
29. LETRA C
30. LETRA B
31. LETRA E
32. LETRA D
33. LETRA C

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 00
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 

