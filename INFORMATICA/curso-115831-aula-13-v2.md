

Livro Eletrônico
Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti 06315057411 - EVA CELESTE DE SOUZA 





1
102




Sumário
1 – Introdução ao Linux .................................................................................................................... 4 1.1 – Contexto Histórico ............................................................................................................... 4 1.2 – Conceitos Básicos .............................................................................................................. 10 1.3 – Interface Gráfica ................................................................................................................. 12 1.3.1 – GNOME....................................................................................................................... 14 1.3.2 – KDE ............................................................................................................................. 15 1.3.3 – XFCE............................................................................................................................ 16 1.3.4 – Unity ............................................................................................................................ 17 1.4 – Rotinas de Inicialização ...................................................................................................... 18 1.4.1 – LILO ............................................................................................................................. 20 1.4.2 – GRUB ........................................................................................................................... 21 1.5 – Tipo de Usuário ................................................................................................................. 22 1.5.1 – Usuário Comum ........................................................................................................... 22 1.5.2 – Usuário Administrador (Root) ...................................................................................... 22 1.5.3 – Usuário de Sistema ...................................................................................................... 22 2 – Distribuições Linux ................................................................................................................... 24 2.1 – Ubuntu ............................................................................................................................... 26 2.2 – Debian ............................................................................................................................... 27 2.3 – Fedora ............................................................................................................................... 28 2.4 – Suse ................................................................................................................................... 29 2.5 – Mint .................................................................................................................................... 30 2.6 – CentOS .............................................................................................................................. 31 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





2
102




2.7 – Mandriva ............................................................................................................................ 32 2.8 – Slackware ........................................................................................................................... 33 2.9 – Kurumin.............................................................................................................................. 34 3 – Gerenciamento de Sistemas de Arquivos ................................................................................ 35 3.1 – Sistemas de Arquivos ......................................................................................................... 35 3.1.1 – EXT2 ............................................................................................................................ 36 3.1.2 – EXT3 ............................................................................................................................ 36 3.1.3 – EXT4 ............................................................................................................................ 36 3.1.4 – ReiserFS ....................................................................................................................... 36 3.2 – Estrutura de Diretórios ....................................................................................................... 37 3.3 – Gerenciamento de Privilégios ............................................................................................ 41 4 – Principais Comandos ................................................................................................................ 45 4.1 – Tipos de Comandos ........................................................................................................... 47 4.1.1 – Comandos Internos ..................................................................................................... 47 4.1.2 – Comandos Externos .................................................................................................... 47 4.2 – Comando ls ........................................................................................................................ 48 4.3 – Comando cd ...................................................................................................................... 52 4.4 – Comando cp ...................................................................................................................... 53 4.5 – Comando rm ...................................................................................................................... 54 4.6 – Comando rmdir.................................................................................................................. 55 4.7 – Comando mv ..................................................................................................................... 56 4.8 – Comando man ................................................................................................................... 57 4.9 – Comando df ....................................................................................................................... 58 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





3
102




4.10 – Comando sudo ................................................................................................................ 59 4.11 – Comando grep ................................................................................................................ 60 4.12 – Comando cat ................................................................................................................... 61 4.13 – Comando apt-get ............................................................................................................ 62 4.14 – Comando chmod ............................................................................................................. 63 4.15 – Outros comandos ............................................................................................................ 64 Resumo .......................................................................................................................................... 65 Sistema Operacional: Linux ........................................................................................................ 65 Mapa Mental .................................................................................................................................. 69 Exercícios Comentados – DIVERSAS BANCAS .............................................................................. 72 Lista de Exercícios – DIVERSAS BANCAS ...................................................................................... 91 Gabarito – DIVERSAS BANCAS ................................................................................................... 102 

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





4
102




1 – INTRODUÇÃO AO LINUX 1.1 – CONTEXTO HISTÓRICO 
Um Sistema Operacional é basicamente um software especial executado em seu computador para possibilitar  a  inicialização  e  a  execução  de  programas.  Atualmente,  existem  diversos  sistemas operacionais no mercado! Um deles é maduro, eficiente, poderoso, moderno e atual – além de acompanhar todas as mudanças tecnológicas de hardware e software dos últimos quarenta anos
! Não, eu não estou falando do Windows! Eu estou falando sobre o Unix...

Professor, você escreveu errado: é Linux! Não,  galera...  estou  falando  sobre  o  Unix!
O Unix é um
sistema  operacional  multitarefa  e  multiusuário,  disponível  para  diversas  plataformas  de hardware
. Ele foi criado no final da década de 1960, quando os computadores eram grandes, caros e de difícil acesso a pessoas comuns. Logo, era imprescindível desenvolver um sistema operacional multiusuário, multitarefa e que funcionasse em diferentes computadores.

O Unix multiusuário,  isto  é,  permitia  que  vários  usuários  utilizassem o  mesmo  computador  ao mesmo tempo por meio de terminais remotos. Ademais, ele era multitarefa, isto é, permitia que vários  programas  fossem  executados  simultaneamente.  Não  é  só  isso:  ele  apresenta  uma  vasta gama de possibilidades relacionadas à rede, com o sistema de cota de disco, FTP, e-mail, WWW, DNS, possibilidade de diferentes níveis de acesso, de executar programas em background etc.

No início, o Unix era distribuído gratuitamente pela AT&T Corporation para as universidades.
Mais tarde, porém, percebendo o sucesso do Unix no meio comercial, a empresa passou a disponibilizá-lo  por  um  preço  muito  alto .  Já  os  departamentos  de  ciência  da  computação  de Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





5
102




diversas universidades no mundo inteiro começaram a desenvolver programas comerciais para o Unix, gerando um grande número de usuários e desenvolvedores de utilitários e programas.

Até meados da década de 1980, o Unix ainda não possuía uma interface gráfica própria. Como assim, professor? Galera, vocês – assim como eu – são jovens, então vocês não sabem o que é um sistema operacional sem interface gráfica, somente com linha de comando! O Professor Renato da Costa – que tem o dobro da minha idade – conhece muito bem, porque ele já trabalhou muito com isso.
Então, para quem nunca viu, eu mostro abaixo um sistema operacional somente com linha de comando – não tem ícone, não tem janela, não tem nada disso...

Claro que, com o passar do tempo, ele implementou uma interface gráfica bonitinha e tal. Ele se tornou referência na comunidade tecnológica, em grande parte devido ao seu design elegante, a sua simplicidade e a sua portabilidade . E foi o sistema operacional mais popular e relevante do mundo até o início da década de noventa, quando o Microsoft Windows começou a se popularizar.
No entanto, foi com as distribuições de Linux que o Unix teve mais influência.



Professor, não gosto desse tal de Unix! Parece antigo, feio e coisa desses nerds de informática! Pequeno gafanhoto, você sabe qual sistema operacional que roda nesses dois computadores acima? Mac OS – um sistema operacional baseado em Unix!
Então, diga não ao preconceito contra o Unix – ele é Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





6
102




um excepcional sistema operacional e merece uma chance. Uma outra versão do Unix é o tema da nossa aula de hoje: Linux! Vamos ver um pouquinho sobre ele...



Como afirma o Professor Rubem E. Ferreira: “Linux é um clone de Unix criado como uma alternativa barata e funcional para quem não está disposto a pagar o alto preço de um sistema Unix comercial ou não  tem  um  computador  suficientemente  rápido”.  Vamos  contar  melhor  essa  história:  havia  um pesquisador chamado Richard Stallman que fundou a Free Software Foundation, uma organização para difundir softwares cujo código-fonte é livre para qualquer um acessar, estudar, copiar e modificar
.

Um dos projetos da Free Software Foundation era o Projeto GNU, que tinha como finalidade criar uma cópia melhorada e livre do sistema operacional Unix, mas que não utilizasse seu código-fonte
.  Como  nós  já  vimos,  o  Unix  era  bastante  caro  na  época.  Pessoal,  era  um  projeto extremamente ambicioso e trabalhoso: havia a necessidade de desenvolver o Kernel, Utilitários de Programação, Administração de Sistema, Administração de Rede, Comandos, entre outros.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





7
102






Uma pequena pausa:
kernel é o núcleo de um Sistema Operacional – ele é o responsável por se comunicar e controlar o hardware! Para quem gosta de carros, eu gosto de dizer que o Kernel é como o chassi de um veículo, isto é, a estrutura que suporta outros componentes. Da mesma forma que  o  chassi  –  que  pode  ser  utilizado  em  vários  carros  –,  o  kernel  pode  ser  utilizado  em  vários sistemas operacionais. Na imagem acima, vemos dois carros com o mesmo chassi!

Voltando  à  história:  no  final  da  década  de  1980,  o projeto  havia  fracassado  –  apenas  alguns utilitários  de  programação  e  alguns  comandos  estavam  prontos;  o  kernel,  nada.  Nessa  mesma época, havia outras iniciativas paralelas:
Dr. Andrew Tanenbaum desenvolveu o Minix – um clone do Unix – como instrumento de ensino para seus alunos sobre os princípios estruturais dos sistemas operacionais .

No entanto, o Minix era limitado para um processador bastante específico e tinha dificuldades em lidar com mais de uma tarefa. Professor, desenrola! Calma, estamos chegando lá! No final da década de oitenta,
um garoto de 22 anos chamado Linus Benedict Torvalds – aluno da Universidade de Helsinque  –  percebeu  que  o  percebeu  que  havia  um  processador  que  seria  perfeito  para executar o clone do Unix: Intel 80386 .

Galera,  pensem  numa  aposta  bem-feita:  esse  processador  revolucionou  o  mundo  naquela época.
Perguntem sobre ele para alguém da sua família com um pouco mais de idade que tenha adquirido  um  computador  no  início  da  década  de  noventa!  Ele  provavelmente  te  falará  com saudade: “Claro que eu lembro. Meu primeiro computador foi um 386!”! Certeza que depois disso cairá uma lágrima dos olhos dele...


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





8
102




Linus  –  esse  senhor  educado  da  foto  ao  lado  –  estava  disposto  a construir  um  kernel  clone  do  Unix  que  possuísse  memória  virtual, multitarefa  preemptiva  e  capacidade  de   multiusuários.
Era  um
trabalho  gigantesco  e,  na  prática,  impossível  para apenas  uma pessoa  concluí-lo,  ainda  que  estivesse  familiarizada  com  as complexidades dos sistemas operacionais.  Na  primavera  de  1991, ele  iniciou  seu  projeto  particular,  inspirado  no  seu  interesse  pelo Minix. Depois de algum tempo de trabalho em seu projeto solitário, conseguiu   criar   um   kernel   capaz   de   executar   os   utilitários   de programação e os comandos do Unix 

Reconhecendo  que  não  conseguiria  continuar  a  desenvolver  sozinho  o  Linux,  ele  enviou  pela internet a seguinte mensagem de desafio para uma lista de discussão:

================================================================================================================================ De:
torvalds@klaava.Helsinki.FI (Linus Benedict Torvalds) Lista de Discussão:
comp.os.minix
Assunto:
O que você gostaria que o Minix tivesse?
Resumo:
Pequena votação sobre o meu Sistema operacional.
Message-ID:
<1991Aug25.205708.9541@klaava.Helsinki.FI> Data:
25 Aug 1991 20:57:08 GMT Organização:
University of Helsinki 
Olá pessoal por aí usando minix – 
Estou fazendo um sistema operacional (gratuito) (apenas um hobby, não será grande e profissional como o gnu) para 386 (486) clones da AT. Isso vem crescendo desde abril, e está começando a ficar pronto. Eu gostaria de receber qualquer feedback sobre coisas que as pessoas gostam / não gostam no Minix, já que meu sistema operacional se parece um pouco (mesmo layout físico do sistema de arquivos (devido a razões práticas) entre outras coisas). No momento, tenho portado o bash (1.08) e o gcc (1.40), e as coisas parecem funcionar. Isso significa que vou conseguir algo prático em alguns meses e gostaria de saber quais recursos a maioria das pessoas desejaria. Todas as sugestões são bem-vindas, mas eu não prometo que vou implementá-las :-)
Linus (torvalds@kruuna.helsinki.fi) 
Obs: Sim, está livre de qualquer código minix e tem um fs multi-threaded. Não é portável (usa a alternância de tarefas do 386, etc), e provavelmente nunca irá suportar nada além de discos rígidos AT, já que é tudo que eu tenho :-(.
================================================================================================================================ 
Em 5 de outubro de 1991, Linus Torvalds lançou a primeira versão de seu sistema operacional:
Linux 0.02. A partir dessa data, muitos programadores no mundo inteiro têm colaborado e ajudado a fazer do Linux o sistema operacional que é atualmente. E foi assim que um cara lá nos cafundós gelados  da  Finlândia  criou  um  Sistema  Operacional  e  hoje  –  trinta  anos  depois  –  você  tem  que estudá-lo para passar em um concurso público :-) 
CENSURADO

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





9
102





Esse é o Tux: um pinguim gorducho que se tornou o mascote do Linux!

(DPE/MT – 2015) O sistema operacional é um conjunto de programas que interfaceia o hardware com o software. O componente desse sistema que gerencia todos os recursos computacionais é denominado:

a) memória.
b) kernel.
c) shell.
d) ROM.
e) DOS.
_______________________ Comentários: conforme vimos em aula, trata-se do kernel (Letra B).

(Banco da Amazônia – 2012) O Mac OS, desenvolvido com base no sistema operacional UNIX, foi substituído pelo OS X, que se baseia em novo paradigma, caracterizando-se pela  ausência  de  uma  linha  de  comando,  isto  é,  trata-se  de  um  sistema  operacional unicamente gráfico.
_______________________ Comentários: todos os sistemas operacionais possuem um shell de linha de comando – seja gráfico ou não (Errado).






Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





10
102




1.2 – CONCEITOS BÁSICOS 
Quando se liga um computador, o sistema operacional é acionado, possibilitando inicializar o hardware e gerenciá-lo, tornando possível sua utilização pelo usuário – ele é descarregado da memória quando o computador é desligado . O Linux – sistema operacional bastante difundido atualmente e adotado por grandes empresas – é multitarefa, multiusuário e multiprocessamento, além de possuir memória virtual por paginação, bibliotecas compartilhadas, etc.

Ao contrário de um software proprietário, ele é um software livre, cujo código-fonte está aberto e disponível  sob  a  Licença  GPL  (Genereal  Public  License)  para  que  o  usuário  possa  ter  acesso  ao código-fonte com o intuito de utilizá-lo executá-lo, estudá-lo, modificá-lo e distribuí-lo livremente de  acordo  com  os  termos  da  licença.
Ele é desenvolvido, em geral, por uma comunidade de programadores voluntários espalhados pelo mundo que contribuem para melhorá-lo.

Ele é um exemplo de sistema operacional livre amplamente difundido que pode ser utilizado tanto em  servidores  de  grandes  empresas  –  onde  ele  é  mais  frequente  –  quanto  em  computadores pessoais,  passando  por  diversas  arquiteturas  ou  plataformas  de  hardware  diferentes.
Existem
muitas questões que querem enganar o aluno dizendo que ele só funciona em servidores. MEN- TI-RA! Ele funciona tanto em servidores quanto em computadores pessoais.

Há muitas coisas que as pessoas acham que não podem ser feitas no Linux, tais como: permitir a conexão  de  pendrive,  acessar  a  internet  por  meio  do  Protocolo  TCP/IP,  realizar  backup,  instalar aplicativos de armazenamento em nuvem (Ex: Google Drive, Dropbox, etc)... tem gente que acha que Linux não tem nem interface gráfica com papel de parede, ícones, menus, etc.
Galera, Linux
tem tudo isso, tem internet, tem navegadores, arquivos, pastas, etc. Bacana?

Professor, é verdade que o Linux não é seguro? Não, esse é outro mito!
O Linux não é mais ou menos seguro que outros sistemas operacionais – como MS-Windows . Lembrem-se: todos os sistemas operacionais  são  vulneráveis  a  eventuais  softwares maliciosos. Beleza?  Dito  isso,  vamos  finalizar essa parte de conceitos básicos do nosso sistema operacional visualizando uma tabela com várias características do Linux. Vejam só:

CARACTERÍSTICAS DO LINUX É multitarefa, isto é, o sistema pode executar mais de uma aplicação ao mesmo tempo.

É multiusuário, isto é, um mesmo computador pode ter várias contas de usuário.

É preemptivo, isto é, permite a interrupção de processos.

Suporta nomes extensos de arquivos e pastas (255 caracteres).

Conectividade com outros tipos de plataformas como: Apple, Sun, Macintosh, Sparc, Unix, Windows, DOS, etc.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





11
102




Utiliza permissões de acesso à arquivos, pastas e programas em execução na memória RAM.

Proteção entre processos executados na memória RAM.

Modularização: ele só carrega para a memória o que é utilizado durante o processamento, liberando totalmente a memória, assim que o programa/dispositivo é finalizado.
Não  há  a  necessidade  de  se  reiniciar  o  sistema  após  modificar  a  configuração  de  qualquer  periférico  de computador ou parâmetros da rede – exceto em falhas de hardware.
Em geral, não necessita de um processador potente para funcionar.

Suporta diversos dispositivos e periféricos disponíveis no mercado, tanto os novos como os obsoletos.

Possui controles de permissão de acesso (Login e Logout).


(ANVISA – 2016) O sistema operacional Linux, embora seja amplamente difundido, está indisponível para utilização em computadores pessoais, estando o seu uso restrito aos computadores de grandes empresas.
_______________________ Comentários: conforme vimos em aula, ele está disponível – sim – para utilização em computadores pessoais (Errado).

(FUB – 2011) O Linux suporta o protocolo IP e possui navegadores web, o que permite acesso à Internet.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).

(Prefeitura de Natal/RN – 2015) O Linux é um sistema operacional:
I.   Considerado proprietário.
II.  Considerado software livre.
III. Misto, isto é meio proprietário, meio livre.

Assinale a alternativa correta:

a) Somente a afirmativa I está correta.
b) Somente a afirmativa II está correta.
c) Somente a afirmativa III está correta.
d) Todas as afirmativas estão incorretas.
e) Todas as afirmativas estão corretas.
_______________________ Comentários: (I) Errado, é um software livre; (II) Correto, é um software livre; (III) Errado, é um software livre (Letra B).


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





12
102




1.3 – INTERFACE GRÁFICA 
Vamos  falar  um  pouco  sobre  interface  de  usuário! O  que  é  isso,  professor?  Galera,  é  o  meio  de interação entre humanos e máquina. Todas as pessoas quando utilizam um computador estão se comunicando por meio de uma interface de usuário. Em geral, essas interfaces podem ser de dois tipos:
CLI (Command Line Interface)  e GUI (Graphic User Interface).  Basicamente,  a  primeira  é uma Interface de Linha de Comando e a segunda é a uma Interface Gráfica.

Quando a informática ainda engatinhava, os computadores funcionavam em uma interface de linha  de  comando  em  que  o  usuário  digitava  uma  série  de  instruções,  o  computador  as processava e retornava com as informações processadas para o usuário .  Os  comandos  eram simples,  diretos  e  precisos,  mas  apresentavam  um  inconveniente:  era  necessário  que  o  usuário soubesse todos esses comandos ou procurassem em um manual (geralmente em inglês).

Foi  aí  que  a  Apple  e  a  Microsoft  desenvolveram  uma interface  gráfica  que  –  aliada  ao  mouse  – eliminou as barreiras e a necessidade de usar comandos e preparou o mundo da informática para o que  é  hoje:  ícones,  janelas,  menus,  botões,  etc.
O  computador  se  tornava  mais  amigável  e convidativo, e eliminava-se a necessidade de aprender todos os comandos do computador – além de abrir portas para novos tipos de aplicativos .

Com  o  surgimento  da  interface  gráfica,  o  terminal  de  comandos  foi  ficando  cada  vez  mais escondido dos usuários, agindo de vez em quando nos bastidores ou pulando por alguns segundos numa instalação mais complexa ou outra. Apesar disso, o terminal ainda é uma ferramenta muito forte e presente em sistemas operacionais UNIX (Ex: Mac OS e Linux).
Isso causa um certo ar de desconfiança e desdém por quem utiliza Windows – especialmente a geração mais nova.

De todo modo, a Microsoft simplesmente esqueceu dele e apostou todas as suas cartas na Interface Gráfica.
Hoje  em  dia,  ambas  as  interfaces  coexistem  na  imensa  maioria  dos  sistemas operacionais. Bem... poucas pessoas sabem, mas as interfaces gráficas geralmente possuem um nome. Ah é, professor? Sim, a interface gráfica do Windows 7 se chamava Aero; do Windows 8 se chamava Metro; e atualmente a interface gráfica do Windows 10 se chama Fluent.

Só que – quando nós chegamos no Universo Linux – devemos lembrar que o código é livre para qualquer pessoa desenvolver recursos e funcionalidades. Diferentemente do Windows em que você  não  pode  escolher  qual  interface  utilizar,  o  Linux  permite  que  você  escolha  entre  diversas interfaces gráficas diferentes. Existe uma variedade imensa de interfaces gráficas – algumas mais leves que outras, outras são mais elegantes, outras são mais funcionais e assim por diante.

Dentre as opções de interface gráfica (também chamadas de Ambiente Gráfico ou Ambiente X), podemos  destacar:
Gnome, KDE, XFCE, Unity, LXDE, Mate, Cinnamon, OpenBox, BlackBox, Window Maker, etc, etc, etc . Calma, galera... nós não vamos ver em detalhes todas elas em nossa aula!  As  únicas  interfaces  gráficas  relevantes  para  provas  de  concurso  são  as  quatro  primeiras.
Então, vamos fazer alguns exercícios e depois vamos detalhá-las...
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





13
102





(MEC – 2009) São interfaces gráficas no ambiente Linux:

a) Gnome, BlackBox, Window Maker e Apache b) BlackBox, Window Maker, Apache e KDE c) KDE, Gnome, BlackBox e Window Maker d) Window Maker, Apache, KDE e Gnome e) Apache, KDE, Gnome e BlackBox _______________________ Comentários: conforme vimos em aula, trata-se do KDE, Gnome, BlackBox e Window Maker (Letra C).

(AGU – 2014) Sistemas Operacionais Linux são programas responsáveis por promover o funcionamento  do  computador,  realizando  a  comunicação  entre  os  dispositivos  de hardware e softwares. Em relação a este sistema, é correto afirmar que KDE e GNOME são:

a) versões de Kernel.
b) distribuições Linux.
c) ambientes gráficos.
d) editores de texto Linux.
e) terminais para execução de comandos.
_______________________ Comentários: conforme vimos em aula, trata-se de ambientes gráficos (Letra C).

(JUCEPAR/PR  –  2016)  Qual  das  expressões  abaixo  é  utilizada  para  se  referenciar  a interface gráfica do Linux?

a) Kernel.
b) Terminal.
c) Shell.
d) Console.
e) Ambiente X.
_______________________ Comentários: conforme vimos em aula, trata-se do Ambiente X (Letra E).





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





14
102




1.3.1 – GNOME


GNOME é um projeto de software livre abrangendo o ambiente gráfico para os usuários  e  os  desenvolvedores.   O   projeto   dá   ênfase   especial   a   usabilidade, acessibilidade e internacionalização. É um dos mais populares do mundo e não se limita apenas à interface, mas a diversas aplicações que compõem toda ela.

(AL/RR – 2010) Gnome é uma interface gráfica que facilita o uso do ambiente Linux e apresenta uma aparência semelhante à oferecida pelos sistemas Windows. Comparando Gnome com a interface gráfica do Windows, analise as afirmativas a seguir e marque a alternativa CORRETA.

I - O Gnome tem uma área de trabalho;  II - O Gnome permite utilizar o botão direito do mouse; III - O Gnome permite criar pastas;  IV - O Gnome permite as operações de copiar e colar;  V - Quando houver uma leitora de CD disponível, o Gnome permitirá ver arquivos que se encontram em um CD.

a) Somente a afirmativa III está correta.
b) Somente a afirmativa IV está correta.
c) Somente as afirmativas I, III, IV e V estão corretas.
d) Somente as afirmativas I, II, III e V estão corretas.
e) Todas as afirmativas estão corretas.
_______________________ Comentários: (I) Correto, ele tem uma área de trabalho; (II) Correto, ele permite utilizar o botão direito do mouse; (III) Correto, ele permite criar pastas; (IV) Correto, ele permite as operações de copiar e colar; (V) Correto, ele permite ver arquivos que se encontram em um CD (Letra E).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





15
102




1.3.2 – KDE



KDE é um ambiente gráfico multiplataforma mais similar ao Windows, portanto é o mais comum quando se migra do  Windows para o Linux .  Ele  é  altamente configurável e flexível.


(DEGASE – 2012) Nas distribuições Linux, uma interface gráfica representa o principal gerenciador   de   pastas   e   arquivos,   utilizado   para   cópia,   exclusão,   organização, movimentação  e  atividades  relacionadas  a  arquivos  e  instalação  de  programas.  É  um recurso  que  permite  a  visualização  de  imagens,  vídeos,  animações  e  a  interação  com essas   características   através   de   mouse,  teclado   e   outros.   Sem   ser   um   sistema operacional,  um  dos  principais  exemplos  dessa  interface  gráfica  no  Linux é  conhecida por:

a) KDE
b) SUSE
c) UBUNTU
d) CHROME
e) SOLARIS
_______________________ Comentários: conforme vimos em aula, trata-se do KDE (Letra A).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





16
102




1.3.3 – XFCE


Trata-se de um ambiente gráfico que pretende ser rápido e  leve, enquanto ainda é visualmente atraente e fácil de usar – além de incorporar a filosofia UNIX de modularidade e reutilização .


(UFLA – 2010) As distribuições Linux, incluindo Fedora e Ubuntu, suportam os seguintes Ambientes de Trabalho (Desktop Enviroment):

a) Konqueror, GNOME e KDE.
b) GNOME, KDE e XFCE.
c) Nautilus, Slackware e KDE.
d) Dolphin, Explorer e KFCE.
_______________________ Comentários: conforme vimos em aula, trata-se do GNOME, KDE e XFCE (Letra B).







Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





17
102




1.3.4 – Unity



Unity é uma interface para o ambiente desktop. Ela foi desenhada inicialmente para fazer um uso mais eficiente do espaço das telas limitadas dos netbooks ,  porém
devido ao sucesso tornou-se a interface padrão do Ubuntu.


(SEDUC/PI – 2014) No sistema operacional Linux é possível executar diversos ambientes gráficos que fornecem os recursos necessários para uma interface (Área de Trabalho) do usuário. Marque a alternativa que NÃO é um ambiente gráfico do Linux.

a) Gnome
b) KDE
c) XFCE
d) iOs
e) Unity
_______________________ Comentários: iOS é um sistema operacional para dispositivos móveis da Apple. Unity é – sim – um ambiente gráfico do Linux (Letra D).




Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





18
102




1.4 – ROTINAS DE INICIALIZAÇÃO 
Algumas pessoas ficam até interessadas em experimentar o Linux, mas pensam que – para isso – elas devem se desfazer do Windows. Galera, isso não é necessário! Como assim, professor?
Você
pode  ter  diversos  sistemas  operacionais  em  seu  computador.  Claro  que  você  não  troca  de sistema operacional com um simples atalho de teclado – lembrem-se que o sistema operacional é um software grande e pesado que ocupa grande parte da memória do seu computador.

Então, como é feito? Pessoal, vocês já sabem que um disco rígido (Hard Disk – HD) é aquele disco que  armazena  dados  em  seu  computador  mesmo  após  você  desligá-lo  da  tomada.
Esse disco é
dividido em milhões de setores, que são pequenas áreas para armazenamento de dados . Todo
disco rígido possui um setor específico chamado setor de inicialização, também conhecido como Master Boot Record (MBR) – Registro Mestre de Inicialização.

Esse  setor  armazena  um  código  executável  que  funciona  como  um  carregador  do  sistema operacional instalado . Como é, professor? Voltemos para o exemplo dos carros: como você faz para ligar o motor bem potente e pesado de um carro em segundos? Você insere a chave e inicia o sistema de ignição do carro. Esse sistema é responsável por fazer com que aquele motor pesado, potente e frio saia da inércia e, em segundos, esteja funcionando a todo vapor.

A  MBR  armazena  um  software  (código  executável)  semelhante  ao sistema   de   ignição!
Dessa  forma,  toda  vez  que  você  liga  um computador,  a  primeira  coisa  carregada  na  memória  é  esse  código executável  capaz  de  inicializar  o  sistema  operacional  desejado .
Agooooora  vem  o  pulo  do  gato:  se  você  possui  mais  de  um  sistema operacional instalado em seu computador, um software exibirá em tela uma  lista  de  sistemas  operacionais  para  que  você  possa  escolher  qual você deseja inicializar. Computação é lindo demais, gente...

Galera,  esse  procedimento  é  chamado  de  Dual  Boot,  porque  na  maioria  dos  casos  possui  duas opções  de  sistemas  operacionais.  Bem,  já  vou  adiantando  para  vocês  que  esses  softwares gerenciadores  de  inicialização  –  conhecidos  como BootLoader  –  não  são  bonitinhos:
eles  são
acessados por meio de uma interface de linha de comando . Nós veremos a seguir um pouquinho sobre os principais softwares de inicialização do Universo Linux: LILO e GRUB!

(BANESTES – 2012) Nos computadores de hoje, facilmente pode-se ter dois sistemas operacionais  instalados,  sendo  que  a  inicialização apresenta  a  opção  de  escolher  o Sistema Operacional para iniciar a máquina.  Esse processo denomina-se Dual Boot. O Linux utiliza um gerenciador de inicialização, o que facilita ter máquina em Dual Boot.
Identifique os gerenciadores de inicialização mais utilizados no mundo Linux.

a) LILO e GRUB.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





19
102




b) MBR e LILO.
c) GRUB e MBR.
d) BIOS e GRUB
e) LILO e BIOS.
_______________________ Comentários: conforme vimos em aula, trata-se do LILO e GRUB (Letra A).

(TJ/AC  –  2012)  Considere  que  dois  servidores  públicos  que  trabalham  em  horários diferentes  usem  o  mesmo  computador,  no  qual  está  instalado  o  sistema  operacional Linux. Considere, ainda, que tenha sido designado a um desses servidores que passe a utilizar   o   sistema   operacional   Windows.   Nessa   situação,   é   necessário   que   seja disponibilizado  outro  computador,  visto  que  um  computador  suporta  a  instalação  de apenas um sistema operacional.
_______________________ Comentários: conforme vimos em aula, isso não é necessário – basta utilizar algum Gerenciador de Inicialização (Errado).

(Polícia Federal – 2014) As rotinas de inicialização GRUB e LILO, utilizadas em diversas distribuições Linux, podem ser acessadas por uma interface de linha de comando.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).

(UFBA – 2014) Quando se pensa em sistemas operacionais, é possível instalar mais de um sistema operacional em uma máquina, por exemplo, o Ubuntu junto com o Windows 7 ou 8. Para que isso ocorra é necessário particionar o disco e realizar duas instalações.
Quando esse procedimento funciona, temos uma máquina com:

a) boot remoto.
b) boot por CD/DVD.
c) dual boot.
d) trial boot.
e) boot normal.
_______________________ Comentários: conforme vimos em aula, trata-se do Dual Boot (Letra C).







Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





20
102




1.4.1 – LILO



O LILO (LInux LOader)  é  o  gerenciador  de  inicialização  mais  antigo  –  vejam  que  ele  tem  uma interface mais simples e rústica. Era o carregador de boot mais popular para Linux até 2001, quando o Bootloader GRUB começou a substituí-lo. Existem muito mais coisas a se falar sobre ele, mas não cai em concurso público, logo isso é mais do que suficiente para vocês :-) 
(FAPEC – Prefeitura de Água Branca/AL – Agente Administrativo) O gerenciador de boot mais tradicionalmente utilizado no Linux é o:

a) LILO
b) MRV
c) MBR
d) KERNEL
_______________________ Comentários: conforme vimos em aula, trata-se do LILO (Letra A).

(PC/ES – 2013) O carregamento (boot) do sistema operacional Linux pode ser gerenciado pelo programa LILO.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).






Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





21
102




1.4.2 – GRUB



O GRUB (GRand Unified Bootloader) é um gerenciador de inicialização mais recente – notem como ele é mais bonito e moderno que o anterior. Ele é mais poderoso que o LILO e suporta um número ilimitado de entradas de sistemas operacionais, além de permitir sistemas de arquivo maiores. Isso também é suficiente para provas de concurso :-) 
(PGM/RR – 2010) No Linux, por padrão, o aplicativo Grub é usado para enviar um correio eletrônico para destinatário na Internet.
_______________________ Comentários: olha que viagem essa questão! Bastava ter lido nossa aula para saber que não faz o menor sentido (Errado).













Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





22
102




1.5 – TIPO DE USUÁRIO 
Um  usuário  é  alguém  que  possui  uma  identificação  no  sistema.  Essas  informações  permitem  ao Linux controlar como o acesso é garantido aos usuários e o que eles podem fazer depois de obter a permissão de acesso. Vamos conhecer os três tipos de usuário do Linux:

1.5.1 – Usuário Comum 
São aqueles que possuem contas para utilização do sistema operacional. Basicamente,  esses usuários  possuem  um  diretório  base (/home/username,  exemplo)  e  podem  criar  e  manipular arquivos  em  seu  diretório,  além  de  executar  tarefas  simples  como  criar  e  editar  documentos, navegar na internet, ouvir música etc. Ao contrário do usuário administrador, o usuário comum é inviabilizado para realização de algumas tarefas a nível de sistema. Em geral, vem com um símbolo de cifrão ($) na linha de comando.

1.5.2 – Usuário Administrador (Root) 
Também chamado de Root, é responsável por controlar todo o sistema e não possui quaisquer tipos de restrições.  Sempre  que  executado  algum  software  ou  atividade que  precise  de  acesso administrativo,  é  necessário  o  root,  que  é  chamado por  meio  do  comando sudo.  Por  exemplo:
sempre  que  for  instalar  um  programa  ou  realizar  um upgrade  de  todo  o  sistema  operacional,  é utilizado o comando sudo para se ter as permissões de root e conseguir efetuar essas tarefas. Em geral, vem com um símbolo de cerquilha (#) na linha de comando.

1.5.3 – Usuário de Sistema 
Usuários  que  não  necessitam  estar  logados  no  sistema  para  controlar  alguns  serviços.  Estes comumente não possuem senhas e, diferentemente dos usuários comuns, não se conectam. São contas usadas para propósitos específicos do sistema e não são de propriedade de uma pessoa em  particular.  Um  exemplo  desse  tipo  de  usuário  é  o  www-data,  que  pode  ser  utilizado  para controlar servidores web como Apache e Nginx.

(Prefeitura de Canavieira/PI – 2015 – Letra A) ROOT é o nome do super usuário.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





23
102




(DETRAN/CE – 2014 – Item IV) O usuário root tem acesso restrito a arquivos e processos do sistema operacional.
_______________________ Comentários: conforme vimos em aula, o usuário root tem acesso irrestrito ao sistema operacional (Errado).

Todos os usuários conseguem listar os conteúdos dos diretórios, mas somente o Usuário Root pode criar arquivos e/ou pastas em um diretório diferente de seu diretório pessoal. Isso quer dizer que, se eu quiser logar no sistema como um usuário comum, somente poderei criar arquivos e/ou pastas em  meu  diretório  pessoal,  ou  seja,  o  diretório /home/<usuário>. Dito  isso,  vamos  ver  alguns exemplos: eu – como usuário comum – tentando criar uma pasta em outro diretório.



Vejam que a permissão foi negada! Agora notem o que ocorre quando tentamos criar a pasta como administrador (root) usando o comando sudo:



O terminal de linha de comando vai solicitar a sua senha pessoal e, depois que você digitá-la, ele  vai  executar  o  comando  solicitado.  Nesse  momento,  você  pode  pensar: Ué,  professor!  Se qualquer usuário que digite o comando sudo poderá executar os comandos avançados, do que adianta?
Bom saber que vocês estão atentos à aula! Belíssima pergunta...

Na  realidade,  o  que  ocorre  é  que  o  usuário  que  instalou  o  sistema  operacional  na  máquina  tem direitos  de  executar  comandos  como  administrador,  porque  –  em  tese  –  ele  é  responsável  pela máquina, ele que instalou tudo, etc. Por essa razão, ele pode executar comandos como o sudo.
Se
você posteriormente pensar em criar um novo usuário no computador, você notará que ele não conseguirá executar comandos com o sudo . Entendido, pessoal? Bom demais...




Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





24
102




2 – DISTRIBUIÇÕES LINUX 


Galera,  o  Linux  não  é  como  o  Windows! Como  assim,  professor?  Cara,  a  Microsoft  combina internamente todos os bits do Windows para produzir cada nova versão do Windows e o distribui como  um  único  pacote.  Se  você  quiser  o  Windows,  precisará  escolher  uma  das  versões  que  a Microsoft oferece.
O Linux funciona de maneira diferente: ele não é produzido por uma única organização. Diferentes organizações e pessoas trabalham em diferentes partes.

Nós  temos  o  Kernel  (núcleo  do  Sistema  Operacional),  os  Utilitários  de  Shell  (interpretador  de comandos), o Servidor X (que produz um desktop gráfico), o Ambiente de Desktop (que roda no Servidor X para fornecer uma área de trabalho gráfica), etc. Galera, serviços do sistema, programas gráficos, comandos do terminal - muitos deles são desenvolvidos de forma independente um do outro e são todos softwares de código aberto .

Se você quisesse, poderia pegar o código-fonte do kernel do Linux, os Utilitários de Shell, o Servidor X e todos os outros programas em um Sistema Operacional Linux – montando tudo sozinho.
No
entanto, compilar o software levaria muito tempo - sem mencionar o trabalho envolvido em fazer com que todos os diferentes programas funcionassem corretamente juntos .

Uma Distribuição Linux faz o trabalho pesado para você! Ela pega todo o código dos projetos de código  aberto,  compilando-o  e  combinando-o  em  um  único  sistema  operacional  que  você  pode instalar e inicializar. Eles também fazem escolhas para você, como escolher o ambiente de desktop padrão, o navegador, etc. A maioria das distribuições adiciona seus próprios toques finais para gerar uma identidade de cada distribuição.

Portanto, o que é uma distribuição?
Trata-se de um sistema operacional criado a partir de uma coleção de software construído sobre o Kernel do Linux. Cada distribuição possui recursos que a tornam única. Algumas distribuições são projetadas para uso geral, enquanto outras são projetadas para  um  caso  de  uso  muito  específico,  como  um  firewall  ou  um  servidor  da  Web.  A  escolha  da distribuição que funciona melhor para você pode levar algum tempo.

As  distribuições  podem  ser  comerciais,  isto  é,  o  usuário  paga  pelo  sistema  e  recebe  um  suporte técnico; ou podem ser livres, isto é, não há cobrança pelo uso, qualquer um pode fazer o download, estudar,  executar,  modificar,  distribuir,  entre  outros.
Claro,  você  não  terá  suporte  técnico Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





25
102




gratuito, no entanto existe uma comunidade gigantesca no mundo para ajudá-lo, caso você necessite. Bacana, não é?


As  principais  distribuições  atualmente  são:
Debian, Ubuntu, RedHat, Fedora, Suse, Mint, CentOS, Mandrake, Slackware, etc. Galera, existem –  inclusive  –  distribuições  brasileiras.  As  mais  famosas  são  a  Kurumin, Conectiva, Kalango e Mandriva.

(COBRA/BB  –  2014)  Na  realização  de  um  determinado  suporte técnico, é requerida a reinstalação do sistema operacional. Para tanto,há necessidade de se  reinstalar  um  sistema  operacional  proprietário. Assinale,  a  seguir,  um  sistema operacional desse tipo.

a) Debian 7.1.
b) Windows 7.
c) Ubuntu 12.
d) FreeBSD.
e) CentOS.
_______________________ Comentários: conforme vimos em aula, trata-se do Windows 7 (Letra B).

(SEPLAG/DF – 2009) Uma alternativa ao sistema operacional Windows, de propriedade da Microsoft, são os sistemas operacionais livres, como o Linux. Existem, porém, várias distribuições  desse  sistema.  Assinale  a  alternativa  que  possui  apenas  nomes  de distribuições do Linux.

a) FreeBSD, Slackware, DOS.
b) Mandrake, Ubuntu, Suse.
c) OS/2, AIX, Solaris.
d) HP-UX, Digix, Mumps68K.
e) Mac-OS, QDOS, OpenBSD.
_______________________ Comentários: conforme vimos em aula, trata-se do Mandrake, Ubuntu, Suse (Letra B).

(SEGESP/AL – 2013) Diferentemente do Linux, o Windows permite que o usuário crie sua  própria  versão  de  sistema  operacional  mediante a  alteração  do  código-fonte  do programa.
_______________________ Comentários: conforme vimos em aula, a questão inverteu Linux e Windows (Errado).
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





26
102




2.1 – UBUNTU



O Ubuntu é, sem dúvida nenhuma, a distribuição mais popular no mundo devido ao fato de ser uma  das  mais  amigáveis  e  fáceis  de  instalar,  utilizar  e  de  se  obter  ajuda  para  resolver problemas
. Ela se preocupa muito com o usuário final de computadores desktop. Originalmente baseada no Debian, diferencia-se além do foco no desktop, em sua forma de publicação de novas versões, que são lançadas semestralmente.

(TRE/AC – 2015) Os softwares são essenciais para a interação homem/máquina. Existem softwares  que  são  proprietários  e  outros  que  são  livres.  Segundo  a  Fundação  para  o Software  Livre,  é  considerado  livre  qualquer  programa  que  pode  ser  copiado,  usado, modificado  e  redistribuído  de  acordo  com  as  necessidades  do  usuário.  Dessa  forma, assinale a alternativa que apresenta um exemplo de software livre.

a) iOS.
b) Windows Server.
c) Ubuntu Linux.
d) MS-Offíce.
e) Windows 7.
_______________________ Comentários: conforme vimos em aula, trata-se do Ubuntu Linux (Letra C).

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





27
102




2.2 – DEBIAN



Trata-se de uma distribuição baseada Projeto GNU conhecida por ser a distribuição mais estável e segura  do  Linux.  No  Debian,  cada  pacote  para  por  inúmeros  testes  até  ser  considerado  estável.
Algumas  pessoas  que  estão  começando  a  usar  podem  considerar  Debian  uma  distribuição complexa  demais  para  iniciantes. Ela  serviu  de  base  para  a  criação  de  diversas  outras distribuições populares, tais como Ubuntu e Kurumin .

(DPU – 2010 – Letra B)  Debian  é  uma  das  distribuições  do  Linux  mais  utilizadas  no mundo;  no  entanto,  sua  interface  não  suporta  a  língua  portuguesa,  sendo  necessário conhecimento de inglês para acesso.
_______________________ Comentários: na verdade, ele suporta a língua portuguesa – há tradução para nossa língua (Errado).








Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





28
102




2.3 – FEDORA



Fedora é uma das mais populares e estáveis distribuições que existem atualmente. Ele era, no começo,  uma  bifurcação  para  a  comunidade,  liberado e  mantido  pela  gigante  RedHat  que,  na época, estava fechando seu sistema e concentrando-se no mercado corporativo. Isso significa que, desde o princípio, o Fedora já contava com o que há de mais moderno em tecnologia de software, assim  como  também  contava  com  uma  das  mais  competentes  e  dedicadas  equipes  em  seu desenvolvimento.

Se  o  que  você  procura  é  uma  distribuição  com  poderes  de  ser  um  servidor  estável,  mas  com  as facilidades das ferramentas de configuração gráficas, ou se, simplesmente, deseja um desktop mais robusto, o Fedora será a sua melhor escolha. Enfim, apesar de não ser tão fácil de usar quanto as distribuições Ubuntu e Mint, é uma distribuição relativamente fácil de usar, mas os iniciantes podem ter um pouco de dificuldade.

(SEJUS/ES  –  2009)  Por  meio  do  processo  de  escolha  de  pacotes,  o  usuário  pode selecionar software que já estão pré-compilados para o funcionamento com o Fedora 10.
_______________________ Comentários: atualmente, a maioria  das  distribuições vem com uma  gama  de  softwares  de  grande utilidade em  seu  próprio disco de instalação, em que o usuário poderá escolher quais pacotes deseja instalar (Correto).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





29
102




2.4 – SUSE



O SUSE é uma das distribuições Linux mais antigas e, assim como o RedHat, sua história está mesclada  com  os  primeiros  passos  no  Linux  no  mundo empresarial.  O  openSUSE,  a  versão comunitária  do  SUSE  Enterprise  Linux,  numa  relação semelhante  ao  que  o  Red  Hat  tem  com  o CentOS, porém ainda mais unificado entre os projetos, que são basicamente o mesmo sistema. O openSUSE pode ser utilizado tanto como Desktop, como em servidores.

(CLIN – 2015) São exemplos de distribuições Linux:

a) Squid e Kerberos.
b) Lilo e Grub.
c) Suse e Red Hat.
d) KDE e Gnome.
_______________________ Comentários: conforme vimos em aula, trata-se do Suse e RedHat (Letra C).




Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





30
102




2.5 – MINT



O  Linux  Mint  é  uma  das  distribuições  Linux  preferidas  dos  usuários  iniciantes  no  Linux  e também é considerada uma das distribuições mais fáceis de usar . Ela é uma distribuição baseada no Ubuntu com o qual é totalmente compatível e partilha os mesmos repositórios. Diferencia-se do Ubuntu  por  incluir  drivers  e  codificadores  proprietários  por  padrão  e  por  alguns  recursos  que permitem fazer em modo gráfico configurações que no Ubuntu são feitas de modo texto.
















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





31
102




2.6 – CENTOS



CentOS  é  uma  distribuição  de  classe  Enterprise  derivada  de  códigos  fonte  gratuitamente distribuídos pela RedHat Enterprise Linux e mantida pelo CentOS Project. CentOS proporciona um grande acesso aos softwares padrão da indústria, incluindo total compatibilidade com os pacotes de softwares preparados especificamente para os sistemas da RHEL.
Isso lhe dá o mesmo nível de segurança e suporte, através de updates, que outras soluções enterprise, porém sem custo .

(TJ/RS – 2018) O CentOS (Community Enterprise Operating System) é uma distribuição Linux  de  classe  Enterprise,  derivada  de  códigos-fonte,  gratuitamente  fornecidos  pela distribuição:

a) Gentoo.  b) Kurumin.        c) Red Hat.  d) Slackware.  e) Ubuntu.
_______________________ Comentários: conforme vimos em aula, trata-se RedHat (Letra C).



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





32
102




2.7 – MANDRIVA



Mandriva é uma das maiores distribuições da atualidade, nasceu da fusão entre o antigo Mandrake e a brasileira Conectiva. A Empresa Francesa Mandriva se dedica à distribuição e suporte do sistema operacional Mandriva, tem sua sede administrativa em Paris e um centro de desenvolvimento em Curitiba, no Brasil.
O Mandriva conta também com um grande número de contribuidores pelo mundo, o público-alvo do Mandriva Linux engloba usuários iniciantes no mundo Linux assim como usuários com mais experiência.


(Banco  da  Amazônia  –  2010)  O  Linux,  um  sistema  multitarefa  e  multiusuário,  é disponível em várias distribuições, entre as quais, Debian, Ubuntu, Mandriva e Fedora.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).







Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





33
102




2.8 – SLACKWARE



Slackware, junto com Debian e RedHat, é uma das distribuições que deram origem a todas as outras
. Embora seja considerada por muitos uma distribuição difícil de se usar, voltada para usuário expert  ou  hacker,  possui  um  sistema  de  gerenciamento  de  pacotes  simples,  assim  como  sua interface de instalação, que é uma das poucas que continua em modo-texto, mas nem por isso se faz complicada.















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





34
102




2.9 – KURUMIN



Chegamos  agora  a  mais  famosa  distribuição  brasileira  (Brasil...  sil...  sil).  O  Kurumin  foi  uma distribuição desenvolvida pela equipe do Guia do Hardware e colaboradores, com o objetivo de ser um sistema fácil de usar, voltado especialmente para iniciantes e ex-usuários do Windows. Todos os componentes e scripts usados são abertos, o que possibilitou também o surgimento de versões modificadas do sistema .

Apesar de ter feito um grande sucesso e ter sido durante algum tempo uma das distribuições mais usadas no país, o projeto acabou falhando em atrair um grupo de desenvolvedores interessados em participar de forma ativa do desenvolvimento. Este e outros fatores acabaram fazendo com que o projeto  fosse  descontinuado  em  janeiro  de  2008. Galera, tenham orgulho... nós tivemos uma distribuição até relativamente famosa no mundo.





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





35
102




3 – GERENCIAMENTO DE SISTEMAS DE ARQUIVOS 3.1 – SISTEMAS DE ARQUIVOS 


Todo sistema operacional necessita de uma estrutura que possa dar suporte a ele para acessar e ler informações  contidas  no  disco  rígido.  O  recurso  que  constrói  uma  base  lógica  estrutural  para  o sistema  operacional  é  o  sistema  de  arquivos. Como assim, professor? Um sistema de arquivos é uma espécie de gerenciador e organizador que permitirá ao sistema operacional ler os arquivos que estão no disco rígido – esta é a finalidade básica de um sistema de arquivos .

Imagine a seguinte situação:
digamos que você necessite de um determinado documento que está armazenado em um depósito com milhões de outros documentos, mas você não pode pegá-lo diretamente – você deve fazê-lo por meio de um atendente. Dessa forma, você recorre ao atendente e este lhe mostra exatamente onde está o documento que você deseja dentro dessa estrutura lógica de organização dos arquivos. O sistema de arquivos é como esse atendente! :) 
O Sistema de Arquivos permite gravar, ler, localizar, remover e realizar funções em um dispositivo de armazenamento – em geral, um disco rígido. Galera, a maioria dos usuários Unix/Linux já foram ou ainda são usuários Windows. Nesse sistema operacional, existem basicamente três sistemas de arquivos: FAT16, FAT32 e NTFS.  No Linux, existem muito mais opções, tais como: EXT2, EXT3, EXT4, RaiserFS, etc. Vamos vê-los a seguir...

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





36
102




3.1.1 – EXT2

Um dos primeiros sistemas de arquivos utilizado nas primeiras versões do Linux foi o EXT2 (Second Extended FileSystem) – embora ele tenha sido uma espécie de padrão não era muito eficiente.

3.1.2 – EXT3

Trata-se  de  uma  versão  do  EXT2,  porém  com  suporte  a journaling 1
.  Essa  característica  foi  uma evolução e tornou o EXT3 um sistema de arquivos muito estável e robusto.

3.1.3 – EXT4

Este é uma espécie de versão do EXT3 que surgiu com a prerrogativa de melhorar o desempenho de compatibilidade, formatos e limites de armazenamentos.

3.1.4 – ReiserFS

Criado recentemente e suportado por quase todas as distribuições, apresenta ótima performance, principalmente para um número muito grande de arquivos pequenos.

O nome desse último sistema de arquivos vem do nome de seu criador: Hans Reiser
! Uma curiosidade meio macabra é que ele foi condenado a 25 anos de prisão por  assassinar  a  própria  esposa  em  2004  –  há  um  documentário  bastante interessante sobre a vida dele no Youtube! Fica a recomendação...

PRINCIPAIS CARACTERÍSTICAS 
No MS-DOS, os dispositivos de armazenamento como drives, HDs e CD-ROMs são representados por letras, por  exemplo:  A:,  B:,  C:,  D:.  No  Linux,  eles  são  representados  por  diretórios  cuja  posição  na  hierarquia  de diretórios é definida no momento de montagem, por exemplo: /mnt/floppy, /mnt/CD-ROM.


No MS-DOS, os nomes de arquivos estão no formato chamado 8.3, por exemplo: ARQUIVO1.TXT. No Linux, podemos   utilizar   nomes   de   arquivos   com   até   255   caracteres   e   mais   de   um   ponto,   por   exemplo:
Programa1.src.tar.gz.

1
Característica que dá permissão ao sistema operacional de manter um log (journal) de todas as mudanças no sistema de arquivos antes de escrever os dados no disco e assim permitindo recuperar o disco após um desastre em uma velocidade maior.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





37
102






O  Linux,  como  qualquer  sistema  operacional  Unix,  diferencia  letras  maiúsculas  de  minúsculas,  portanto, relatório, RELATÓRIO e Relatório são arquivos diferentes.


É possível inserir espaços no meio do nome dos arquivos.


Não  há  extensões  compulsórias  como  .COM  e  .EXE  para  programas,  .BAT  para  arquivos  de  lote,  .BAK  para backup ou outras.


(Prefeitura de Palhoça/SC – 2014)  Os  sistemas  de  arquivos  default  (por  padrão)  dos sistemas operacionais Windows 7 e Linux Ubuntu são, respectivamente:

a) NTFS e EXT4.
b) NTFS e NTFS.
c) EXT3 e EXT3.
d) NTFS e EXT3.
e) EXT4 e NTFS.
_______________________ Comentários: conforme vimos em aula, trata-se do NTFS e EXT4 (Letra A).

(EBC – 2011) O Windows 7 Professional grava os arquivos em formato nativo ext3 e fat32;
o Linux utiliza, por padrão, o formato NTFS, mais seguro que o adotado pelo Windows.
_______________________ Comentários: conforme vimos em aula, EXT3 é um sistema de arquivos do Linux e NTFS é um sistema de arquivos do Windows (Errado).

TJ/AC – 2012) No Linux, os nomes de arquivos podem ter até 256 caracteres, porém o nome de arquivo Um_nome_arquivo_longo+uma_longa_exntensão é inválido, pois o sinal + é um caractere reservado e não pode ser usado.
_______________________ Comentários: conforme vimos em aula, podem ter até 255 caracteres (Errado).




3.2 – ESTRUTURA DE DIRETÓRIOS 
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





38
102




O Linux organiza seus diretórios em uma estrutura hierárquica conhecida como árvore de diretórios que segue o Padrão FHS (Filesystem Hierarchy Standard). Como assim, professor? É mais ou menos assim: arquivos relacionados a dispositivos de hardware ficam situados no diretório dev; arquivos
relacionados  a  bibliotecas  essenciais  ficam  situados  no  diretório lib;  arquivos  relacionados  a arquivos de configuração se situam no diretório etc.

Galera, é claro que cada diretório possui outros subdiretórios, mas vocês não precisam conhecê-los para prova. Basicamente vocês precisam conhecer apenas os subdiretórios do diretório raiz “/” que estão apresentados abaixo! Como assim diretório raiz, professor? Galera, eu falei que é uma estrutura de  árvore  e,  em  uma  árvore,  tudo  tem  origem  na  raiz.
Aqui  é  a  mesma  coisa:  todos  os subdiretórios têm origem no diretório raiz. Então vejam só...



DIRETÓRIO DESCRIÇÃO
/

Trata-se do diretório raiz do Linux. É aqui que encontrará todos os diretórios e todos os dados que se encontram em seu sistema. Até mesmo um CD/DVD, disco externo ou qualquer outro periférico se encontram dentro da raiz do sistema. Na linha de comandos, você navega para o root digitando cd /.

/bin

Padrão FHS
/binProgramas utilizados com frequência /bootArquivos utilizados durante a inicializaçãodo sistema /devDispositivos de hardware /etcArquivos de configuração do sistema e dos programas /homePasta para os diretórios dos usuários /libBibliotecas essenciais e módulos Linux /sbinProgramas essenciais para o funcionamento do sistema /rootDiretório pessoal do usuário root /optSoftwares adicionados de maneira não padrão /procInformações sobre os processos sendo executados /mediaPontos de montagem de mídias removíveis /mntConexão de volumes de rede e dispositivos removíveis /tmpArquivos temporários do sistema /usrArquivos acessados pelo usuário /varInformações variáveis do sistema /srvDados dos serviços do sistema Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





39
102




O /bin é o diretório onde ficam guardados arquivos binários que têm de estar acessíveis a todos os utilizadores do sistema. Estes arquivos binários são programas que o próprio sistema inicia de forma autónoma.

/dev

Trata-se  do  diretório  onde  ficam  arquivos  especiais  associados  aos  dispositivos  do  sistema.
Estes ficheiros são especiais porque representam os dispositivos do sistema. Por exemplo: um disco rígido do sistema aparecerá como /dev/sda.

/etc

Trata-se do diretório onde se encontram todos os arquivos globais de configuração do sistema.
Na sua grande maioria, estes arquivos podem ser editados com o uso de um simples editor de texto. Repare que neste diretório encontram-se arquivos de configuração do sistema e, não, de um usuário específico. Os arquivos de configuração de um usuário específico encontram-se no diretório home de cada utilizador.

/home

Trata-se  do  diretório  onde  encontramos  um  arquivo para  cada  usuário  existente  no  sistema.
Sempre que adicionamos um novo usuário, por exemplo, com o nome profdiego2 no diretório /home, é criado um arquivo para este usuário como /home/profdiego2/. Dentro desse diretório, ficam todos os arquivos de configurações específicas para aquele usuário, bem como todos os seus arquivos de dados.

/lib

Trata-se do diretório onde estão armazenadas as bibliotecas compartilhadas no sistema. Estas bibliotecas  podem  variar  de  acordo  com  a  distribuição  utilizada  e  podem  ser,  por  exemplo, bibliotecas  de  linguagens  como  Perl,  Python,  C,  etc.  É  também  neste  diretório  que  estão  os módulos do Kernel do Sistema Operacional.

/mnt

Trata-se  do  diretório  em  que  os  administradores  de sistema  montam  sistemas  de  arquivos temporários  enquanto  os  utilizam.  Por  exemplo:  se  você  estiver  montando  uma  partição  do Windows para executar algumas operações de recuperação de arquivos, você pode montá-lo em  /mnt/windows.  No  entanto,  você  pode  montar  outros  sistemas  de  arquivos  em  qualquer lugar no sistema.

/proc

Trata-se  do  diretório  onde  se  encontram  arquivos  especiais  associados  aos  processos  do sistema. Estes arquivos são especiais porque representam os processos em funcionamento no sistema. Por exemplo: haverá um arquivo que fornece informação sobre o funcionamento do processador ou sobre outras operações que ocorram no sistema.

/root

Trata-se  do  diretório  do  superusuário  do  sistema.  Este  diretório  não  é  a  mesma  coisa  que  o diretório  raiz  do  sistema  –  de  onde  descendem  todos  os  restantes  diretórios.  Trata-se,  na verdade, de um diretório dedicado ao superusuário root.

/sbin

Trata-se do diretório destinado aos arquivos binários que são utilizados pelo superusuário root e para administração do sistema. Pode-se dizer que este diretório é semelhante ao /bin, mas Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





40
102




com a peculiaridade de serem programas que normalmente não serão utilizados por usuários com  permissões  limitadas.  Este  diretório  pode  não  existir  em  um  sistema  e  pode  também substituir o diretório /bin.

/tmp

Trata-se do diretório onde encontramos os arquivos temporários do sistema. Estes arquivos são normalmente gerados pelo sistema e, como o nome indica, permanecem no sistema durante um período limitado de tempo. Por exemplo: sempre que instalamos um programa, este utiliza o diretório /tmp/ para colocar arquivos que serão necessários durante a instalação, mas que não voltarão a ser necessários.

/usr

Trata-se do diretório onde estão arquivos e programas utilizados pelos usuários existentes no sistema.  No  caso dos  programas,  no  diretório /usr/bin  ficam  todas as aplicações  que  não  são essenciais ao sistema e, por conseguinte, não se encontram no diretório /sbin ou /bin . No caso dos programas que ficam no diretório /usr/bin, as bibliotecas associadas a estes sistemas ficam localizadas no diretório /usr/lib.

/var

Trata-se do diretório onde ficam diversos arquivos de dados vindos das contas de usuários. É neste diretório que são colocadas bases de dados locais pertencentes a programas instalados pelos utilizadores.

/boot

Trata-se do diretório onde se encontram variados arquivos necessários para a inicialização do sistema  operacional.  É  neste  diretório,  por  exemplo,  que  podemos  encontrar  os  arquivos BootLoader – responsáveis por gerir a inicialização do sistema.

/opt

Trata-se  do  diretório  que  contém  subdiretórios  para  pacotes  de  software  opcionais.  É comumente usada por softwares proprietários, que não obedecem à hierarquia do sistema de arquivos-padrão.  Por  exemplo:  um  programa  proprietário  pode  colocar  seus  arquivos  em /opt/aplicativo quando você instalá-lo.

/media

Trata-se  do  diretório  que  contém  subdiretórios  em  que  os  dispositivos  de  mídia  removível inseridos  no  computador  são  montados.  Por  exemplo: quando  você  insere  um  CD  em  seu sistema  Linux,  um  diretório  será  criado  automaticamente  dentro  do  diretório  /media.  Você pode acessar o conteúdo do CD dentro desse diretório.

/srv

Trata-se  do  diretório  que  contém  dados  para  serviços  prestados  pelo  sistema.  Se  você  usa  o servidor Apache em um site, por exemplo, provavelmente armazena os arquivos do seu site em um diretório dentro do /srv.


(PC/ES  –  2011)  O  sistema  de  diretório  do  Linux  apresenta  os  diretórios  de  maneira hierarquizada, por isso, também é conhecido como árvore de diretórios.
_______________________ Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





41
102




Comentários: conforme vimos em aula, a questão está perfeita (Correta).

(PC/MG – 2013)  Em  relação  à  estrutura  básica  dos  diretórios  do  sistema  operacional Linux, correlacione as colunas a seguir, numerando os parênteses:

Diretório      Finalidade I. /boot                   ( ) Contém arquivos para acessar periféricos.
II. /dev                    ( ) Contém os diretórios dos usuários.
III. /lib                              ( ) Contém arquivos necessários para a inicialização do sistema.
IV. /home                       ( ) Contém bibliotecas compartilhadas por programas.

A sequência CORRETA, de cima para baixo, é:

a) I, III, II, IV.
b) II, III, I, IV.
c) II, IV, I, III.
d) III, IV, I, II.
_______________________ Comentários: (I)    /boot  contém  arquivos  necessários  para  a  inicialização  do  sistema;  (II)  /dev  contém  arquivos  para  acessar periféricos; (III) /lib contém bibliotecas compartilhadas por programas; (IV) /home contém os diretórios dos usuários (Letra C).

(TRT/CE – 2017)  A  estrutura  de  diretórios  do  sistema  operacional  Linux,  os  diretórios /tmp e /dev são destinados, respectivamente, a:

a) arquivos variáveis, ou seja, passíveis de mudanças, como arquivos de logs do sistema;
e armazenamento de informações referentes aos usuários do sistema operacional.

b) arquivos temporários; e arquivos de configurações específicas de programas.

c) processos que estejam sendo executados; e arquivos de dispositivos.

d) arquivos temporários; e arquivos de dispositivos.
_______________________ Comentários: (a) Errado, a primeira parte trata do /var e a segunda do /home; (b) Errado, a primeira parte trata do /tmp e a segunda parte trata do /etc; (c) Errado, a primeira parte trata do /proc e a segunda parte trata do /dev; (d) Correto, a primeira parte trata do /tmp e a segunda parte trata do /dev (Letra D).


3.3 – GERENCIAMENTO DE PRIVILÉGIOS 
Uma das coisas que torna o Linux segura é a sua exigência de que cada coisa tenha dono e permissões  de  uso.  Assim,  para  que  seja  possível  restringir  ou  permitir  o  acesso  e  o  uso  de Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





42
102




determinados  recursos  a  uma  ou  mais  pessoas,  é  necessário  que  cada  uma  tenha  um  usuário devidamente  criado  no  sistema  operacional.  Criar  uma  conta  para  cada  usuário  no  sistema operacional  não  serve  apenas  para  restringir  ou  permitir  o  acesso  aos  recursos  oferecidos,  mas também para respeitar o espaço que cada pessoa tem.

Com uma conta, uma pessoa poderá ter os seus próprios diretórios, personalizar o seu desktop, ter atalhos e configurações para os seus programas preferidos, entre outros . Além disso, mesmo
que o computador seja utilizado apenas por uma pessoa, é recomendável criar um usuário próprio para ela. Por que, professor? Já não existe o usuário root? Porque o usuário root é o que "manda" no sistema – ele tem poderes de administrador e tem acesso a todos os recursos. Logo, usá-lo no dia- a-dia não é recomendável, visto que se o computador for tomado por outra pessoa ou se o próprio usuário fizer algo errado, o sistema operacional poderá ser seriamente comprometido.

O  Gerenciamento  de  Privilégios  permite  ao  administrador  do  sistema  definir  políticas  para acesso aos arquivos, diretórios e programas executáveis do sistema. Como vimos, os arquivos são organizados em diretórios e, portanto, o Linux oferece facilidades de proteção dos arquivos e diretórios.  Essas  proteções  são  organizadas  em  três  classes  de  privilégios:  privilégios  do  dono, privilégios de um grupo e privilégio dos outros usuários.

O dono do arquivo é normalmente aquele que criou o arquivo; o grupo é um conjunto de usuários que tem acesso a um determinado arquivo; e outros usuários são todos aqueles que não donos de arquivos ou que pertençam a um grupo.
Além disso, cada classe de privilégio é composta por três níveis  básicos  de  permissões:  permissão  de  leitura,  permissão  de  escrita  e  permissão  de execução
. Vamos ver em detalhes:

PERMISSÃO DESCRIÇÃO
Leitura
[r]
Permissão de leitura de arquivos e listagem de conteúdo em diretórios.

Escrita
[w]
Permissão de escrita em arquivos ou diretórios.
Execução
[x]
permissão de execução de arquivos ou de acesso a diretórios.

Beleza! Nós vimos que existem três classes de privilégios e esses privilégios possuem três níveis de permissões. Agora  como  eu  sei  que  determinado  arquivo,  por  exemplo,  pode  ser  acessado  ou modificado  ou  executado  pelo  dono,  grupo  ou  outros usuários? Para  isso,  necessário  identificar alguns  dados  sobre  esse  arquivo  no  terminal  de  linha  de  comando .  Todo  arquivo  terá  um conjunto de 10 caracteres que trarão todas essas informações.



DONO - LEITURA
DONO - ESCRITA
DONO - EXECUÇÃO
OUTROS - LEITURA
OUTROS - ESCRITA
OUTROS - EXECUÇÃO
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





43
102




-rwx rwx rwx





TIPOS DE OBJETO
d Diretório b Arquivo de bloco c Arquivo especial de caractere p Canal s Socket - Arquivo normal 
Professor, não entendi muito bem! Galera,  vejam  só:  existe  um  comando  capaz  de  listar  arquivos detalhados de um diretório ou arquivo pelo terminal de linha de comando.
Entre esses detalhes, há os dez caracteres que eu mencionei anteriormente que indica as classes de privilégio e níveis de permissão
. Vamos ver um exemplo? Na imagem abaixo, é possível ver que o Diretório Vídeos está listado como drwxr-xr-x. O que isso significa?

Podemos  ver  que  é  um  diretório;  podemos  ver  que  o  dono  tem  permissão  de  leitura,  escrita  e execução; podemos ver que o grupo tem permissão para leitura e execução, mas não de escrita;
podemos ver que outros usuários têm permissão para leitura e execução, mas não de escrita. Existe um comando chamado chmod responsável pela atribuição de permissões de arquivos . Dito isso,
é hora finalmente de conhecermos alguns comandos...

TIPO DE OBJETO
GRUPO - LEITURA
GRUPO - ESCRITA
GRUPO - EXECUÇÃO
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





44
102




(UFRJ – 2014) No tocante à utilização de comandos para organização e manipulação de arquivos  e  diretórios  no  sistema  operacional  Linux,  o  comando  responsável  pela atribuição de permissões de arquivos é o:

a) tail
b) vi
c) chmod
d) nmap
e) top
_______________________ Comentários: conforme vimos em aula, trata-se do chmod (Letra C).

(SERPRO – 2010) Considere que, após a execução do comando ls , um usuário obtenha a seguinte resposta:

drwxrwxrwx João users teste 
Nesse caso, no trecho drwxrwxrwx, d identifica o tipo de arquivo como arquivo comum;
a  segunda,  a  terceira  e  a  quarta  letras  —  rwx  —  garantem  a  João  a  permissão  de  ler, gravar e executar o arquivo teste; respectivamente; e a quinta, a sexta e a sétima letras — rwx — especificam, respectivamente, que, do grupo users, apenas João terá acesso ao arquivo teste.
_______________________ Comentários: conforme vimos em aula, d identifica o tipo de arquivo como diretório. Ademais, a quinta, sexta e sétima letras especificam que todos presentes no grupo terão permissão para ler, gravar e executar o arquivo teste (Errado).















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





45
102




4 – PRINCIPAIS COMANDOS 
Galera, para entender os principais comandos, nós precisamos entender o conceito de Shell! Esse é o nome dado a uma classe de programas que funcionam como interpretador de comandos e linguagem  de  programação  interpretada  no  Unix .  Não  vamos  tratar  aqui  de  linguagens  de programação,  o  nosso  foco  é  no  interpretador  de  comandos.  Pessoal,  vocês  sabem  que computadores só fazem o que nós mandamos fazer.

Computadores não pensam por si só! Tudo que eles fazem, são os usuários que mandam ou o que os desenvolvedores programam. Quando você quer ver o que tem dentro do seu pendrive, você utiliza o mouse para procurar a pasta dele, dá um duplo clique e visualiza o que há na pasta. Se você  quiser  excluir,  copiar,  colar,  recortar,  entre  diversas  outras  possibilidades,  você  pode  fazer tudo isso facilmente por meio de janelas, ícones, menus, etc.
























No  entanto,  há  outra  maneira  de  realizar  todas  essas  atividades. Como, professor?  Utilizando  o Shell!
Como eu disse, o Shell é uma interface de linha de comandos para acessar os serviços de um sistema operacional . Agora vejam que bacana: shell é o mesmo que casca, em inglês. Vocês sabem o porquê? Porque ele é a camada mais externa em torno do núcleo do sistema operacional.
A imagem acima deixa isso mais claro...

Shell
Kerne
l
Hard
ware
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





46
102





(UFPE  –  2014)  No  sistema  operacional  Linux,  a  interface  de  linha  de  comando semelhante ao Prompt de comando do sistema Windows é conhecida como:

a) prompt.
b) boot.
c) shell.
d) gui.
e) Xwindow.
_______________________ Comentários: conforme vimos em aula, trata-se do shell (Letra C).















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





47
102




4.1 – TIPOS DE COMANDOS 
Nós  veremos  à  frente  vários  comandos  diferentes  que  podem  ser  utilizados  no  interpretador  de comandos do Linux, mas antes vamos ver que eles se dividem em comandos internos e externos.

4.1.1 – Comandos Internos São comandos que estão dentro de um shell interpretador de comandos.  Quando  o  shell  é carregado na memória, seus comandos ficam residentes nela. A maior vantagem é a velocidade, pois não precisam ser procurados no disco rígido ou criar processos. Exemplos: cd, alias e logout.
4.1.2 – Comandos Externos São comandos que estão localizados em diretórios específicos no disco rígido, como /bin e /sbin.
O Linux precisa consultar o disco rígido sempre que um desses comandos é solicitado. A maioria dos comandos do Linux é externa. Exemplos: ls, cp, rm, mv, mkdir e rmdir.

Professor,  é  verdade  que  Linux  e  Windows  possuem  comandos  diferentes  para  executar  uma mesma tarefa? Sim, um exemplo clássico são os comandos ls e dir – que fazem a mesma coisa!

(IBAMA  –  2012)  Quando  se  liga  um  computador,  o  sistema  operacional  é  acionado, possibilitando inicializar e gerenciar o hardware e tornando possível sua utilização pelo usuário. O Linux e o Windows são sistemas operacionais distintos e possuem comandos diferentes para executar uma mesma tarefa,  como listar arquivos de um diretório, por exemplo.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).

IMPORTANTE

Abaixo veremos diversos comandos. Cada comando pode ser modificado por meio de parâmetros. Os parâmetros podem ser combinados de diversas formas. Por exemplo:

ls -l -a = ls -a -l = ls -la = Ls -al 

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





48
102




4.2 – COMANDO LS

Trata-se de um comando que exibe o conteúdo de diretórios (ls = list source). Por ser o comando mais frequente em provas, vamos vê-lo com mais detalhes...

PARÂMETRO DESCRIÇÃO
-
Ao simplesmente digitar ls no shell e pressionar a Tecla Enter, o usuário pode conferir  uma  lista  com  os  arquivos  contidos  no  diretório,  sem  maiores detalhes,  sem  que  sejam  exibidas  informações  tais  como,  por  exemplo, tamanho dos arquivos, data de modificação, etc:



PARÂMETRO DESCRIÇÃO
ls -l
Lista  os  arquivos  utilizando  o  formato  longo  dos  nomes  dos  arquivos, mostrando detalhes sobre permissões, tamanho, tipo, etc (l = long).



PARÂMETRO DESCRIÇÃO
ls -a
Lista todos os arquivos de um diretório, inclusive os arquivos ocultos (a = all).




PARÂMETRO DESCRIÇÃO
ls -t
Lista  os  arquivos  por  ordem  de  data  de  modificação.  Arquivos  que  foram modificados por último, mais recentemente, são exibidos em primeiro lugar.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





49
102






PARÂMETRO DESCRIÇÃO
ls -lt
Lista  os  arquivos  por  ordem  de  data  de  modificação,  também  exibindo  os modificados   mais   recentemente   em   primeiro   lugar.   No   entanto,   este comando lista tudo com mais detalhes.



PARÂMETRO DESCRIÇÃO
ls -ltr
Similar ao comando acima com a diferença de listar em ordem inversa, ou seja, os modificados mais recentemente vão ficando para o final da lista.



PARÂMETRO DESCRIÇÃO
ls -s
O comando acima exibe os arquivos de uma pasta em formato de bloco, sendo que eles são ordenados por tamanho:



PARÂMETRO DESCRIÇÃO
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





50
102




ls -1
Permite fazer com que os arquivos do diretório sejam listados por linha, um em cada linha.



PARÂMETRO DESCRIÇÃO
ls -lh
Para obter uma listagem de arquivos que exiba seus respectivos tamanhos de uma forma mais compreensível ou Human Readable (humanamente legível).
Dessa forma, você pode conferir os tamanhos em Kb, Mb, Gb, etc.



PARÂMETRO DESCRIÇÃO
ls -lh
Para obter uma listagem de arquivos que exiba seus respectivos tamanhos de uma forma mais compreensível ou Human Readable (humanamente legível).
Dessa forma, você pode conferir os tamanhos em Kb, Mb, Gb, etc.

(FUNDASUS – 2015) Um analista de suporte necessita executar o comando Linux que lista todos os arquivos (inclusive ocultos) de uma determinada pasta, com todos os seus detalhes. Para tanto, o comando que o analista de suporte deve utilizar é o:

a) ls -A
b) ls -la
c) -ls a
d) ls -l
e) ls
_______________________ Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





51
102




Comentários: conforme vimos em aula, trata-se do ls -la, visto que a questão fala em arquivos (inclusive ocultos) e também fala que é uma lista com todos os seus detalhes (Letra B).

(EBC  –  2016)  No  ambiente  Linux,  o  comando  ls  permite  listar  todos  os  arquivos  do diretório atual.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).

(PC/AC – 2015) O comando Linux, usado para listar o conteúdo de um diretório, é o:

a) cd.
b) rm.
c) ls.
d) md.
e) dir.
_______________________ Comentários: conforme vimos em aula, trata-se do ls (Letra C).

























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





52
102




4.3 – COMANDO CD

Este comando permite ao usuário mudar o diretório de trabalho. A mudança de diretório pode ser feita de forma sequencial (de diretório pai para diretório filho ou vice-versa) ou pode ser feita de forma aleatória (de um diretório qualquer para outro diretório qualquer).

PARÂMETRO DESCRIÇÃO
-
Quando utilizado sem parâmetro, esse comando permite ir para o diretório home.

cd /
Permite ir para o diretório raiz do Linux.

cd nome-do-
diretório
Permite ir para um diretório filho do diretório atual.

cd ..
Permite ir para o diretório pai do diretório atual.

cd ../ nome-do-
diretório
Permite ir para um diretório do mesmo nível (diretório irmão) do diretório atual.

cd -
Permite voltar ao último diretório visitado antes do diretório atual.

cd /usr/lib
Permite fornecer o caminho completo do diretório para onde quer ir.


(IF/AM – 2014) Se um usuário de um sistema Linux quiser sair de um diretório e ir para outro, deve digitar, no prompt de comados, o comando:

a) apropos.
b) bg.
c) cat.
d) cd.
e) ls.
_______________________ Comentários: conforme vimos em aula, trata-se do cd (Letra D).











Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





53
102




4.4 – COMANDO CP

Esse comando é utilizado para copiar arquivos (cp = copy). O arquivo de origem e o destino da cópia podem residir em sistemas de arquivo diferentes, ou até no mesmo diretório desde que tenham nomes diferentes . Este comando copia também mais de um arquivo de um diretório para outro. Para criar uma cópia do arquivo teste.txt com o nome teste_bak.txt, basta digitar:

cp   teste.txt   teste_bak.txt 
É possível especificar mais de um arquivo no comando cp usando os curingas *, ? e [ ]. O primeiro substitui um grupo qualquer de caracteres (qualquer número de caracteres, inclusive zero, e para qualquer  valor  de  caractere);  o  segundo  substitui  apenas  um  caractere  (qualquer  caractere);  e  o terceiro substitui um único caractere dentro de uma faixa de valores. Abaixo são mostrados alguns exemplos:

cp   teste*.txt   /tmp/.    cp   teste?.txt   /tmp/.    cp   teste[1-3].txt   /tmp/.

O primeiro comando acima copia todos os arquivos do diretório atual que começam por teste e têm  extensão  txt  para  o  diretório  /tmp .  O  segundo  comando  copia  todos  os  arquivos  que começam  por  teste,  têm  um caractere  qualquer  na  sexta  posição  e  extensão  txt para  o  diretório /tmp. O último comando copia os arquivos teste1.txt, teste2.txt e teste3.txt (se existirem) para o diretório /tmp.

PARÂMETRO DESCRIÇÃO
-b
Gera cópia de segurança se o arquivo de destino já existir.

-f
Substitui arquivos existentes sem pedir confirmação.

-i
Pede permissão antes de substituir arquivos existentes.

-l
Cria um link para o arquivo de origem ao invés de copiar o arquivo.

-r
Copia arquivos e subdiretórios (recursivo).

-u
Copia apenas quando o arquivo de origem é mais novo que o arquivo de destino ou quando o arquivo de destino não existe.
-v
Lista os arquivos copiados.





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA ==12b2d8==






54
102




4.5 – COMANDO RM

Este comando remove arquivos. É uma forma curta de se referir a remove (remover).

PARÂMETRO DESCRIÇÃO
-f Apaga sem pedir confirmação.
-i Apaga após pedir confirmação.
-r Apaga arquivos e subdiretórios.
-v Lista arquivos deletados.

 Para apagar o arquivo teste.txt, basta digitar: rm teste.txt.
 Para apagar o diretório teste e todo o seu conteúdo, digite: rm -fr teste.

(TCM/CE – 2010) Remove arquivos no Linux o comando:

a) pwd
b) mkdir
c) cd
d) rm
e) tar
_______________________ Comentários: conforme vimos em aula, trata-se do rm (Letra D).


















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





55
102




4.6 – COMANDO RMDIR

Este comando remove diretórios vazios – o diretório tem que estar vazio antes de ser excluído.

PARÂMETRO DESCRIÇÃO
-p Remove uma hierarquia de diretórios.
-v Exibe informações para cada diretório processado.
--help Informa as opções do aplicativo.
--version Exibe a versão implementada do aplicativo.

(CEFET/RJ  –  2010  –  Item  I)  No  Linux,  o  comando rmdir  diretório  apaga  o  diretório informado (sublinhado) desde que o mesmo esteja vazio.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).



























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





56
102




4.7 – COMANDO MV

Este comando move (ou renomeia) arquivos.

PARÂMETRO DESCRIÇÃO
-b Gera cópia de segurança se o arquivo de destino já existir.
-f Move o arquivo sem pedir confirmação.
-i Move o arquivo, mas pede confirmação caso já exista um arquivo com o mesmo nome.
-v Exibe os nomes dos arquivos afetados pelo comando.
--help Exibe as opções do comando.
--version Exibe informações sobre o comando.

(IF/MT  –  2015)  No  sistema  operacional  Linux,  qual  o  comando  para mover  todos  os arquivos com extensão .jpg de uma pasta com muitos arquivos para outra?

a) $ vm *.jpg /outra-pasta b) $ mv *.jpg /outra-pasta c) $ rd *.jpg /outra-pasta d) $ cp *.jpg /outra-pasta _______________________ Comentários: conforme vimos em aula, trata-se do comando $mv *.jpg /outra-pasta (Letra B).

(SEGESP/AL  –  2013)  Em  ambiente  Linux,  o  comando  mv  é  utilizado  para  mover  ou renomear um ou mais arquivos e diretórios, o que facilita a organização das informações.
_______________________ Comentários: conforme vimos em aula, a questão está perfeita (Correto).














Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





57
102




4.8 – COMANDO MAN

Este utilitário formata e apresenta páginas do manual on-line sobre um determinado comando.

PARÂMETRO DESCRIÇÃO
-a
Mostra  todas  as  páginas  para  o  nome  definido  seguindo  a  ordem  das  seções  definida  em /etc/manpath.config.
-f ou –whatis
apresenta  apenas  uma  pequena  descrição  do  comando. Esta  opção  fornece  o  mesmo resultado do comando whatis.

(UFPE – 2014) Num PC rodando o sistema operacional Linux , quando se deseja obter informações de ajuda sobre um utilitário ‘du’, deve-se executar o comando:

a) help du.
b) ajuda du.
c) manual du.
d) man du.
e) howto du.
_______________________ Comentários: conforme vimos em aula, trata-se do man du (Letra D).

(TRT/SP  –  2018)  Para  conhecer  a  finalidade  de  um  comando  no  Linux,  um  Técnico precisará  digitar  um  primeiro  comando  seguido  do  nome  do  comando  que  deseja conhecer. O primeiro comando que terá que utilizar, nesse caso, é o:

a) bash
b) help
c) man
d) show
e) ls
_______________________ Comentários: conforme vimos em aula, trata-se do man (Letra C).








Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





58
102




4.9 – COMANDO DF

Este comando exibe informações sobre espaço livre e espaço usado nas partições do sistema.

PARÂMETRO DESCRIÇÃO
-a Inclui também na listagem os sistemas de arquivos com zero blocos.
--help Exibe as opções do comando.
-k Lista o tamanho dos blocos em kbytes.
-m Lista o tamanho dos blocos em Mbytes.

(PC/AC – 2015) Um usuário de um ambiente com sistema operacional Linux deseja saber quanto de espaço foi utilizado no seu disco rígido. O comando para essa operação é o:

a) df.
b) find.
c) whereis.
d) top.
e) ssh.
_______________________ Comentários: conforme vimos em aula, trata-se do df (Letra A).

(FUNDAÇÃO  CASA  –  2014)  Com  relação  ao  sistema  operacional  Linux,  assinale  a alternativa  que  apresenta  o  comando  que  exibe  a  quantidade  de  espaço  livre  nas unidades de disco do computador, no qual o sistema operacional está instalado.

a) free.
b) cd.
c) ls.
d) pwd.
e) df.
_______________________ Comentários: conforme vimos em aula, trata-se do df (Letra E).








Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





59
102




4.10 – COMANDO SUDO

O comando sudo do sistema operacional Unix permite a usuários comuns obter privilégios de outro usuário,  em  geral  o  superusuário  (root),  para  executar  tarefas  específicas  dentro  do  sistema  de maneira segura e controlável pelo administrador.

PARÂMETRO DESCRIÇÃO
-h Exibe as opções do comando.
-l Lista os comandos permitidos e proibidos para o usuário no ambiente de trabalho atual.
-u usuário O sudo executa o comando com os privilégios do usuário especificado.
-V Fornece informações sobre o comando.

(UFG – 2018)  Muitas  vezes  um  usuário  do  sistema  operacional  Linux  Ubuntu  precisa executar  programas  com  permissão  de  superusuário.  Para  isso,  ele  pode  usar  o comando:

a) root.
b) chmod.
c) sudo.
d) chown.
_______________________ Comentários: conforme vimos em aula, trata-se do sudo (Letra C).



















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





60
102




4.11 – COMANDO GREP

Realiza buscas no conteúdo dos arquivos (ou input) procurando linhas que respeitem um padrão.

PARÂMETRO DESCRIÇÃO
-a Trata arquivos binários como se fossem arquivos de texto.
-c Imprime somente a contagem das linhas com expressão.
-i Ignora a diferença entre letras maiúsculas e letras minúsculas.

(TRT/PE – 2018) Um Analista recebeu um arquivo chamado funcionarios.txt contendo o nome e outras informações de cerca de 10000 funcionários. Ao ser solicitado a localizar os  dados  do  funcionário  Marconi  Teixeira  nesse  arquivo,  estando  na  pasta  em  que  se encontra o arquivo em um terminal Linux, digitou o comando:

a) get 'Marconi Teixeira' from funcionarios.txt b) grep 'Marconi Teixeira' funcionarios.txt c) ls 'Marconi Teixeira' in funcionarios.txt d) locate 'Marconi Teixeira' >> funcionarios.txt e) search 'Marconi Teixeira' funcionarios.txt _______________________ Comentários: conforme vimos em aula, devemos buscar o padrão ‘Marconi Teixeira’ no arquivo funcionários.txt (Letra B).




















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





61
102




4.12 – COMANDO CAT

O comando cat, do sistema operacional, Unix é usado para unir, criar e exibir arquivos.

PARÂMETRO DESCRIÇÃO
-n Numera todas as linhas.
--version Mostra informações sobre o aplicativo.

(CISMEPAR/PR – 2016) Em um computador com sistema operacional Linux, o comando fdisk   consegue   gerenciar   partições   no   HD.   Todavia, é   importante   conhecer   a funcionalidade  do  comando,  para  evitar  a  perda  de  dados.  Um  comando  com  grande utilidade  no  Linux,  que  permite  mostrar  o  conteúdo de  um  arquivo,  está  presente  na alternativa:

a) cat
b) cal
c) top
d) type
_______________________ Comentários: conforme vimos em aula, trata-se do cat (Letra A).






















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





62
102




4.13 – COMANDO APT-GET 
Este utilitário permite a instalação, reinstalação, atualização e remoção de pacotes do sistema.

PARÂMETRO DESCRIÇÃO
-h Fornece as opções do utilitário.
-u Mostra a lista de pacotes sendo atualizada.

(DETRAN/RO  –  2014)   Qual   a   finalidade   do   comando   apt-get   install   --reinstall nome_do_pacote utilizado no Linux/Unix?

a)  Instalar um determinado pacote.
b) Atualizar o pacote especificado.
c) Procurar um determinado pacote.
d) Deletar um determinado pacote.
e) Reinstalar um determinado pacote.
_______________________ Comentários: conforme vimos em aula, ele reinstala um determinado pacote (Letra E).























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





63
102




4.14 – COMANDO CHMOD 
Trata-se do comando que permite alterar permissões de acesso de objetos do sistema (arquivos e diretórios) –
chmod vem de change mode.

PARÂMETRO DESCRIÇÃO
-c Informa quais arquivos estão tendo as permissões alteradas.
-v Informa quais arquivos estão sendo processados (não necessariamente alterados).

(UFRJ – 2014) No tocante à utilização de comandos para organização e manipulação de arquivos  e  diretórios  no  sistema  operacional  Linux,  o  comando  responsável  pela atribuição de permissões de arquivos é o:

a) chmod
b) tail
c) vi
d) nmap
e) top
_______________________ Comentários: conforme vimos em aula, trata-se do chmod (Letra A).




















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





64
102




4.15 – OUTROS COMANDOS 
COMANDO DESCRIÇÃO
cut Mostra apenas seções específicas de um arquivo de texto ou da saída de outros comandos.
diff Compara o conteúdo de dois arquivos.
du Exibe um resumo do uso do espaço em disco find Localiza arquivos para pesquisa de arquivos de texto do diretório atual.
gzip Comprime ou descomprime um arquivo.
head Mostra as primeiras linhas de um arquivo tail Mostra as últimas linhas de um arquivo kill Finaliza (mata) um processo.
mkdir Cria um diretório.
rmdir Remove um diretório mount Inclui o sistema de arquivos de um dispositivo qualquer no sistema de arquivos do Linux.
pwd Mostra o caminho por inteiro do diretório atual, isto é, um pathname.
passwd Muda o password do utilizador (usuário logado).
top Lista os processos que mais utilizam processamento.
shutdown Desliga ou reinicia o sistema.
su Permite mudar de usuário em um ambiente shell.
touch Permite alterar a data e a hora do último acesso e/ou data de modificação de um arquivo.
vi Abre o Editor VI para editar/criar arquivos.
clear Este comando limpa a tela do terminal.





















Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





65
102




RESUMO
SISTEMA OPERACIONAL: LINUX 
Características Essenciais 
CARACTERÍSTICAS DO LINUX É multitarefa, isto é, o sistema pode executar mais de uma aplicação ao mesmo tempo.
É multiusuário, isto é, um mesmo computador pode ter várias contas de usuário.
É preemptivo, isto é, permite a interrupção de processos.
Suporta nomes extensos de arquivos e pastas (255 caracteres).
Conectividade com outros tipos de plataformas como: Apple, Sun, Macintosh, Sparc, Unix, Windows, DOS, etc.
Utiliza permissões de acesso à arquivos, pastas e programas em execução na memória RAM.
Proteção entre processos executados na memória RAM.
Modularização: ele só carrega para a memória o que é utilizado durante o processamento.
Não há a necessidade de reiniciar o sistema após modificar a configuração de qualquer periférico de computador ou parâmetros da rede.
Em geral, não necessita de um processador potente para funcionar.
Suporta diversos dispositivos e periféricos disponíveis no mercado, tanto os novos como os obsoletos.
Possui controles de permissão de acesso (Login e Logout).

Rotinas de Inicialização 
ROTINAS DESCRIÇÃO
LILO
Trata-se de um gerenciador de inicialização mais antigo – vejam que ele tem uma interface mais simples e rústica.
Era o carregador de boot mais popular para Linux até 2001, quando o Bootloader GRUB começou a substituí-lo.

GRUB
Trata-se de um gerenciador de inicialização mais recente –ele é mais bonito e moderno que o anterior, é mais poderoso  que  o  LILO  e  suporta  um  número  ilimitado  de  entradas  de  sistemas  operacionais,  além  de  permitir sistemas de arquivo maiores.

Tipos de Usuário

USUÁRIO DESCRIÇÃO
COMUM
São aqueles que possuem contas para utilização do sistema operacional. Basicamente, esses usuários possuem um diretório base (/home/username, exemplo) e podem criar e manipular arquivos em seu diretório e em outros diretórios, além de executar tarefas simples como criar e editar documentos, navegar na internet, ouvir música etc. Ao contrário do usuário administrador, o usuário comum é inviabilizado para realização de algumas tarefas a nível de sistema. Em geral, vem com um símbolo de cifrão ($) na linha de comando.
ADMINISTRADOR
Também chamado de Root, é responsável por controlar todo o sistema e não possui quaisquer tipos de restrições.
Sempre que executado algum software ou atividade que precise de acesso administrativo, é necessário o root, que é chamado por meio do comando sudo. Por exemplo: sempre que for instalar um programa ou realizar um upgrade de todo o sistema operacional, é utilizado o comando sudo para se ter as permissões de root e conseguir efetuar essas tarefas. Em geral, vem com um símbolo de cerquilha (#) na linha de comando.
SISTEMA
Usuários  que  não  necessitam  estar  logados  no  sistema  para  controlar  alguns  serviços.  Estes  comumente  não possuem senhas e, diferentemente dos usuários comuns, não se conectam. São contas usadas para propósitos específicos do sistema e não são de propriedade de uma pessoa em particular. Um exemplo desse tipo de usuário é o www-data, que pode ser utilizado para controlar servidores web como Apache e Nginx.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





66
102




Distribuições Linux

DEFINIÇÃO
Trata-se de um sistema operacional criado a partir de uma coleção de software construído sobre o Kernel do Linux. Cada distribuição possui recursos que a tornam única. Algumas distribuições são projetadas para uso geral, enquanto outras são projetadas para um caso de uso muito específico, como um firewall ou um servidor da Web. A escolha da distribuição que funciona melhor para você pode levar algum tempo. As principais distribuições atualmente são: Debian, Ubuntu, RedHat, Fedora, Suse, Mint, CentOS, Mandrake, Slackware, etc. Galera, existem – inclusive – distribuições brasileiras. As mais famosas são a Kurumin, Conectiva, Kalango e Mandriva.

Sistemas de Arquivos 
USUÁRIO DESCRIÇÃO
EXT2
Um  dos  primeiros  sistemas  de arquivos  utilizado  nas  primeiras versões  do Linux  foi  o EXT2  (Second Extended FileSystem) – embora ele tenha sido uma espécie de padrão não era muito eficiente.
EXT3
Trata-se de uma versão do EXT2, porém com suporte a journaling. Essa característica foi uma evolução e tornou o EXT3 um sistema de arquivos muito estável e robusto.
EXT4
Este  é  uma  espécie  de  versão  do  EXT3  que  surgiu  com  a  prerrogativa  de  melhorar  o  desempenho  de compatibilidade, formatos e limites de armazenamentos.
REISERFS
Criado   recentemente   e   suportado   por   quase   todas   as distribuições,   apresenta   ótima   performance, principalmente para um número muito grande de arquivos pequenos.

Estrutura de Diretórios 

Padrão FHS
/binProgramas utilizados com frequência /bootArquivos utilizados durante a inicializaçãodo sistema /devDispositivos de hardware /etcArquivos de configuração do sistema e dos programas /homePasta para os diretórios dos usuários /libBibliotecas essenciais e módulos Linux /sbinProgramas essenciais para o funcionamento do sistema /rootDiretório pessoal do usuário root /optSoftwares adicionados de maneira não padrão /procInformações sobre os processos sendo executados /mediaPontos de montagem de mídias removíveis /mntConexão de volumes de rede e dispositivos removíveis /tmpArquivos temporários do sistema /usrArquivos acessados pelo usuário /varInformações variáveis do sistema /srvDados dos serviços do sistema Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





67
102




Gerenciamento de Privilégios 
PERMISSÃO DESCRIÇÃO
LEITURA [r]
Permissão de leitura de arquivos e listagem de conteúdo em diretórios.
ESCRITA [w]
Permissão de escrita em arquivos ou diretórios.
EXECUÇÃO [x]
permissão de execução de arquivos ou de acesso a diretórios.




-rwx rwx rwx





TIPOS DE OBJETO
d Diretório b Arquivo de bloco c Arquivo especial de caractere p Canal s Socket - Arquivo normal 
Principais Comandos

COMANDO DESCRIÇÃO
ls
Trata-se de um comando que exibe o conteúdo de diretórios (ls = list source).

cd
Este  comando  permite  ao  usuário  mudar  o  diretório  de  trabalho.  A  mudança  de  diretório  pode  ser  feita  de  forma sequencial ou pode ser feita de forma aleatória.
cp
Esse comando é utilizado para copiar arquivos (cp = copy). O arquivo de origem e o destino da cópia podem residir em sistemas de arquivo diferentes, ou até no mesmo diretório desde que tenham nomes diferentes.
rm
Este comando remove arquivos. É uma forma curta de se referir a remove (remover).

rmdir
Este comando remove diretórios vazios – o diretório tem que estar vazio antes de ser excluído.

mv
Este comando move (ou renomeia) arquivos.

man
Este utilitário formata e apresenta páginas do manual on-line sobre um determinado comando.

df
Este comando exibe informações sobre espaço livre e espaço usado nas partições do sistema.

TIPO DE OBJETO
DONO - LEITURA
DONO - ESCRITA
DONO - EXECUÇÃO
GRUPO - LEITURA
GRUPO - ESCRITA
GRUPO - EXECUÇÃO
OUTROS - LEITURA
OUTROS - ESCRITA
OUTROS - EXECUÇÃO
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





68
102




sudo
Este comando permite a usuários comuns obter privilégios de outro usuário, em geral o superusuário (root), para executar tarefas específicas dentro do sistema de maneira segura e controlável pelo administrador.
grep
Realiza buscas no conteúdo dos arquivos (ou input) procurando linhas que respeitem um padrão.

cat
O comando cat, do sistema operacional, Unix é usado para unir, criar e exibir arquivos.

apt-get
Este utilitário permite a instalação, reinstalação, atualização e remoção de pacotes do sistema.

chmod
Trata-se do comando que permite alterar permissões de acesso de objetos do sistema (arquivos e diretórios) – chmod vem de change mode.









Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





69
102




MAPA MENTAL

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





70
102





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





71
102





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





72
102




EXERCÍCIOS COMENTADOS – DIVERSAS BANCAS 
1. (COVEST-COPSET  /  UFPE  /  2013)  No  sistema  operacional  Linux,  a  interface  de  linha  de comando semelhante ao Prompt de comando do sistema Windows é conhecida como:

a) prompt.
b) boot.
c) shell.
d) gui.
e) Xwindow.

Comentários:

No entanto, há outra maneira de realizar todas essas atividades. Como, professor? Utilizando o Shell! Como eu disse, o Shell é uma interface de linha de comandos para acessar os serviços de um sistema operacional. Agora vejam que bacana: shell é o mesmo que casca, em inglês. Vocês sabem o porquê? Porque ele é a camada mais externa em torno do núcleo do sistema operacional. A imagem acima deixa isso mais claro...

Conforme vimos em aula, trata-se do shell.

Gabarito: Letra C

2. (UFCG / UFCG/ 2016) No ambiente Linux, o comando $ ls:

a) Mostra a quantidade de espaço usada no disco rígido.
b) Mostra o uso da memória.
c) Lista todos os arquivos do diretório.
d) Abre um arquivo.
e) Abre o explorador de informações.

Comentários:

Trata-se de um comando que exibe o conteúdo de diretórios (ls = list source). Por ser o comando mais frequente em provas, vamos vê-lo com mais detalhes...

Conforme vimos em aula, ele lista todos os arquivos do diretório.

Gabarito: Letra C

3. (IBADE / SEDUC-RO / 2016) Um sistema operacional pode ser definido como um conjunto de programas  especialmente  feitos  para  a  execução  de  várias  tarefas,  entre  as  quais  servir  de intermediário entre o utilizador e o computador. Um sistema operacional tem também como Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





73
102




função  gerir  todos  os  periféricos  de  um  computador.  Analise  as  afirmativas  abaixo  sobre  os sistemas operacionais Linux e Windows.

I. O Windows é o software livre mais comumente encontrado nos computadores, ao contrário do Linux que se configura como um software proprietário.
II. Ambos os sistemas operacionais são multiusuários.
III.  No  ambiente  Windows,  não  é  possível  manter  duas  ou  mais  versões  do  mesmo  arquivo armazenadas em locais diferentes.

Está correta apenas o que se afirma em:

a) I.
b) II.
c) III.
d) I e III.
e) I e II.


Comentários:

(I)  Errado,  a  questão  inverteu  os  conceitos  –  Windows  é  proprietário  e  Linux  é  livre;  (II)  Correto, ambos os sistemas operacionais permitem a utilização por mais de um usuário; (III) Errado, é claro que é possível.

Gabarito:
Letra B

4. (COPESE - UFPI / Pref. de Bom Jesus – PI / 2015)  Sobre  sistemas  operacionais  (Windows  e Linux) assinale a opção CORRETA.

a) Os sistemas operacionais utilizam sempre o mesmo sistema de arquivos, no caso o chamado NTFS.

b)  Os  programas  desenvolvidos  para  Linux  funcionam normalmente,  sem  necessitar  de adaptações no Windows e vice-versa.

c)  O  sistema  operacional  é  um  software  cuja  função é  gerenciar  os  recursos  do  sistema, fornecendo  uma interface  entre  o  computador  e  o  usuário  e  fornecendo  suporte para  que  os demais programas possam funcionar.

d) Firefox e Chrome são exemplos de sistemas operacionais.

e)  A  multitarefa  é  um  recurso  do  sistema  operacional  que  permite  ele  seja  executado  em máquinas diferentes.

Comentários:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





74
102




(a) Errado. NTFS é um sistema de arquivos do Windows e, não, do Linux – e existem várias opções de sistemas de arquivos para cada sistema operacional; (b) Errado. São necessárias adaptações para funcionar em outro sistema operacional; (c) Correto, a questão está perfeita; (d) Errado. Ambos são navegadores   web;   (e)   Errado,   ela   permite   a   execução   de  processos   simultâneos  em   um computador.

Gabarito:
Letra C

5. (IBFC  /  EMBASA  /  2015)  Quanto  as  características  dos  Sistemas  Operacionais,  analise  as afirmativas abaixo, dê valores Verdadeiro (V) ou Falso (F) e assinale a alternativa que apresenta a sequência correta (de cima para baixo):

( ) 0 Windows é considerado um Sistema Operacional proprietário.
( ) O Linux somente funciona com processadores da Intel.

a) V - V
b) V - F
c) F - V
d) F - F.

Comentários:

Ele é um exemplo de sistema operacional livre amplamente difundido que pode ser utilizado tanto em  servidores  de grandes empresas  –  onde  ele  é  mais  frequente –  quanto em computadores pessoais,  passando  por  diversas  arquiteturas ou plataformas de  hardware  diferentes. Existem muitas questões que querem enganar o aluno dizendo que ele só funciona em servidores.
MEN-TI-RA! Ele funciona tanto em servidores quanto em computadores pessoais.

O Windows é realmente um sistema operacional proprietário, mas o Linux funciona com diversos processadores.

Gabarito: Letra B

6. (COPESE - UFPI / UFPI / 2015) Assinale a opção que corresponde a um sistema operacional cujo código fonte está disponível sob a licença GPL (General Public License – Licença Pública Geral) para que qualquer pessoa o possa utilizar, estudar, modificar e distribuir livremente de acordo com os termos da licença.

a) Windows XP.
b) Windows Vista.
c) Linux.
d) Word 2010.
e) BrOffice.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





75
102




Comentários:

Ao contrário de um software proprietário, ele é um software livre, cujo código-fonte está aberto e disponível sob a Licença GPL (Genereal Public License) para que o usuário possa ter acesso ao código-fonte com o intuito de utilizá-lo executá-lo, estudá-lo, modificá-lo e distribuí-lo livremente de acordo com os termos da licença. Ele é desenvolvido, em geral, por uma comunidade de programadores voluntários espalhados pelo mundo que contribuem para melhorá-lo.

Conforme vimos em aula, trata-se do Linux (Letra C).

Gabarito: Letra C

7. (Pref. do RJ / CM do RJ / 2015) Da mesma forma que no Windows 7 e 8, o Ubuntu Linux 13.04 disponibiliza diversos atalhos de teclado para uso. Neste contexto, um deles deve ser utilizado para  alternar  o  acesso  entre  aplicativos  abertos  e em  execução  de  forma  concorrente.  Esse atalho é:


a) Alt + Tab
b) Alt + Home
c) Super + Tab
d) Super + Home.

Comentários:

Da mesma forma do Windows, é possível alternar entre aplicativos abertos por meio do atalho ALT + TAB.

Gabarito: Letra A

8. (COVEST-COPSET / UFPE / 2015) Indique  a  alternativa  que  apresenta  exemplos  apenas  de sistemas operacionais:

a) Microsoft Word, Windows XP e Linux.
b) Mac Os X, Windows Explorer e MS DOS.
c) Linux, MS DOS e Microsoft Office.
d) Internet Explorer, Windows 7 e Microsoft PowerPoint.
e) Windows 98, Linux e Mac Os X.

Comentários:

Microsoft Word, Windows Explorer, Microsoft Office, Internet Explorer e Microsoft PowerPoint não são sistemas operacionais.

Gabarito: Letra E
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





76
102





9. (PR-4 / UFRJ / 2014) No Sistema Operacional Linux, o comando ls é utilizado para:

a) listar diretórios e arquivos b) listar aplicativos em execução c) excluir diretórios d) criar um diretório seguro.
e) criar um arquivo.

Comentários:

Trata-se de um comando que exibe o conteúdo de diretórios (ls = list source). Por ser o comando mais frequente em provas, vamos vê-lo com mais detalhes...

Conforme vimos em aula, trata-se do comando para listar diretórios e arquivos.

Gabarito: Letra A

10. (UFES / UFES / 2014) Softwares, assim como outras obras de esforço intelectual, como músicas e livros, são protegidos por direitos autorais (também conhecido como copyright). Para copiar e instalar um software em um computador, uma pessoa física ou uma empresa precisa seguir o que  consta  na  licença  daquele  software.  O  software que  pode  ser  obtido  gratuitamente  na internet e instalado em qualquer PC sem infração de direitos autorais é:

a) Microsoft Windows 7.
b) Microsoft Word 2013.
c) Microsoft Excel 2013.
d) Ubuntu Linux 12.04 LTS.
e) Microsoft Windows XP.


Comentários:


As  principais  distribuições  atualmente  são: Debian, Ubuntu, RedHat, Fedora, Suse, Mint, CentOS, Mandrake, Slackware, etc. Galera, existem – inclusive – distribuições brasileiras. As mais famosas são a Kurumin, Conectiva, Kalango e Mandriva.

Conforme vimos em aula, trata-se da única opção que apresenta uma distribuição do Linux.

Gabarito: Letra D

11. (CESGRANRIO  /  BB  /  2014) O  sistema  operacional  cujas  características  são  utilizar  código aberto e interface por linha de comando é o:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





77
102




a) Mac OS
b) iOS
c) Linux
d) Windows
e) Android

Comentários:

Até meados da década de 1980, o Unix ainda não possuía uma interface gráfica própria. Como assim, professor? Galera, vocês – assim como eu – são jovens, então vocês não sabem o que é um sistema operacional sem interface gráfica, somente com linha de comando!

Conforme vimos em aula, trata-se do Linux. Todo os outros são de proprietários – exceto o Android.
No  entanto,  sua  interface  por  linha  de  comando  está  restrita  aos  serviços  de  manutenção  e restauração do equipamento, configurada de fábrica em menus prontos.

Gabarito:
Letra C

12. (FUNCAB / IF-RR / 2013) Pode-se afirmar que o que diferencia o sistema operacional Linux do sistema operacional Windows é que o sistema Linux:

a) possui estrutura de arquivos e diretórios b) por concepção, seu código fonte é aberto.
c) possui controles de permissão de acesso, como Login e Logout.
d) gerencia software e hardware e) permite que o computador, no qual está instalado, conecte-se à rede.

Comentários:

Ao contrário de um software proprietário, ele é um software livre, cujo código-fonte está aberto e disponível sob a Licença GPL (Genereal Public License) para que o usuário possa ter acesso ao código-fonte com o intuito de utilizá-lo executá-lo, estudá-lo, modificá-lo e distribuí-lo livremente de acordo com os termos da licença. Ele é desenvolvido, em geral, por uma comunidade de programadores voluntários espalhados pelo mundo que contribuem para melhorá-lo.

Conforme vimos em aula, a única opção que diferencia esses sistemas operacionais é que o Linux é, por concepção, de código aberto.

Gabarito: Letra B

13. (UFES / UFES / 2013) Selecione a afirmativa correta:

a) Windows Mint, Debian e Ubuntu são exemplos de versões do Windows.
b) Linux e Excel são exemplos de programas de planilha eletrônica.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





78
102




c) Powerpoint e Impress são exemplos de navegadores da Internet.
d) Word e Writer são exemplos de editores de texto.
e)  Software  proprietário  é  qualquer  programa  de  computador  que  pode  ser  usado,  copiado, estudado e redistribuído sem nenhuma restrição.

Comentários:

(a)  Errado.  Todas  essas  são  distribuições  Linux;  (b)  Errado,  Linux  é  um  sistema  operacional;  (c) Errado, são exemplos de ferramentas de apresentação; (d) Correto, ambos são editores de texto;
(e) Errado. A questão trata dos softwares livres.

Gabarito: Letra D

14. (UEPA / PC-PA / 2013)  Quanto  aos  Sistemas  de  arquivos  utilizados  nos  diferentes  sistemas operacionais,  assinale  a  opção  que  preenche  corretamente  as  lacunas  do  texto  abaixo:
__________  e  __________  são  sistemas  de  arquivo  da plataforma  Windows,  enquanto  que _________ é um sistema de arquivo desenvolvido para o Linux. A alternativa correta é:

a) FAT32, NTFS, EXT2 b) NTFS, HFS, SWAP
c) EXT2, EXT3, SWAP
d) FAT32, JFS, EXT3
e) NTFS, JFS, Reiser.

Comentários:

O Sistema de Arquivos permite gravar, ler, localizar, remover e realizar funções em um dispositivo de armazenamento – em geral, um disco rígido. Galera, a maioria dos usuários Unix/Linux já foram ou ainda são usuários Windows. Nesse sistema operacional, existem basicamente três sistemas de arquivos: FAT16, FAT32 e NTFS.  No Linux, existem muito mais opções, tais como: EXT2, EXT3, EXT4, RaiserFS, etc. Vamos vê-los a seguir...

Conforme  vimos  em  aula,  FAT32  e  NTFS  são  sistemas  de  arquivo  da  plataforma  Windows, enquanto que EXT2 é um sistema de arquivo desenvolvido para o Linux.

Gabarito: Letra A

15. (COPEVE-UFAL / CASAL / 2010) Solaris, Linux e MacOS X são exemplos de:

a) software do tipo editor de texto.
b) software do tipo editor de planilha eletrônica.
c) hardware do tipo conversor de áudio e vídeo.
d) software do tipo sistema operacional.
e) software para edição de imagens.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





79
102





Comentários:

Todos esses são sistemas operacionais.

Gabarito: Letra D

16. (UFPEL / UFPEL / 2016) No ambiente do sistema operacional Ubuntu, a tecla de atalho utilizada para fechar a janela atual aberta é:

a) Alt + F1.
b) Ctrl + Z.
c) Ctrl + DEL.
d) Alt + F4.
e) Alt + Z.

Comentários:

Assim como no Sistema Operacional Windows, a tecla de atalho utilizada para fechar a janela atual aberta é o ALT + F4.

Gabarito:
Letra D

17.  (UFPEL / UFPEL / 2014) A respeito do sistema operacional Ubuntu, é correto afirmar que:

a) o pacote LibreOffice é o padrão de aplicativos de escritório no Ubuntu.

b) o Ubuntu só pode ser instalado em computadores que já possuam o Windows funcionando.

c) para que o Ubuntu funcione em um notebook, é obrigatório comprar uma licença exclusiva para esse tipo de computador.

d)  ainda  não  existe  software  de  apresentação  de  slides  semelhante  ao  Microsoft  PowerPoint para ser instalado e utilizado no Ubuntu.

e) o único navegador (browser) que funciona no Ubuntu é o Opera.

Comentários:

(a) Correto. O LibreOffice, assim como o Ubuntu, é livre e é o padrão de ferramentas de escritório;
(b) Errado. Você não precisa ter Windows nenhum funcionando para instalar o Ubuntu ou qualquer outra distribuição Linux; (c) Errado. Isso absolutamente não existe; (d) Errado. Existe, sim – ele se Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





80
102




chama  LibreOffice  Impress;  (e)  Errado.  Existe  diversos  outros  navegadores  que  funcionam  no Ubuntu, tais como Mozilla Firefox e Google Chrome.

Gabarito: Letra A

18. (UFPEL / UFPEL / 2013) Considere que, ao inserir um pen drive em um computador com sistema operacional  GNU/Linux  (Ubuntu  11.10),  o  dispositivo  seja  montado  automaticamente  pelo sistema. Esse dispositivo será montado, por padrão, dentro do seguinte diretório:

a) d:\
b) /usb/
c) /media/
d) e:\pendrive\
e) a:\usb

Comentários:

Galera, o pendrive é sempre montado dentro do diretório /media/.

Gabarito: Letra C

19. (UFPEL  /  UFPEL  /  2013)  Dentre  as  funcionalidades  oferecidas  pelo  prompt  de  comandos (terminal)  do  sistema  operacional  GNU/Linux  (Ubuntu  11.10),  qual  comando  de  terminal permite criar uma pasta/diretório?

a) mkdir
b) dodir
c) exdir
d) gedit
e) direx

Comentários:

O comando no Linux para a criação de pastas/diretórios é o mkdir (do inglês, make directory).

Gabarito:
Letra A

20.  (UFPEL / UFPEL / 2012) No Ubuntu 11.10, em uma instalação padrão, a combinação de teclas necessária para que a tela seja bloqueada é:

a) Ctrl+Alt+B
b) Ctrl+C
c) Ctrl+V
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





81
102




d) Ctrl+Alt+L
e) Ctrl+Shift+O

Comentários:

O comando utilizado para bloquear a tela no Ubuntu é o CTRL + ALT + L.

Gabarito: Letra D

21. (UFPEL / UFPEL / 2011) Em linux, usando o aplicativo “Terminal”, utilizado para a digitação de comandos, possuindo as permissões necessárias, o comando que lista arquivos, de forma longa, em ordem de data e hora de criação ou alteração e o comando que lista, de forma longa, em ordem de tamanho são, respectivamente, 
a) ls -lt e ls -lS.
b) ls -ld e ls -ll.
c) ls -lh e ls -lt.
d) ls -lS e ls -li.
e) ls -ll e ls -lJ.

Comentários:

Para  listar,  já  sabemos  que  se  utiliza  o  comando  ls;  para  listar  de  forma  longa,  utilizamos  o parâmetro
-l (lembre-se  de long);  para  listar  em  ordem  de  data  e  hora  de  criação  ou  alteração, utilizamos  o  parâmetro -t (lembre-se  de time);  para  listar  em  ordem  de  tamanho,  utilizamos  o parâmetro -S (lembre-se de size). Logo, trata-se do ls -lt e ls -lS.

Gabarito:
Letra A

22. (IDECAN / CBM DF - 2017) Considere as afirmativas sobre comandos no Sistema Operacional Linux.

I. ls é utilizado para exibir o conteúdo do arquivo.
II. pwd exibe o nome diretório corrente.
III. dl mostra o espaço em disco livre.

Está(ão) correta(s) apenas a(s) afirmativa(s) 
a) I.
b) II.
c) I e II.
d) II e III.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





82
102




Comentários:

ls: Trata-se de um comando que exibe o conteúdo de diretórios (ls = list source). Por ser o comando mais frequente em provas, vamos vê-lo com mais detalhes...
pwd: Mostra o caminho por inteiro do diretório atual, isto é, um pathname.

df: Este comando exibe informações sobre espaço livre e espaço usado nas partições do sistema.

Conforme vimos em aula, somente o comando do item II está correto. O erro do item I é afirmar que exibe o conteúdo do arquivo, enquanto exibe o conteúdo do diretório; e o erro do item III é que não existe o comando dl e o correto é o df.

Gabarito: Letra B

23. (IDECAN / CBM DF - 2017) Utilizando um Sistema Operacional de ambiente Linux, um usuário digitou o comando chmod 755 concurso.txt no terminal de comandos.

Sobre o comando em questão, está INCORRETO afirmar que 
a) serão negadas todas permissões ao dono.
b) será atribuída permissão de leitura para o grupo.
c) será atribuída permissão de execução para o grupo.
d) será atribuída permissão de leitura e execução para outros usuários.

Comentários:

Trata-se do comando que permite alterar permissões de acesso de objetos do sistema (arquivos e diretórios) – chmod vem de change mode.

Conforme vimos em aula, o chmod serve para alterar permissões de acesso aos usuários. O acesso do dono não é alterado com o uso desse comando. Assim, como a questão pede a opção incorreta, temos a alternativa A.

Gabarito: Letra A

24. (IDECAN / CBM DF - 2017) Um usuário utiliza Sistemas Operacionais de ambiente Linux para realizar as suas atividades diárias. A fim de utilizar um driver de CD-ROM foi necessário realizar a montagem do dispositivo que por padrão ficou armazenado no diretório:

a) /etc.
b) /bin.
c) /mnt.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





83
102




d) /pwd.

Comentários:

/mnt

Trata-se  do  diretório  em  que  os  administradores  de sistema  montam  sistemas  de  arquivos temporários  enquanto  os  utilizam.  Por  exemplo:  se  você  estiver  montando  uma  partição  do Windows para executar algumas operações de recuperação de arquivos, você pode montá-lo em  /mnt/windows.  No  entanto,  você  pode  montar  outros  sistemas  de  arquivos  em  qualquer lugar no sistema.


Conforme vimos em aula, trata-se da alternativa C.

Gabarito: Letra C

25. (IDECAN  /  CBM  DF  -  2017)  Considere  as  afirmativas  sobre  a  utilização  de  comandos  nos sistemas operacionais de ambiente Linux.

I. O comando search é utilizado para localizar arquivos.
II. O comando dir é utilizado para listar o conteúdo de um diretório.
III. O comando rm é utilizado para excluir arquivos.

Está(ão) correta(s) apenas a(s) afirmativa(s) 
a) I.
b) II.
c)
III.
d) II e III.

Comentários:

O comando find localiza arquivos para pesquisa de arquivos de texto do diretório atual.
O Linux e Windows possuem comandos diferentes para executar uma mesma tarefa? Sim, um exemplo clássico são os comandos ls e dir – que fazem a mesma coisa!
O comando ls é um comando que exibe o conteúdo de diretórios (ls = list source). Por ser o comando mais frequente em provas, vamos vê-lo com mais detalhes...
O comando rm remove arquivos. É uma forma curta de se referir a remove (remover).

Conforme vimos em aula, trata-se da opção D. O comando search não existe, o comando correto para localizar arquivos é o find.

Gabarito:
Letra D

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





84
102




26. (IDECAN / CBM DF - 2017)  Sobre  diretórios  nos  Sistemas  Operacionais  de  ambiente  Linux, analise as afirmativas a seguir.

I. Os arquivos dos usuários são armazenados no diretório /home.
II. Os arquivos temporários criados pelos programas são armazenados no diretório /usr.
III.  As  bibliotecas  compartilhadas  pelos  programas  do sistema  e  módulos  do  kernel  são armazenadas no diretório /dev.

Está(ão) correta(s) apenas a(s) afirmativa(s) 

a) I.
b) II.
c) III.
d)
I e II.

Comentários:

DIRETÓRIO DESCRIÇÃO
/home
Trata-se  do  diretório  onde  encontramos  um  arquivo  para  cada  usuário  existente  no  sistema.
Sempre  que  adicionamos  um  novo  usuário,  por  exemplo,  com o  nome  profdiego2  no  diretório /home, é criado um arquivo para este usuário como /home/profdiego2/. Dentro desse diretório, ficam  todos  os  arquivos de  configurações  específicas  para  aquele  usuário, bem  como  todos os seus arquivos de dados.
/tmp
Trata-se do diretório onde encontramos os arquivos temporários do sistema. Estes arquivos são normalmente gerados pelo sistema e, como o nome indica, permanecem no sistema durante um período  limitado  de  tempo.  Por  exemplo:  sempre  que instalamos  um  programa,  este  utiliza  o diretório  /tmp/  para  colocar  arquivos  que serão  necessários  durante  a  instalação,  mas  que  não voltarão a ser necessários.
/dev
Trata-se do diretório onde ficam arquivos especiais associados aos dispositivos do sistema. Estes ficheiros  são  especiais  porque  representam  os  dispositivos  do  sistema.  Por  exemplo:  um  disco rígido do sistema aparecerá como /dev/sda.
/lib
Trata-se do diretório onde estão armazenadas as bibliotecas compartilhadas no sistema. Estas bibliotecas  podem  variar  de  acordo  com  a  distribuição  utilizada  e  podem  ser,  por  exemplo, bibliotecas  de  linguagens  como  Perl,  Python,  C,  etc.  É  também  neste  diretório  que  estão  os módulos do Kernel do Sistema Operacional.

Conforme vimos em aula, somente a primeira alternativa está correta. O item II descreve o diretório /tmp e o item III traz uma definição do diretório /lib.

Gabarito: Letra A

27. (IDECAN / UERN - 2016) Muitas empresas estão optando por utilizarem o Sistema Operacional Linux.  A  grande  vantagem  desse  Sistema  é  que  não  se  tem a  necessidade  de  pagamento  de licença para utilizá-lo, diferente dos sistemas proprietários, da Microsoft, por exemplo, que se deve pagar uma licença para utilização. Por não ter que pagar licença, as empresas economizam Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





85
102




e podem investir em equipamentos, infraestrutura, entre outros. Trabalhar com Linux já é uma realidade, e muitas ações são feitas utilizando-se do terminal, ou seja, usam-se os comandos pela  linha  de  comando  do Linux.  Diferente  do Windows,  onde  quase  tudo  é  feito  através  da interface gráfica, no Linux os comandos podem ser usados pela linha de comando e, em algumas versões, fazendo uso de interface gráfica. “Suponha que se esteja editando um arquivo na linha de  comandos  do Linux,  mas  tenha  se  esquecido  o  diretório  em  que  se  encontra.  Um  desses comandos pode ser usado para a verificação de qual diretório se encontra (isso em caso do seu aviso de comandos não mostrar essa informação)”. Assinale a alternativa correta que apresenta este comando.


a) ls.
b) cd.
c) pwd.
d) mkdir.

Comentários:

COMANDO DESCRIÇÃO
pwd Mostra o caminho por inteiro do diretório atual, isto é, um pathname.

Conforme vimos em aula, trata-se do comando pwd.

Gabarito:
Letra C

28. (IDECAN / UERN - 2016) Sobre comandos utilizados em Sistemas Operacionais Linux, marque V para as afirmativas verdadeiras e F para as falsas.


( ) O comando ls é utilizado para listar todos os arquivos do diretório.
( ) O comando addir é utilizado para criar um novo diretório.
( ) O comando
chmod modifica as permissões de um arquivo ou diretório.
( ) O comando dir exibe o caminho completo do diretório atual.

a) V, V, F, F.
b) V, F, V, F.
c) F, V, V, F.
d) F, F, V, V.

Comentários:

ls: comando que exibe o conteúdo de diretórios (ls = list source). (V) 
mkdir: cria um diretório. (F) 
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





86
102




chmod:  comando que permite alterar permissões de acesso de objetos do sistema (arquivos e diretórios) – chmod vem de change mode. (V) 
Pwd: mostra o caminho por inteiro do diretório atual, isto é, um pathname. (F) 
Conforme vimos em aula, a alternativa correta e a letra B: V, F, V, F.

Gabarito: Letra B

29. (IDECAN / UERN - 2016) Organizar arquivos e pastas (diretórios) é uma tarefa muito importante para os usuários do computador. Seja com qual Sistema Operacional se está trabalhando, com essa  organização  fica  muito  mais  fácil  encontrar  aquilo  que  se  deseja  no  computador.  “No Sistema Operacional Linux há um comando que efetua uma procura por arquivos/diretórios no disco. Essa busca pode ser feita considerando-se critérios como: data de modificação, tamanho etc.,  usando  algumas  opções  com  o  comando.  Sua  sintaxe  padrão  é: comando  [diretório] [opções/expressão]. Neste caso, indica que a busca será realizada neste diretório, percorrendo seus subdiretórios.” Assinale a alternativa referente a este comando.


a) tail.
b) less.
c) find.
d) sort.

Comentários:

COMANDO DESCRIÇÃO
find Localiza arquivos para pesquisa de arquivos de texto do diretório atual.

Conforme vimos em aula, trata-se do comando find.

Gabarito:
Letra C

30. (IDECAN / AGU - 2014) Sistemas Operacionais Linux são programas responsáveis por promover o funcionamento do computador, realizando a comunicação entre os dispositivos de hardware e softwares. Em relação a este sistema, é correto afirmar que KDE e GNOME são 
a) versões de Kernel.
b) distribuições Linux.
c) ambientes gráficos.
d) editores de texto Linux.
e) terminais para execução de comandos.

Comentários:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





87
102





KDE é um ambiente gráfico multiplataforma mais similar ao Windows, portanto é o mais comum quando se migra do Windows para o Linux.

GNOME é um projeto de software livre abrangendo o ambiente gráfico para os usuários e os desenvolvedores.

Conforme vimos em aula, o KDE e o GNOME são ambientes gráficos.

Gabarito: Letra C

31. (IDECAN / BANESTES - 2012) Nos computadores de hoje, facilmente pode-se ter dois sistemas operacionais  instalados,  sendo  que  a  inicialização apresenta  a  opção  de  escolher  o  Sistema Operacional para iniciar a máquina. Esse processo denomina-se Dual Boot. O Linux utiliza um gerenciador   de  inicialização,   o   que   facilita   ter   máquina   em Dual  Boot.   Identifique   os gerenciadores de inicialização mais utilizados no mundo Linux.


a) LILO e GRUB.
b) MBR e LILO.
c) GRUB e MBR.
d) BIOS e GRUB.
e) LILO e BIOS.

Comentários:

O LILO (LInux LOader) é o gerenciador de inicialização mais antigo – ele tem uma interface mais simples e rústica.
O GRUB (GRand Unified Bootloader) é um gerenciador de inicialização mais recente – é mais bonito e moderno que o anterior.

Conforme vimos em aula, o LILO e o GRUB são gerenciadores de inicialização.

Gabarito:
Letra A

32. (IDECAN / BANESTES - 2012) Sobre os diretórios encontrados nos Sistemas Linux, relacione corretamente as colunas.

1. bin ( ) Bibliotecas.
2. dev ( ) Diretório de usuários.
3. etc ( ) Programas binários (executáveis).
4. lib ( ) Arquivos especiais para dispositivos E/S.
5. usr ( ) Arquivos diversos do sistema.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





88
102




a) 3, 4, 2, 1, 5
b) 4, 5, 1, 2, 3
c) 1, 3, 4, 5, 2
d) 2, 1, 3, 4, 5
e) 5, 2, 1, 3, 4

Comentários:

DIRETÓRIO DESCRIÇÃO
/bin

O /bin é o diretório onde ficam guardados arquivos binários que têm de estar acessíveis a todos os utilizadores do sistema. Estes arquivos binários são programas que o próprio sistema inicia de forma autónoma.
/dev

Trata-se  do  diretório  onde  ficam  arquivos  especiais  associados  aos  dispositivos  do  sistema.
Estes ficheiros são especiais porque representam os dispositivos do sistema. Por exemplo: um disco rígido do sistema aparecerá como /dev/sda.
/etc

Trata-se do diretório onde se encontram todos os arquivos globais de configuração do sistema.
Na sua grande maioria, estes arquivos podem ser editados com o uso de um simples editor de texto. Repare que neste diretório encontram-se arquivos de configuração do sistema e, não, de um usuário específico. Os arquivos de configuração de um usuário específico encontram-se no diretório home de cada utilizador.
/lib

Trata-se do diretório onde estão armazenadas as bibliotecas compartilhadas no sistema. Estas bibliotecas  podem  variar  de  acordo  com  a  distribuição  utilizada  e  podem  ser,  por  exemplo, bibliotecas  de  linguagens  como  Perl,  Python,  C,  etc.  É  também  neste  diretório  que  estão  os módulos do Kernel do Sistema Operacional.
/usr

Trata-se do diretório onde estão arquivos e programas utilizados pelos usuários existentes no sistema.  No  caso dos  programas,  no  diretório /usr/bin  ficam  todas as aplicações  que  não  são essenciais ao sistema e, por conseguinte, não se encontram no diretório /sbin ou /bin . No caso dos programas que ficam no diretório /usr/bin, as bibliotecas associadas a estes sistemas ficam localizadas no diretório /usr/lib.


Galera, associando os diretórios apresentados às pequenas descrições, chegamos à alternativa B.

Gabarito: Letra B

33. (AOCP / EBSERH - 2017) Em um sistema Unix-like, qual comando apresenta os processos em execução atualizando em tela?

a) jobs
b) pstree
c) top
d) ps
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





89
102




e) ps ax.

Comentários:

(a)  Errado,  esse  comando  verifica  detalhes  sobre  jobs  em  execução;  (b)  Errado,  esse  comando permite exibir uma lista hierárquica de processos no formato de árvore; (c) Correto, esse comando mostra o uso da memória; (d) Errado, esse comando gera um instantâneo dos processos atuais no terminal e permite mostrar informações sobre uma seleção dos processos ativos; (e) Errado, esse comando mostra todos os processos.

Gabarito: Letra C

34. (AOCP / FUNDASUS / 2015) Considerando o Sistema Operacional LINUX, o “nome do login” do superusuário padrão é:

a) root.
b) super.
c) usu.
d) master.
e) primary.

Comentários:

Root
é a designação de um tipo de usuário de computador que tem acesso irrestrito aos arquivos e processos  de  sistemas  operacionais  baseados  em  Unix  –  também  conhecido  como  superusuário padrão.

Gabarito: Letra A

35. (AOCP / UFPEL / 2015) Sobre o Linux, qual é o comando para confirmar a data e hora atual do sistema?

a) Time.
b) Date.
c) Hora.
d) Cat.
e) Type.


Comentários:

(a) Errado, esse comando mede o tempo de execução de programas; (b) Correto, esse atalho exibe data e hora atual do sistema; (c) Errado, esse comando não existe; (d) Errado, esse comando mostra Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





90
102




o conteúdo de um arquivo e é utilizado para concatenar arquivos de texto. Detalhe: o comando cat é equivalente o comando type do Windows.

Gabarito: Letra B

36. (AOCP / EBSERH / 2015) Qual é a maior diferença entre o Libre Office e o Microsoft Office?

a) O Código do Microsoft Office é aberto, e o Libre não tem código aberto.
b) O programa Impress do Libre é equivalente ao Publisher do Microsoft Office.
c) Libre não possui um editor de texto, e o Microsoft Office possui (Microsoft World).
d)  Libre  Office,  programa  ou  software  livre  (gratuito),  e  o  Microsoft  Office,  programa  ou software pago.
e) No Libre, o programa para montar planilhas chama-se CALC e, no Microsoft, chama-se Power Point

Comentários:

(a) Errado, a questão inverteu os conceitos; (b) Errado, ele é equivalente ao Microsoft Powerpoint do Microsoft Office; (c) Errado, o LibreOffice possui um editor de texto chamado Writer e o editor de texto do Office se chama Microsoft Word e, não, Microsoft World; (d) Correto, ele é um software livre e gratuito enquanto o Microsoft Office é um software pago; (e) Errado, o programa para montar planilhas da Microsoft é o MS-Excel.

Gabarito: Letra D

37. (AOCP / EBSERH / 2015) Quais são as vantagens do Libre Office?

a)  Software  pago,  Código  aberto,  Multiplataforma,  Extenso  suporte  a  idiomas,  Interface  de usuários    consistente,    Integração,    Granulidade,    Compatibilidade    com    arquivos,    sem dependência do fornecedor.

b)    Sem  taxas  de  licenciamento,  Código  aberto,  Monoplataforma  (funciona  somente  no Windows),   Extenso   suporte   a   idiomas,   Interface   de   usuários   consistente,   Integração, Granulidade, Compatibilidade com arquivos, sem dependência do fornecedor.

c) Sem taxas de licenciamento, Código Fechado, Multiplataforma, Extenso suporte a idiomas, Interface de usuários consistente, Integração, Granulidade, Compatibilidade com arquivos, sem dependência do fornecedor.

d) Poucas taxas de licenciamento, Código aberto, Multiplataforma, Extenso suporte a idiomas, Interface de usuários consistente, Integração, Granulidade.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





91
102




e)  Sem  taxas  de  licenciamento,  Código  aberto,  Multiplataforma,  Extenso  suporte  a  idiomas, Interface de usuários consistente, Integração, Granulidade, Compatibilidade com arquivos, sem dependência do fornecedor.

Comentários:

(a) Errado, ele não é pago – é gratuito; (b) Errado, ele é multiplataforma – funciona em diversos sistemas operacionais; (c) Errado, ele tem código aberto; (d) Errado, não tem taxas de licenciamento;
(e) Correto, ele não possui taxas de licenciamento, tem código aberto, é multiplataforma, entre outras características.

Gabarito: Letra E

38. (AOCP  /  EBSERH  /  2015) Sobre  atalhos  do  programa  Libre  Office,  assinale  a alternativa INCORRETA.

Obs: A tecla + significa a junção de uma tecla com uma letra ou outra tecla.

a) CTRL + X – Corta os itens Selecionados.
b) CTRL + V – Cola os itens copiados ou cortados da área de transferência.
c) SHIFT + F – Procura o termo de pesquisa inserido pela última vez.
d) CTRL + Z – Desfaz a última ação.
e) CTRL + Y – Refaz a última ação.


Comentários:

(a) Correto, esse atalho realmente corta os itens selecionados; (b) Correto, esse atalho realmente cola os itens copiados ou cortados da área de transferência; (c) Errado, o atalho correto para realizar essa função é o CTRL+SHIFT+F; (d) Correto, esse atalho realmente desfaz a última ação; (e) Correto, esse atalho realmente refaz a última ação.

Gabarito: Letra C




LISTA DE EXERCÍCIOS – DIVERSAS BANCAS 
1. (COVEST-COPSET  /  UFPE  /  2013)  No  sistema  operacional  Linux,  a  interface  de  linha  de comando semelhante ao Prompt de comando do sistema Windows é conhecida como:


a) prompt.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





92
102




b) boot.
c) shell.
d) gui.
e) Xwindow.

2. (UFCG / UFCG/ 2016) No ambiente Linux, o comando $ ls:

a) Mostra a quantidade de espaço usada no disco rígido.
b) Mostra o uso da memória.
c) Lista todos os arquivos do diretório.
d) Abre um arquivo.
e) Abre o explorador de informações.

3. (IBADE / SEDUC-RO / 2016) Um sistema operacional pode ser definido como um conjunto de programas  especialmente  feitos  para  a  execução  de  várias  tarefas,  entre  as  quais  servir  de intermediário entre o utilizador e o computador. Um sistema operacional tem também como função  gerir  todos  os  periféricos  de  um  computador.  Analise  as  afirmativas  abaixo  sobre  os sistemas operacionais Linux e Windows.

I. O Windows é o software livre mais comumente encontrado nos computadores, ao contrário do Linux que se configura como um software proprietário.
II. Ambos os sistemas operacionais são multiusuários.
III.  No  ambiente  Windows,  não  é  possível  manter  duas  ou  mais  versões  do  mesmo  arquivo armazenadas em locais diferentes.

Está correta apenas o que se afirma em:

a) I.
b) II.
c) III.
d) I e III.
e) I e II.


4. (COPESE - UFPI / Pref. de Bom Jesus – PI / 2015)  Sobre  sistemas  operacionais  (Windows  e Linux) assinale a opção CORRETA.

a) Os sistemas operacionais utilizam sempre o mesmo sistema de arquivos, no caso o chamado NTFS.

b)  Os  programas  desenvolvidos  para  Linux  funcionam normalmente,  sem  necessitar  de adaptações no Windows e vice-versa.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





93
102




c)  O  sistema  operacional  é  um  software  cuja  função é  gerenciar  os  recursos  do  sistema, fornecendo  uma interface  entre  o  computador  e  o  usuário  e  fornecendo  suporte para  que  os demais programas possam funcionar.

d) Firefox e Chrome são exemplos de sistemas operacionais.

e)  A  multitarefa  é  um  recurso  do  sistema  operacional  que  permite  ele  seja  executado  em máquinas diferentes.

5. (IBFC  /  EMBASA  /  2015)  Quanto  as  características  dos  Sistemas  Operacionais,  analise  as afirmativas abaixo, dê valores Verdadeiro (V) ou Falso (F) e assinale a alternativa que apresenta a sequência correta (de cima para baixo):

( ) 0 Windows é considerado um Sistema Operacional proprietário.
( ) O Linux somente funciona com processadores da Intel.

a) V - V
b) V - F
c) F - V
d) F - F.

6. (COPESE - UFPI / UFPI / 2015) Assinale a opção que corresponde a um sistema operacional cujo código fonte está disponível sob a licença GPL (General Public License – Licença Pública Geral) para que qualquer pessoa o possa utilizar, estudar, modificar e distribuir livremente de acordo com os termos da licença.

a) Windows XP.
b) Windows Vista.
c) Linux.
d) Word 2010.
e) BrOffice.

7. (Pref. do RJ / CM do RJ / 2015) Da mesma forma que no Windows 7 e 8, o Ubuntu Linux 13.04 disponibiliza diversos atalhos de teclado para uso. Neste contexto, um deles deve ser utilizado para  alternar  o  acesso  entre  aplicativos  abertos  e em  execução  de  forma  concorrente.  Esse atalho é:

a) Alt + Tab
b) Alt + Home
c) Super + Tab
d) Super + Home.

8. (COVEST-COPSET / UFPE / 2015) Indique  a  alternativa  que  apresenta  exemplos  apenas  de sistemas operacionais:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





94
102





a) Microsoft Word, Windows XP e Linux.
b) Mac Os X, Windows Explorer e MS DOS.
c) Linux, MS DOS e Microsoft Office.
d) Internet Explorer, Windows 7 e Microsoft PowerPoint.
e) Windows 98, Linux e Mac Os X.

9. (PR-4 / UFRJ / 2014) No Sistema Operacional Linux, o comando ls é utilizado para:

a) listar diretórios e arquivos b) listar aplicativos em execução c) excluir diretórios d) criar um diretório seguro.
e) criar um arquivo.

10. (UFES / UFES / 2014) Softwares, assim como outras obras de esforço intelectual, como músicas e livros, são protegidos por direitos autorais (também conhecido como copyright). Para copiar e instalar um software em um computador, uma pessoa física ou uma empresa precisa seguir o que  consta  na  licença  daquele  software.  O  software que  pode  ser  obtido  gratuitamente  na internet e instalado em qualquer PC sem infração de direitos autorais é:

a) Microsoft Windows 7.
b) Microsoft Word 2013.
c) Microsoft Excel 2013.
d) Ubuntu Linux 12.04 LTS.
e) Microsoft Windows XP.


11. (CESGRANRIO  /  BB  /  2014)  O  sistema  operacional  cujas  características  são  utilizar  código aberto e interface por linha de comando é o:

a) Mac OS
b) iOS
c) Linux
d) Windows
e) Android

12. (FUNCAB / IF-RR / 2013) Pode-se afirmar que o que diferencia o sistema operacional Linux do sistema operacional Windows é que o sistema Linux:

a) possui estrutura de arquivos e diretórios b) por concepção, seu código fonte é aberto.
c) possui controles de permissão de acesso, como Login e Logout.
d) gerencia software e hardware e) permite que o computador, no qual está instalado, conecte-se à rede.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





95
102





13. (UFES / UFES / 2013) Selecione a afirmativa correta:

a) Windows Mint, Debian e Ubuntu são exemplos de versões do Windows.
b) Linux e Excel são exemplos de programas de planilha eletrônica.
c) Powerpoint e Impress são exemplos de navegadores da Internet.
d) Word e Writer são exemplos de editores de texto.
e)  Software  proprietário  é  qualquer  programa  de  computador  que  pode  ser  usado,  copiado, estudado e redistribuído sem nenhuma restrição.

14. (UEPA / PC-PA / 2013)  Quanto  aos  Sistemas  de  arquivos  utilizados  nos  diferentes  sistemas operacionais,  assinale  a  opção  que  preenche  corretamente  as  lacunas  do  texto  abaixo:
__________  e  __________  são  sistemas  de  arquivo  da plataforma  Windows,  enquanto  que _________ é um sistema de arquivo desenvolvido para o Linux. A alternativa correta é:

a) FAT32, NTFS, EXT2 b) NTFS, HFS, SWAP
c) EXT2, EXT3, SWAP
d) FAT32, JFS, EXT3
e) NTFS, JFS, Reiser.

15. (COPEVE-UFAL / CASAL / 2010) Solaris, Linux e MacOS X são exemplos de:

a) software do tipo editor de texto.
b) software do tipo editor de planilha eletrônica.
c) hardware do tipo conversor de áudio e vídeo.
d) software do tipo sistema operacional.
e) software para edição de imagens.

16. (UFPEL / UFPEL / 2016) No ambiente do sistema operacional Ubuntu, a tecla de atalho utilizada para fechar a janela atual aberta é:


a) Alt + F1.
b) Ctrl + Z.
c) Ctrl + DEL.
d) Alt + F4.
e) Alt + Z.

17. (UFPEL / UFPEL / 2014) A respeito do sistema operacional Ubuntu, é correto afirmar que:

a) o pacote LibreOffice é o padrão de aplicativos de escritório no Ubuntu.

b) o Ubuntu só pode ser instalado em computadores que já possuam o Windows funcionando.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





96
102




c) para que o Ubuntu funcione em um notebook, é obrigatório comprar uma licença exclusiva para esse tipo de computador.

d)  ainda  não  existe  software  de  apresentação  de  slides  semelhante  ao  Microsoft  PowerPoint para ser instalado e utilizado no Ubuntu.

e) o único navegador (browser) que funciona no Ubuntu é o Opera.

18. (UFPEL / UFPEL / 2013) Considere que, ao inserir um pen drive em um computador com sistema operacional  GNU/Linux  (Ubuntu  11.10),  o  dispositivo  seja  montado  automaticamente  pelo sistema. Esse dispositivo será montado, por padrão, dentro do seguinte diretório:

a) d:\
b) /usb/
c) /media/
d) e:\pendrive\
e) a:\usb

19. (UFPEL  /  UFPEL  /  2013)  Dentre  as  funcionalidades  oferecidas  pelo  prompt  de  comandos (terminal)  do  sistema  operacional  GNU/Linux  (Ubuntu  11.10),  qual  comando  de  terminal permite criar uma pasta/diretório?

a) mkdir
b) dodir
c) exdir
d) gedit
e) direx

20.  (UFPEL / UFPEL / 2012) No Ubuntu 11.10, em uma instalação padrão, a combinação de teclas necessária para que a tela seja bloqueada é:

a) Ctrl+Alt+B
b) Ctrl+C
c) Ctrl+V
d) Ctrl+Alt+L
e) Ctrl+Shift+O

21. (UFPEL / UFPEL / 2011) Em linux, usando o aplicativo “Terminal”, utilizado para a digitação de comandos, possuindo as permissões necessárias, o comando que lista arquivos, de forma longa, em ordem de data e hora de criação ou alteração e o comando que lista, de forma longa, em ordem de tamanho são, respectivamente, 
a) ls -lt e ls -lS.
b) ls -ld e ls -ll.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





97
102




c) ls -lh e ls -lt.
d) ls -lS e ls -li.
e) ls -ll e ls -lJ.

22. (IDECAN / CBM DF - 2017) Considere as afirmativas sobre comandos no Sistema Operacional Linux.

I. ls é utilizado para exibir o conteúdo do arquivo.
II. pwd exibe o nome diretório corrente.
III. dl
mostra o espaço em disco livre.

Está(ão) correta(s) apenas a(s) afirmativa(s) 
a)
I.
b) II.
c) I e II.
d) II e III.

23. (IDECAN / CBM DF - 2017) Utilizando um Sistema Operacional de ambiente Linux, um usuário digitou o comando chmod 755 concurso.txt no terminal de comandos.

Sobre o comando em questão, está INCORRETO afirmar que 
a) serão negadas todas permissões ao dono.
b) será atribuída permissão de leitura para o grupo.
c) será atribuída permissão de execução para o grupo.
d) será atribuída permissão de leitura e execução para outros usuários.

24. (IDECAN / CBM DF - 2017) Um usuário utiliza Sistemas Operacionais de ambiente Linux para realizar as suas atividades diárias. A fim de utilizar um driver de CD-ROM foi necessário realizar a montagem do dispositivo que por padrão ficou armazenado no diretório:

a) /etc.
b) /bin.
c) /mnt.
d) /pwd.

25. (IDECAN  /  CBM  DF  -  2017)  Considere  as  afirmativas  sobre  a  utilização  de  comandos  nos sistemas operacionais de ambiente Linux.

I. O comando search é utilizado para localizar arquivos.
II. O comando dir é utilizado para listar o conteúdo de um diretório.
III. O comando rm é utilizado para excluir arquivos.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





98
102




Está(ão) correta(s) apenas a(s) afirmativa(s) 
a) I.
b) II.
c) III.
d) II e III.

26. (IDECAN / CBM DF - 2017)  Sobre  diretórios  nos  Sistemas  Operacionais  de  ambiente  Linux, analise as afirmativas a seguir.

I. Os arquivos dos usuários são armazenados no diretório /home.
II. Os arquivos temporários criados pelos programas são armazenados no diretório /usr.
III.  As  bibliotecas  compartilhadas  pelos  programas  do sistema  e  módulos  do  kernel  são armazenadas no diretório /dev.

Está(ão) correta(s) apenas a(s) afirmativa(s) 

a) I.
b)
II.
c) III.
d) I e II.

27. (IDECAN / UERN - 2016) Muitas empresas estão optando por utilizarem o Sistema Operacional Linux.  A  grande  vantagem  desse  Sistema  é  que  não  se  tem a  necessidade  de  pagamento  de licença para utilizá-lo, diferente dos sistemas proprietários, da Microsoft, por exemplo, que se deve pagar uma licença para utilização. Por não ter que pagar licença, as empresas economizam e podem investir em equipamentos, infraestrutura, entre outros. Trabalhar com Linux já é uma realidade, e muitas ações são feitas utilizando-se do terminal, ou seja, usam-se os comandos pela  linha  de  comando  do Linux.  Diferente  do Windows,  onde  quase  tudo  é  feito  através  da interface gráfica, no Linux os comandos podem ser usados pela linha de comando e, em algumas versões, fazendo uso de interface gráfica. “Suponha que se esteja editando um arquivo na linha de  comandos  do Linux,  mas  tenha  se  esquecido  o  diretório  em  que  se  encontra.  Um  desses comandos pode ser usado para a verificação de qual diretório se encontra (isso em caso do seu aviso de comandos não mostrar essa informação)”. Assinale a alternativa correta que apresenta este comando.


a) ls.
b) cd.
c) pwd.
d) mkdir.

28. (IDECAN / UERN - 2016) Sobre comandos utilizados em Sistemas Operacionais Linux, marque V para as afirmativas verdadeiras e F para as falsas.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





99
102




( ) O comando ls é utilizado para listar todos os arquivos do diretório.
( ) O comando addir é utilizado para criar um novo diretório.
( ) O comando
chmod modifica as permissões de um arquivo ou diretório.
( ) O comando dir exibe o caminho completo do diretório atual.

a) V, V, F, F.
b) V, F, V, F.
c) F, V, V, F.
d) F, F, V, V.

29. (IDECAN / UERN - 2016) Organizar arquivos e pastas (diretórios) é uma tarefa muito importante para os usuários do computador. Seja com qual Sistema Operacional se está trabalhando, com essa  organização  fica  muito  mais  fácil  encontrar  aquilo  que  se  deseja  no  computador.  “No Sistema Operacional Linux há um comando que efetua uma procura por arquivos/diretórios no disco. Essa busca pode ser feita considerando-se critérios como: data de modificação, tamanho etc.,  usando  algumas  opções  com  o  comando.  Sua  sintaxe  padrão  é: comando  [diretório] [opções/expressão]. Neste caso, indica que a busca será realizada neste diretório, percorrendo seus subdiretórios.” Assinale a alternativa referente a este comando.


a) tail.
b) less.
c) find.
d) sort.

30.  (IDECAN / AGU - 2014) Sistemas Operacionais Linux são programas responsáveis por promover o funcionamento do computador, realizando a comunicação entre os dispositivos de hardware e softwares. Em relação a este sistema, é correto afirmar que KDE e GNOME são 

a) versões de Kernel.
b) distribuições Linux.
c) ambientes gráficos.
d) editores de texto Linux.
e) terminais para execução de comandos.

31. (IDECAN / BANESTES - 2012) Nos computadores de hoje, facilmente pode-se ter dois sistemas operacionais  instalados,  sendo  que  a  inicialização apresenta  a  opção  de  escolher  o  Sistema Operacional para iniciar a máquina. Esse processo denomina-se Dual Boot. O Linux utiliza um gerenciador   de  inicialização,   o   que   facilita   ter   máquina   em Dual  Boot.   Identifique   os gerenciadores de inicialização mais utilizados no mundo Linux.

a) LILO e GRUB.
b) MBR e LILO.
c) GRUB e MBR.
d) BIOS e GRUB.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





100
102




e) LILO e BIOS.

32. (IDECAN / BANESTES - 2012) Sobre os diretórios encontrados nos Sistemas Linux, relacione corretamente as colunas.

1. bin ( ) Bibliotecas.
2. dev ( ) Diretório de usuários.
3. etc ( ) Programas binários (executáveis).
4. lib ( ) Arquivos especiais para dispositivos E/S.
5. usr ( ) Arquivos diversos do sistema.

a) 3, 4, 2, 1, 5
b) 4, 5, 1, 2, 3
c) 1, 3, 4, 5, 2
d) 2, 1, 3, 4, 5
e) 5, 2, 1, 3, 4

33. (AOCP / EBSERH - 2017) Em um sistema Unix-like, qual comando apresenta os processos em execução atualizando em tela?

a) jobs
b) pstree
c) top
d) ps
e) ps ax.

34. (AOCP / FUNDASUS / 2015) Considerando o Sistema Operacional LINUX, o “nome do login” do superusuário padrão é:

a) root.
b) super.
c) usu.
d) master.
e) primary.


35. (AOCP / UFPEL / 2015) Sobre o Linux, qual é o comando para confirmar a data e hora atual do sistema?

a) Time.
b) Date.
c) Hora.
d) Cat.
e) Type.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





101
102




36. (AOCP / EBSERH / 2015) Qual é a maior diferença entre o Libre Office e o Microsoft Office?

a) O Código do Microsoft Office é aberto, e o Libre não tem código aberto.
b) O programa Impress do Libre é equivalente ao Publisher do Microsoft Office.
c) Libre não possui um editor de texto, e o Microsoft Office possui (Microsoft World).
d)  Libre  Office,  programa  ou  software  livre  (gratuito),  e  o  Microsoft  Office,  programa  ou software pago.
e) No Libre, o programa para montar planilhas chama-se CALC e, no Microsoft, chama-se Power Point

37. (AOCP / EBSERH / 2015) Quais são as vantagens do Libre Office?

a)  Software  pago,  Código  aberto,  Multiplataforma,  Extenso  suporte  a  idiomas,  Interface  de usuários    consistente,    Integração,    Granulidade,    Compatibilidade    com    arquivos,    sem dependência do fornecedor.

b)    Sem  taxas  de  licenciamento,  Código  aberto,  Monoplataforma  (funciona  somente  no Windows),   Extenso   suporte   a   idiomas,   Interface   de   usuários   consistente,   Integração, Granulidade, Compatibilidade com arquivos, sem dependência do fornecedor.

c) Sem taxas de licenciamento, Código Fechado, Multiplataforma, Extenso suporte a idiomas, Interface de usuários consistente, Integração, Granulidade, Compatibilidade com arquivos, sem dependência do fornecedor.

d) Poucas taxas de licenciamento, Código aberto, Multiplataforma, Extenso suporte a idiomas, Interface de usuários consistente, Integração, Granulidade.

e)  Sem  taxas  de  licenciamento,  Código  aberto,  Multiplataforma,  Extenso  suporte  a  idiomas, Interface de usuários consistente, Integração, Granulidade, Compatibilidade com arquivos, sem dependência do fornecedor.

38. (AOCP  /  EBSERH  /  2015) Sobre  atalhos  do  programa  Libre  Office,  assinale  a alternativa INCORRETA.

Obs: A tecla + significa a junção de uma tecla com uma letra ou outra tecla.

a) CTRL + X – Corta os itens Selecionados.
b) CTRL + V – Cola os itens copiados ou cortados da área de transferência.
c) SHIFT + F – Procura o termo de pesquisa inserido pela última vez.
d) CTRL + Z – Desfaz a última ação.
e) CTRL + Y – Refaz a última ação.




Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 





102
102




GABARITO – DIVERSAS BANCAS 
1. LETRA C
2. LETRA C
3. LETRA B
4. LETRA C
5. LETRA B
6. LETRA C
7. LETRA A
8. LETRA E
9. LETRA A
10. LETRA D
11. LETRA C
12. LETRA B
13. LETRA D
14. LETRA A
15. LETRA D
16. LETRA D
17. LETRA A
18. LETRA C
19. LETRA A
20. LETRA D
21. LETRA A
22. LETRA B
23. LETRA A
24. LETRA C
25. LETRA D
26. LETRA A
27. LETRA C
28. LETRA B
29. LETRA C
30. LETRA C
31. LETRA A
32. LETRA B
33. LETRA C
34. LETRA A
35. LETRA B
36. LETRA D
37. LETRA E
38. LETRA C

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 13
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 