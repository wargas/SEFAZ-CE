

Livro Eletrônico
Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti 06315057411 - EVA CELESTE DE SOUZA 









1
82
Sumário
Apresentação da Aula ...................................................................................................................... 2 Backup ............................................................................................................................................. 3 1 – Conceitos Básicos ................................................................................................................... 3 2 – Tipos de Backup ..................................................................................................................... 7 2.1 Backup Completo ............................................................................................................... 7 2.2 Backup Incremental ............................................................................................................. 9 2.3 Backup Diferencial ............................................................................................................ 12 2.4 Backup de Cópia ............................................................................................................... 16 2.5 Backup Diário .................................................................................................................... 16 Resumo .......................................................................................................................................... 18 Questões Comentadas .................................................................................................................. 20 Lista de Questões .......................................................................................................................... 60 Gabarito ......................................................................................................................................... 81 














Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







2
82



APRESENTAÇÃO DA AULA Fala, galera! O assunto da nossa aula de hoje é Backup (Becape)! Pessoal, eu sou meio paranoico com cópias de segurança. Eu já sonhei (na verdade, foi um pesadelo) que havia perdido todas as aulas que eu tinha escrito na vida. Vocês têm noção de que eu já escrevi mais de 10.000 páginas? Se eu  já  fico  paranoico,  imagina  o  impacto  que  uma  empresa  tem  se  perder  seus  dados.  Para  isso existem as cópias de segurança e hoje nós vamos estudar as estratégias para realiza-las.

PROFESSOR DIEGO CARVALHO - www.instagram.com/professordiegocarvalho 
Galera, todos os tópicos da aula possuem Faixas de Incidência, que indicam se o assunto cai muito ou pouco em prova. Diego, se cai pouco para que colocar em aula? Cair pouco não significa que não cairá justamente na sua prova! A ideia aqui é: se você está com pouco tempo e precisa ver somente aquilo que cai mais, você pode filtrar pelas incidências média, alta e altíssima; se você tem tempo sobrando e quer ver tudo, vejam também as incidências baixas e baixíssimas. Fechado?

INCIDÊNCIA EM PROVA: baixíssima 
INCIDÊNCIA EM PROVA: baixa 
INCIDÊNCIA EM PROVA: média 
INCIDÊNCIA EM PROVA: ALTA 
INCIDÊNCIA EM PROVA: Altíssima 

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







3
82



BACKUP
1 – CONCEITOS BÁSICOS INCIDÊNCIA EM PROVA: baixa 
Todos  nós  já  sentimos  aquela  sensação  horrível  de perder  algo  precioso:  fotos,  vídeos ou...  uma aula que você passou a madrugada inteira escrevendo! Isso é frustrante, mas é menos traumático.
O bicho pega quando são perdidos dados de sistemas de informação de uma organização em que muitas pessoas necessitam e confiam – afetando a integridade dessas informações! Perder dados se traduz imediatamente em perda de confiança em instituições.

Vocês já imaginaram se todos os dados das aulas do nosso curso e de outros professores fossem perdidos? Vocês ficariam furiosos, porque vocês confiam na integridade dos dados e dependem    deles    para    organizarem    seus    estudos, cronogramas, entre outros. Se não houver uma redundância de   armazenamento,   todos   os   professores   terão   que reescrever  ou  regravar  tudo  de  novo,  o  que  geraria um prejuízo insano para a instituição, para os professores e para os  alunos.  Dados  são  perdidos  frequentemente!
Em  um
minuto  está  tudo  perfeito,  no  minuto  seguinte  algum arquivo importante em um banco de dados se corrompe, ocorre algum desastre natural (Incêndio, Inundação, etc), um  dispositivo  de  armazenamento  é  furtado  ou  você deleta algo sem querer (Quem nunca?).


Por conta disso, quando você tem dados sensíveis, é necessário fazer cópias de segurança – essa cópia de segurança é também conhecida como Backup.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







4
82



Backup  é  um  serviço  que  garante  que  você  pode  sempre  recuperar  informações  de  forma confiável e tempestiva. Em geral, recomenda-se gravar em alguma mídia removível ou em algum local  seguro  em  que  nenhum  acidente  poderia  danificar  o  original  e  a  cópia.  O backup  pode  ser armazenado na própria instituição (on-site) ou em algum local geograficamente remoto (off-site) – preferencialmente o segundo, visto que um desastre no site principal não afetaria o backup.

Imaginem  se  os  dados  de  sistemas  de  empresas  localizadas  nas  Torres  Gêmeas  tivessem  seus backups armazenados também nas Torres Gêmeas. Em caso de um atentado terrorista, a empresa perderia tanto os dados originais quanto seus becapes. Becape, professor? Tome vergonha na cara e escreva certo, Diego! Calma, parça!
Becape é a palavra aportuguesada de backup – vocês verão algumas questões utilizando esse termo em vez do termo em inglês. Bacana?

Ademais, o backup deve armazenar as informações em uma mídia segura de modo que, caso haja alguma pane, seja possível restaurar a informação original. Professor, o que você quer dizer com mídia segura? Pode  ser  em  um pendrive,  em  fitas  magnéticas,  em  cartões  de  memória,  na nuvem, em um HD externo, etc. A escolha da mídia de armazenamento do backup é relevante tanto para a gravação da cópia de segurança como para a restauração dos dados de um backup.

Como  assim,  professor?  Galera,  se  eu  for  fazer  um  backup  doméstico,  não  há  problema  em armazená-lo em um pendrive; mas se eu for fazer em uma empresa, ele não é o mais recomendado.
Para  realizar  essa  escolha,  deve-se  levar  em  consideração  o  volume  de  dados,  o  tempo  de leitura/escrita  de  dados,  o  tempo  de  restauração  de  backup,  o  custo  da  mídia  de armazenamento, entre outros.
Professor, eu posso fazer o backup na Memória RAM?

Não, cara! A Memória RAM é um tipo de memória volátil, logo ela não é recomendável para fazer backup porque – caso haja alguma queda de energia – perde-se tudo que estiver armazenado. Por falar  nisso,  dentre  os  meios  que  nós  mencionamos,  o  mais  indicado  atualmente  é  o  backup  em nuvem! Por que?
Porque geralmente os arquivos são guardados em locais fisicamente de alta segurança.
Como assim, Diego?

As empresas que fazem armazenamento em nuvem (Ex: Google, Dropbox, Apple, etc) geralmente investem fortunas em infraestruturas de proteção de dados contra incêndios, quedas de energia, enchentes, danos físicos, etc – ademais, há redundâncias em locais geograficamente distantes.
E
mais: se você quiser proteger ainda mais  possíveis dados sensíveis, pode-se criptografar os backups feitos na nuvem.
Certinho?

(MDIC – 2014) A  definição  e  a  execução  de  procedimentos  regulares  e  periódicos  de becape  dos  dados  de  um  computador  garante  a  disponibilidade  desses  dados  após eventuais ocorrências de desastres relacionados a defeitos tanto de hardware quanto de software.
_______________________ Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







5
82



Comentários: Backup é a salvaguarda da exatidão da informação que pode ser restaurada a qualquer instante, mas não garante a disponibilidade da informação - apenas sua integridade. Em geral, você só pode dizer que o backup garante disponibilidade se estiver explícito que se trata de um backup salvo em local fisicamente distinto dos dados originais (Errado).

ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO!
ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO!
ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO!
ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO!
ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO! ATENÇÃO!

Muita atenção agora porque nós vamos entender como funcionam as rotinas de backup! Vamos imaginar  o  seguinte  cenário:  em meu  computador,  eu tenho  um  disco  rígido. No Windows,  esse disco rígido pode ser acessado por meio do diretório C:\, onde estão armazenados meus arquivos pessoais.  Vamos  supor  que  –  dentro  da  pasta C:\Usuários\Adm\Documentos –  eu  tenha  três arquivos: Felipe.mp3, Renato.docx, Diego.xlsx.



Galera,  todo  arquivo  quando  é  criado  ganha  um  atributo  de  arquivamento! É o que, Diego? Isso mesmo, um atributo de arquivamento – também chamado de Bit Archive ou Flag Archive!
E o
que seria isso? Vocês devem saber que toda informação em um computador é representada por bits (0 ou 1). O atributo de arquivamento é um único bit de um arquivo que indica que esse arquivo não sofreu backup. Vamos entender isso melhor? Bora lá...



Sabe o que é isso acima? É o prompt de comando do Windows! Eu fui lá e digitei um comando (relaxa, vocês não precisam saber) que mostra quais são os atributos dos arquivos da nossa pasta. Galera, cada arquivo pode ter quatro atributos, representados pelas letras A, S, H e R. O que eles significam?
Por exemplo: um arquivo com atributo R é somente-leitura, isto é, ele só pode ser lido/acessado, mas não pode ser modificado.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







6
82



Já o atributo H significa que um determinado arquivo está oculto. Seguindo a lógica, um atributo S significa que se trata de um arquivo de sistema. Professor, eu tenho que saber isso? Não, o único que é importante agora é o atributo A! Por que? Porque ele é o nosso atributo de arquivamento!
Toda
vez  –  tooooooooooda  veeeeeeeeeez  –  que  um  arquivo  é  salvo/modificado,  ele  ganha  um atributo A, o que significa que ele não sofreu backup.

Agora que vem a sacada para que vocês entendam todo o restante da aula, portanto prestem bastante atenção. Nós sabemos que toda vez que um arquivo é salvo/modificado, ele ganha um atributo  A  (de  arquivamento)  para  indicar  que  esse arquivo  não  sofreu  backup. O que acontece quando eu faço um backup desse arquivo? O atributo A desaparece para indicar que aquele arquivo já sofreu backup, isto é, foi arquivado.

Logo,  o  atributo  de  arquivamento  é  utilizado  pelo  sistema  operacional  para  indicar  se  um determinado arquivo precisa sofrer backup ou não. Ué, professor... e se eu fizer um backup manual, simplesmente copiando um arquivo para um backup? Isso funciona, mas não é recomendável – o ideal é utilizar algum software de backup. E como esse software sabe o que copiar ou não? Por meio do tipo de backup e do atributo de arquivamento.

Antes  de  partir  para  o  estudo  sobre  os  tipos  de  backup,  é  importante  falar  um  pouco  sobre  os termos utilizados em prova.
Nós sabemos que o atributo de arquivamento é, na realidade, um bit. Logo, ele só pode ter dois valores: 0 ou 1! Quando a prova diz que o atributo de arquivamento é  marcado,  significa  que  Bit  Archive  =  1  (arquivo  recebe  o  atributo  A);  e  quando  o  atributo  de arquivamento é desmarcado, significa que Bit Archive = 0 (arquivo perde o atributo A).

(Prefeitura  de  Passagem  Franca  do  Piauí/PI  –  2016) “Trata-se  de  uma  cópia  de segurança dos dados ou programas que permite restaurar elementos perdidos em caso de uma falha ou perda dos dados”. O texto fala da técnica conhecida como:

a) backup
b) dashboard
c) recovery
d) firmware
e) temporary
_______________________ Comentários: conforme vimos em aula, a questão trata de Backup (Letra A).






Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







7
82



2 – TIPOS DE BACKUP

2.1 Backup Completo
INCIDÊNCIA EM PROVA: ALTA 
Também chamado de Total, Normal ou Full, trata-se do backup que faz uma cópia de todos os dados  de  uma  unidade.  Se  uma  organização  possui  a  política  de  realizar  backup  completo diariamente, todos os dados serão copiados todos os dias, mesmo que não tenham sido alterados.
A principal vantagem é que aumenta a chance de recuperação de dados íntegros, além de realizar uma operação menos sofisticada/complexa e de exigir um menor tempo para recuperar dados.



Por outro lado, trata-se de um procedimento com tempo de execução maior e requer mais espaço  de  armazenamento,  visto  que  todos  os  arquivos  serão  copiados.  Dessa  forma,  por limitações  técnicas,  esse  tipo  de backup  é  realizado  periodicamente,  em  geral  combinados  com backups  incrementais  e/ou  diferenciais.  Em  suma:  se  acontecer  um  desastre,  basta  restaurar  o último backup completo, por outro lado pode ocupar muito espaço e demorar muito tempo.

Voltando  ao  nosso  exemplo! Por  que  todos  os  arquivos  da  nossa  pasta  possuem  o atributo  de arquivamento?
Nós  vimos  que,  sempre  que  um  arquivo  é  salvo,  ele  recebe  um  atributo  de arquivamento.  Como  os  três  arquivos  da  pasta  foram  criados/salvos  sem  nunca  terem  sofrido backup,  então  todos  eles  possuem  esse  atributo. O que faz o backup completo?  Ele  basicamente copia todos esses arquivos sem se importar se o arquivo possui atributo de arquivamento ou não!



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







8
82



Professor, o que aconteceria se eu fizesse um backup normal dos arquivos acima? Nesse contexto, o software de backup copiaria todos esses arquivos em um único arquivo compactado chamado, por exemplo,
Backup_Completo_1.bkf.  Além  disso,  ele  desmarcaria  o  atributo  de  arquivamento  (Bit Archive = 0), uma vez que esse atributo serve para indicar se um arquivo sofreu backup. Notem na imagem a seguir que todos os arquivos perderam o atributo de arquivamento...



Galera,  imaginem  uma  empresa  com  quinhentos  computadores!  Em  geral,  não  é  viável  fazer backup normal todos os dias porque pode demorar horas e horas – o mais comum é realizar esse tipo de backup a cada dez ou quinze dias e frequentemente aos domingos para não atrapalhar os funcionários, uma vez que reduz o desempenho das máquinas . Entendido, pessoal? Vamos fazer alguns exercícios para testar...

(CRM/SC – 2015) Existem várias maneiras de se realizar cópias de segurança, conhecida como backups. A forma mais simples (menor sofisticação) para fazê-lo é:

a) Backup diferencial.
b) Backup completo.
c) Backup incremental.
d) Backup delta.
_______________________ Comentários: conforme vimos em aula, trata-se do Backup Completo (Letra B).

(MEC – 2015) Um becape completo consiste na cópia de todos os arquivos para a mídia de becape.
_______________________ Comentários: conforme vimos em aula, um becape completo realmente copia todos os arquivos para uma mídia (Correto).










Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







9
82



2.2 Backup Incremental INCIDÊNCIA EM PROVA: Altíssima 
Trata-se de uma cópia de todos os dados que foram criados ou modificados desde o último backup normal ou  incremental anterior.  Ele  surgiu  para  sanar  algumas  deficiências  do Backup Completo, como sempre copiar todos os dados a cada operação mesmo que nenhuma alteração tenha  sido  realizada.  Após  o backup,  ele  desmarca  o  atributo  de  arquivamento  (Bit  Archive =  0), informando que aquele arquivo já sofreu backup.



O primeiro passo é realizar um Backup Completo! Nos backups incrementais subsequentes, serão copiados apenas os dados modificados ou criados desde o último backup normal ou incremental anterior.
A principal vantagem é que será copiada uma quantidade menor de dados do que no caso de um backup completo.
Por consequência, o Backup Incremental também é realizado mais rapidamente e necessita de menos espaço de armazenamento.

Por outro lado, a recuperação de dados é mais lenta e complexa, visto que o último backup completo  deve  ser  recuperado  e,  em  seguida,  os  dados  incrementais  de  cada  dia  até  o momento da falha.
Isso significa, por exemplo, que se tivermos um backup completo (Domingo) e três backups  incrementais  do  mesmo  arquivo  (Segunda,  Terça  e  Quarta),  este  será  recuperado quatro vezes – tornando o gerenciamento mais complexo para o administrador.



Voltando  ao  nosso  exemplo!  Vejam  acima  que  nossos  arquivos  sofreram  backup,  logo  nenhum apresenta  o  atributo  de  arquivamento.  No  entanto,  no  dia  seguinte  o  arquivo Renato.docx foi
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







10
82



modificado. Além disso, foi criado um novo arquivo em nossa pasta chamada Heber.pptx. Nesse momento, meu backup já está desatualizado. Vejam na imagem a seguir que há dois arquivos que estão com o atributo de arquivamento – indicando que não sofreram backup.



Eu posso fazer um backup completo? Posso, mas demoraria horas! Uma estratégia mais interessante seria  fazer  um  backup  incremental. O que é um incremento?  É  um  aumento,  um  acréscimo,  uma adição! Logo, o backup incremental vai adicionar algo ao backup que já temos (no caso, o backup completo)  e  gerar  o  arquivo Backup_Incremental_1.bkf.    Esse  tipo  de  backup  copia  apenas  os arquivos novos ou modificados – indicados pelo atributo de arquivamento.



Após  copiar  os  arquivos,  desmarca-se  o  atributo  de arquivamento  desses  dois  arquivos  –  como mostra a imagem acima. No dia seguinte, altera-se novamente o arquivo Renato.docx, altera-se o arquivo
Felipe.mp3 e cria-se mais um arquivo chamado Paulo.rar. Notem, na imagem abaixo, que esses três arquivos são marcados com o atributo de arquivamento, indicando que esses arquivos não sofreram backup.



Quando  fizermos  um  novo  backup  incremental,  nós  já sabemos  que  serão  copiados  apenas  os arquivos  criados  ou  modificados  desde  o  último  backup  incremental  anterior.  Dessa  forma,  será gerado o arquivo
Backup_Incremental_2.bkf. Após a geração do arquivo, desmarca-se o atributo de arquivamento desses três arquivos. Qual é a grande vantagem do backup incremental? Galera, o backup incremental só copia o incremento, logo é beeeeem mais rápido de ser criado.

Por outro lado, a restauração do backup é mais trabalhosa. Como assim, Diego? Pensem comigo:
um backup completo é feito no domingo, e depois backups incrementais são feitos diariamente até sexta-feira. Se um disco rígido de uma máquina queima no sábado, eu precisarei comprar um novo Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







11
82



disco  rígido,  buscar  o  backup  completo  mais  todos  os  backups  incrementais  de  segunda,  terça, quarta, quinta e sexta, e inserir tudo no disco rígido novo.

Se eu tivesse feito backups completos todos esses dias, nós já sabemos que seria muito demorado.
Por outro lado, eu poderia simplesmente restaurar o backup completo de sexta-feira no novo disco rígido  e  rapidinho  tudo  estaria  restaurado  e  funcionando  normalmente. Viram  agora  como  há vantagens e desvantagens em cada tipo de backup?
Pois é... é uma decisão que deve ser tomada pela direção da empresa.

(Polícia Federal – 2013) Imediatamente  após  a  realização  de  um  becape  incremental utilizando-se um software próprio de becape, há expectativa de que esteja ajustado  o flag  archive  de  todos  os  arquivos  originais  que  foram  copiados  para  uma  mídia  de becape.
_______________________ Comentários: conforme vimos em aula, desmarca-se a Flag/Bit Archive de todos os arquivos que foram copiados para o backup (Correto).



























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







12
82



2.3 Backup Diferencial INCIDÊNCIA EM PROVA: Altíssima 
Também conhecido como Backup Incremental Cumulativo, trata-se de uma cópia de todos os dados  que  foram  criados  ou  modificados  desde  o  último  backup  completo  ou  incremental.
Percebam que o Backup Diferencial copiará todos os dados que foram modificados desde o último backup completo ou incremental anterior e não removerá o atributo de arquivamento (Bit Archive = 1). Entendido?



Notem que ele armazena mais dados do que o Backup Incremental. Isso exige mais espaço e mais tempo de backup que os backups incrementais. Por  outro  lado,  a  recuperação  de  dados tende a ser mais rápida que o backup incremental, uma vez que só são necessários o último backup completo e o último backup diferencial, enquanto o backup incremental necessita do último backup completo e de todos os backups incrementais.



Voltando ao nosso exemplo! Nós tínhamos os três arquivos acima sem o atributo de arquivamento porque   os   arquivos   haviam   sofrido   um   backup   normal,   sendo   gerado   o   arquivo Backup_Completo_1.bkf.  No  dia  seguinte,  o  arquivo Renato.docx foi  modificado  e  o  arquivo Heber.pptx foi criado. Notem na imagem a seguir que eles possuem o atributo de arquivamento indicando que não sofreram backup.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







13
82





Nós podemos fazer – então – um backup diferencial somente com esses dois arquivos, gerando o arquivo
Backup_Diferencial_1.bkf. Ué, Diego! Ficou exatamente igual ao backup incremental do exemplo anterior. Sim, mas há uma diferença fundamental: após o backup diferencial, os atributos de arquivamento não são removidos. No dia seguinte, criam-se os arquivos Paulo.rar e Terror.bmp, e gera-se o arquivo Backup_Diferencial_1.bkf.



Notem  na  imagem  acima  que  esse  segundo  backup  diferencial  copiará  os  arquivos  novos,  mas também copiará os arquivos copiados pelo primeiro backup diferencial, uma vez que os atributos de  arquivamento  não  foram  removidos. A  grande  vantagem  é  que  –  para  restaurar  –  nós precisamos apenas do backup completo e do último backup diferencial – pode-se descartar o primeiro backup diferencial.
Compreenderam?

BACKUP INCREMENTAL BACKUP DIFERENCIAL DIA 1 Backup Normal DIA 1 Backup Normal DIA 3
Backup
Incremental
DIA 3 Backup Diferencial DIA 5
Backup
Incremental
DIA 5 Backup Diferencial DIA 7
Backup
Incremental
DIA 7 Backup Diferencial DIA 9
Backup
Incremental
DIA 9 Backup Diferencial 
Notem  na  tabela  acima  uma  comparação  entre  esses  dois  últimos  tipos  de  backup.  No  caso  do Backup Incremental: caso ocorra uma falha no dia 10, temos que restaurar todos os backups para retornarmos os dados completamente. No caso do Backup Diferencial: caso ocorra uma falha no dia 10, temos que restaurar apenas o Backup Normal e o último Backup Diferencial.
Logo, o Backup
Diferencial é mais rápido de restaurar, mas é mais lento para criar.
Bacana?

(Prefeitura  de  Florianópolis  –  2014) A  diferença  entre  um backup  Incremental  e  um backup Diferencial é:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







14
82



a)  O backup  diferencial  marca  os  arquivos  copiados  como  arquivos  que  passaram  por backup,  enquanto  o backup  incremental  não  marca  os  arquivos  como  arquivos  que passaram por backup.

b)  Para  restaurar  um backup  diferencial  deve-se  possuir  todos  os backups  realizados desde o último backup normal, incluindo outros backups diferenciais realizados ao longo do tempo, enquanto o incremental necessita somente o último backup normal.

c)  O backup  diferencial  copia  todos  os  arquivos  criados  ou  alterados  desde  o  último backup normal, enquanto o incremental copia somente os arquivos criados ou alterados desde o último backup incremental ou normal.

d) Um backup que utiliza uma combinação de backups normal e incremental exige mais espaço  em  disco  que  uma  combinação  de backups  normal  e  diferencial, e  é  o  método mais lento para fazer backup.

e) Um backup que utiliza uma combinação de backups normal e diferencial exige menos espaço em disco que uma combinação de backups normal e incremental, mas é o método mais lento para restaurar os dados.
_______________________ Comentários: (a) Errado, a questão inverteu os conceitos; (b) Errado, a questão inverteu os conceitos; (c) Correto, o backup diferencial  copia  todos  os arquivos criados  ou alterados  desde  o  último  backup  normal  ou incremental, enquanto  o  backup incremental copia somente os arquivos criados ou alterados desde o último backup incremental ou normal; (d) Errado, a questão inverteu os conceitos; (e) Errado, a questão inverteu os conceitos (Letra C).

(CRA/SC – 2013) Assinale a alternativa que diz respeito a seguinte definição:

“Este tipo de backup fornece um backup dos arquivos modificados desde que foi realizado um backup completo. Normalmente salva somente os arquivos que são diferentes ou novo desde o último backup completo, mas isso pode variar em diferentes programas de backup.
Juntos,  um  backup  completo  e  um  backup  desse  tipo  incluem  todos  os  arquivos  no computador, alterados e inalterados.” 
a) Backup incremental.
b) Backup de referência.
c) Backup normal.
d) Backup diferencial.
_______________________ Comentários: (a) Errado. O Backup Incremental copia somente os arquivos criados ou alterados desde o último backup normal ou incremental; (b) Errado. Esse tipo de backup não existe; (c) Errado. O Backup Normal faz uma cópia de todos os dados de uma  unidade;  (d)  Correto.  O  Backup  Diferencial  copia  os  arquivos  criados  ou  alterados  desde  o  último  backup  normal  ou incremental (Letra D).

(ANEEL  –  2010) Um  backup  diferencial  copia  arquivos  criados  ou  alterados  desde  o último backup normal ou incremental. O atributo de arquivo não é desmarcado. Caso o Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







15
82



usuário  esteja  executando  uma  combinação  dos  backups  normal  e  diferencial,  a restauração  de  arquivos  e  pastas  exigirá  o  último  backup  normal  e  o  último  backup diferencial.
_______________________ Comentários: Um  backup  diferencial  copia  arquivos  criados  ou  alterados  desde  o  último  backup  normal  ou  incremental?
Correto! O atributo de arquivo não é desmarcado? Correto (Flag Archive = 1); Caso o usuário esteja executando uma combinação dos  backups  normal  e  diferencial,  a  restauração  de arquivos  e  pastas  exigirá  o  último  backup  normal  e o  último  backup diferencial? Correto! Você precisará do backup normal e o último backup diferencial (Correto).




































Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







16
82



2.4 Backup de Cópia
INCIDÊNCIA EM PROVA: baixa 
Trata-se de uma cópia de todos os arquivos selecionados, mas não os marca como arquivos que passaram por backup, isto é, não alteram a Flag/Bit Archive.  Em  geral,  é  utilizado  de  forma emergencial e normalmente é usada caso se queira fazer o backup de arquivos entre um backup completo e um backup incremental. Galera, esse é o tipo de backup mais raro em prova até porque ele é extremamente simples.

(BANESTES  –  2014  –  IV) O  backup  utilizado  de  maneira  emergencial,  e  que normalmente antes de alguma alteração crucial no sistema, pode não afetar a rotina de backups organizados da empresa é o backup de cópia.
_______________________ Comentários: O Backup de Cópia geralmente é utilizado de maneira emergencial ou antes de alterações cruciais no sistema.
Antes de correr algum risco, você faz o backup (Correto).

2.5 Backup Diário
INCIDÊNCIA EM PROVA: baixa 
Trata-se de uma cópia de todos os arquivos selecionados que foram modificados no dia da execução  do  backup  diário.  Os  arquivos  não  são  marcados  como  arquivos  que  passaram  por backup,  isto  é, não  alteram  a Flag/Bit Archive.  Ele  utiliza  como  critério  apenas  a  data  do  backup.
Quanto a esse backup, assim como o anterior, não há muito o que detalhar. Ele é tão simples de entender que – junto com o anterior – são os mais raros de cair em prova. Bacana?

(BANESTES  –  2014  –  IV) Sabemos  que  a  cópia  de  segurança  de  todos  os  dados e informações  utilizadas  é  de  suma  importância  para  todos.  Diante  disso,  marque  a alternativa correta sobre o modelo de backup diário.

a) Copia todos os arquivos não selecionados que foram modificados no dia da execução do backup diário

b)  Copia  parcialmente  os  arquivos  selecionados  que foram  modificados  no  dia  da execução do backup diário.

c) Copia todos os arquivos selecionados que não foram modificados no dia da execução do backup diário.

d)  Copia  todos  os  arquivos  não  selecionados  que  não  foram  modificados  no  dia  da execução do backup diário.

e) Copia todos os arquivos selecionados que foram modificados no dia da execução do backup diário.
_______________________ Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







17
82



Comentários: conforme vimos em aula, copia todos os arquivos selecionados que foram modificados no dia da execução do backup diário (Letra E).

Bit/flag archive





Comparativo de backups 



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







18
82



RESUMO

FUNCIONAMENTO
Todo arquivo  no seu  computador  possui um  atributo  de  arquivamento  chamado  Bit/Flag  Archive. O que é isso, professor?  É  um  único  bit  que  pode  possuir  o  valor  1  (marcado)  ou  0  (desmarcado).  Sempre  que  salvamos  um arquivo, esse atributo fica marcado (1) e – ao fazer um backup normal ou incremental – ele é desmarcado (0) para indicar que já sofreu backup.

TIPO DE BACKUP

DESCRIÇÃO

BACKUP COMPLETO

Também chamado de Total, Normal ou Full, trata-se do backup que faz uma cópia de todos os  dados  de  uma  unidade.  Se  uma  organização  possui a  política  de  realizar  backup completo  diariamente,  todos  os  dados  serão  copiados  todos  os  dias,  mesmo  que  não tenham sido alterados. A principal vantagem é que aumenta a chance de recuperação de dados íntegros, além de realizar uma operação menos sofisticada/complexa e de exigir um menor tempo para recuperar dados.
BACKUP INCREMENTAL

Trata-se de uma cópia de todos os dados que foram modificados desde o último backup – não  importa  de  qual  tipo  (Ex:  Backup  Completo,  Backup  Diferencial  ou  Backup Incremental).  Ele  surgiu  para  sanar  algumas  deficiências  do  Backup  Completo,  como sempre copiar todos os dados a cada operação, mesmo que nenhuma alteração tenha sido realizada. Após o backup, ele desmarca o atributo de arquivo (Bit Archive).

BACKUP DIFERENCIAL

Trata-se de uma cópia de dados em que, após realizar o primeiro backup completo, cada backup  diferencial  compara  o  conteúdo  a  ser  copiado  com  o  último  backup  completo  e copia todas as alterações realizadas. Notem que o Backup Incremental copiava todos os dados que foram modificados desde o último backup. O Backup Diferencial copiará todos os dados que foram modificados desde o último backup completo.

BACKUP DE CÓPIA

Trata-se de uma cópia de todos os arquivos selecionados, mas não os marca como arquivos que passaram por backup, isto é, não alteram a Flag/Bit Archive. Em geral, é utilizado de forma emergencial e normalmente é usada caso queira fazer o backup de arquivos entre um backup completo e um backup incremental.


BACKUP DIÁRIO

Trata-se de uma cópia de todos os arquivos selecionados que foram modificados no dia da execução do backup diário. Os arquivos não são marcados como arquivos que passaram por backup, isto é, não alteram a Flag/Bit Archive.





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







19
82




Bit/flag archive




Comparativo de backups 



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







20
82



QUESTÕES COMENTADAS

1. (CESPE  /  IFF  /  Conhecimento  Gerais  -  2018) Na  primeira  vez  que  se  realiza  uma  cópia  de segurança, seja de um servidor ou de um computador pessoal, o tipo de becape mais indicado é o:

a) diferencial.
b) incremental
c) periódico.
d) diário.
e) completo.

Comentários:

Tanto antes do Backup Incremental quanto antes do Backup Diferencial, recomenda-se fazer um Backup Completo.

Gabarito: Letra E

2. (FCC / SABESP/ Estagiário - 2017) Uma organização possui a política de realizar backup todos os  dias  e  todos  os  dados  são  copiados  diariamente, independentemente  de  terem  sido modificados ou não, para dispositivos do tipo fita magnética, disco magnético ou óptico, DVD ou blu-ray. Esta organização realiza backup do tipo:

a) completo
b) incremental
c) diferencial
d) progressivo
e) cumulativo

Comentários:


Backup de todos os dados? Independente de terem sido modificados ou não? Trata-se  do  Backup Completo. Esse tipo de backup realiza a cópia de todos os arquivos e pastas, sem se importar se os arquivos foram modificados ou são idênticos – tudo é copiado.

Gabarito: Letra A

3. (CESPE  /  PC-GO  /  Agente  de  Polícia  -  2016) Com  relação  aos  procedimentos  de  becape, assinale a opção correta.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







21
82



a) O becape incremental deve ser feito depois de realizada cópia completa de todos os arquivos de interesse.

b) A cópia completa deve ser feita periodicamente, para copiar os arquivos que sofreram alguma modificação na última cópia incremental.

c)  Na  cópia  incremental,  não  é  necessário  especificar  os  intervalos  de  tempo  em  que  houve alterações nos arquivos.

d) O becape incremental não utiliza dados recuperados das cópias completas.

e)    Na    cópia    incremental,    os    arquivos    copiados    anteriormente    são    recopiados, independentemente do ponto de recuperação definido.


Comentários:

(a) Correto. Conforme vimos em aula, o becape incremental deve ser feito depois de realizada cópia completa de todos os arquivos de interesse; (b) Errado. O becape completo é executado apenas no início de cada ciclo de becape incremental. Após um backup incremental, são executados apenas outros backups incrementais; (d) Errado. Todo ciclo de becape incremental se inicia com um becape completo; (e) Errado. Essa é a definição de becape diferencial – o becape incremental não recopia dados já copiados.

A Letra C será comentada pelo Excelentíssimo Prof. Renato da Costa:

“Sabemos  que  o  becape  incremental  utiliza  como  critério  para  cópia  o  status  do  atributo  de arquivamento, copiando somente os arquivos que possuem atributo e retirando-os, marcando como tendo sofrido becape, logo, não há do que se falar acerca de tempo. Não há como se especificar tempo no becape incremental de nenhuma maneira (premissa)”.

Em outras palavras, não faz nenhum sentido falar em tempo. O becape se dá pela marcação do Bit Archive. Por outro lado, dizer que "não é necessário" não está errado, é só uma redação péssima.
De fato, não é necessário especificar os intervalos de tempo porque não fará a menor diferença.
Dessa forma, a questão possui duas respostas, mas a banca considerou como correta apenas a Letra A.

Gabarito: Letra A

4. (IBFC  /  MGS/  Técnico  em  Informática  -  2016) Um  backup  incremental  copia  somente  os arquivos criados ou alterados desde o último backup normal ou incremental, e os marca como arquivos que passaram por backup. Portanto:

a) o atributo de arquivo não é desmarcado.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







22
82



b) o atributo e a seguridade do arquivo não é desmarcado.
c) o atributo de arquivo é desmarcado.
d) o atributo e a seguridade do arquivo é desmarcado.


Comentários:


Notem  que  a  banca  sempre  tenta  confundir  o  aluno  com  a  redação  da  questão.  Marcar  como arquivos  que  não  passaram  por  backup  é  o  mesmo  que desmarcar  (não  marcar)  o  atributo  de arquivamento (Bit Archive = 0). Logo, muito cuidado com essas interpretações!

Gabarito: Letra C

5. (FCC / DPE-SP/ Oficial de Defensoria Pública - 2015) Marcos Paulo fez um backup incremental de seus arquivos. Ele aplicou uma função que copia:

a)  somente os arquivos criados ou alterados desde o último backup normal ou incremental e os marca como arquivos que passaram por backup (o atributo de arquivo é desmarcado).

b) todos os arquivos selecionados e os marca como arquivos que passaram por backup (ou seja, o atributo de arquivo é desmarcado).

c) todos os arquivos selecionados que foram modificados no dia de execução do backup diário.

d) todos os arquivos selecionados, mas não os marca como arquivos que passaram por backup (ou seja, o atributo de arquivo não é desmarcado).

e) arquivos criados ou alterados desde o último backup normal ou incremental. Não marca os arquivos como arquivos que passaram por backup (o atributo de arquivo não é desmarcado).


Comentários:


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







23
82





(a) Correto,  a questão de fato trata do backup incremental, em que se copiam arquivos criados ou alterados desde o último backup normal ou incremental, desmarcando o atributo de arquivamento;
(b) Errado, a questão trata do backup completo; (c) Errado, a questão trata do backup diário; (d) Errado,  a  questão  trata  do  backup  de  cópia;  (e)  Errado,  marcos  os  arquivos  como  arquivos  que passaram por backup e o atributo de arquivo é desmarcado.

Gabarito: Letra A

6. (VUNESP / CM PRADÓPOLIS – 2016) Ao manipular arquivos e pastas, é importante ter cópias de segurança dos arquivos e pastas utilizados. O MS-Windows 7, em sua configuração padrão, possui recursos para fazer cópias de segurança de arquivos e pastas. Assinale a alternativa que contém o nome dado ao procedimento de cópias de segurança.

a) Limpeza de Disco.
b) Clone.
c) Sincronização.
d) Fragmentação.
e) Backup.

Comentários:

O procedimento de realização de cópias de segurança é o backup.

Gabarito:
Letra E

7. (VUNESP / PC SP – 2014) Recomenda-se que um usuário de computador sempre tenha uma cópia  de  segurança  de  seus  arquivos.  A  operação  que  realiza  este  procedimento  é  conhecida como:

a) Digitalização.
b) Codificação.
c) Certificação Digital.
d) Decodificação.
e) Backup.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







24
82




Comentários:

A operação que realiza cópias de segurança é conhecida como Backup.

Gabarito: Letra E

8. (CRESCER CONSULTORIAS / Prefeitura de Lagoa Alegre – PI – 2019) Fazer backup de  100 gigabytes de dados todas as noites quando talvez 10 gigabytes de dados foram alterados não é uma boa prática. Por este motivo, que tipo de backup deve ser utilizado?

a) Backup Completo
b) Backup Diferencial c) Backup Incremental d) Backup Delta

Comentários:



Dentre  as  opções,  aquele  que  ocuparia  menos  espaço de  armazenamento  nesse  contexto  é  o Backup Incremental.

Gabarito: Letra C

9. (QUADRIX / CRESS-SC – 2019) O backup é um procedimento no qual os dados são copiados, preferencialmente, de um dispositivo para outro.

Comentários:

Perfeito!  Não  é  recomendado  realizar  backup  de  dados  no  mesmo  dispositivo  onde  estão armazenados os dados originais.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







25
82



Gabarito: Correto

10. (FADESP  /  DETRAN-PA  –  2019) Com  relação  aos  tipos  de  backup,  analise  as  seguintes afirmativas.

I. O backup completo faz a cópia de todos os arquivos destinados a ele, independente de versões anteriores ou de alterações nos arquivos desde o último backup.

II. O backup incremental faz a cópia dos arquivos que foram alterados ou criados desde o último backup completo ou incremental.

III. Da mesma forma que o backup incremental, o backup diferencial só copia arquivos criados ou  alterados  desde  o  último  backup.  No  entanto,  a  diferença  deste para  o  incremental  é  que cada backup diferencial mapeia as modificações em relação ao último backup completo.

A sequência que expressa corretamente o julgamento das afirmativas é:

a) I – F; II – F; III – V.
b) I – V; II – F; III – F.
c) I – V; II – V; III – F.
d) I – V; II – V; III – V.
e) I – F; II – F; III – F.

Comentários:

(I) Correto. O backup completo não está nem ligando se o arquivo já foi copiado anteriormente ou não – todas as informações são armazenadas;

(II) Correto. O backup incremental copia arquivos que foram alterados ou criados desde o último backup completo ou incremental;

(III)  Correto.  O  backup  diferencia  copia  arquivos  que  foram  alterados  ou  criados  desde  o  último backup completo ou incremental, mas mapeia alterações em relação ao backup completo.


Gabarito: Letra D

11. (IBFC / MGS – 2019) Quanto aos conceitos básicos referentes às cópias de segurança (backup), analise as afirmativas abaixo, dê valores Verdadeiro (V) ou Falso (F):

( ) o backup diferencial armazena todos os dados alterados desde o último backup full.
( ) o backup incremental proporciona na sua execução o maior tempo, e de mídia, de backup.
( ) no backup diferencial, a recuperação de dados necessita de vários conjuntos de mídia.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







26
82




Assinale a alternativa que apresenta a sequência correta de cima para baixo.:

a) V - F - F
b) V - V - F
c) F - V - V
d) F - F - V

Comentários:

(I)  Correto.  Desde  o  último  backup  full  ou  incremental;  (II)  Errado.  O  backup  incremental  é  mais rápido  que  o  completo  e  que  o  diferencial;  (III)  Errado.  É  necessário  apenas  o  último  backup completo e o último backup diferencial para restauração/recuperação de dados.

Gabarito: Letra A

12. (IBADE / Câmara de Porto Velho – 2018) O backup é vital para a preservação dos dados. Com o  objetivo  de  ganhar  eficiência  foi  criada  uma  técnica  grava  apenas  as  alterações  ocorridas desde o último backup e assim sucessivamente. A esse tipo de backup dá-se o nome de:

a) Journal.
b) Full.
c) Incremental.
d) Diferencial.
e) Molecular.

Comentários:

A técnica que grava apenas as alterações ocorridas desde o último backup e assim sucessivamente é o Backup Incremental.

Gabarito: Letra C

13. (CESPE / FUB – 2018) O becape diferencial, utilizado para diminuir a quantidade de fitas a serem lidas e gravadas, é feito a partir de um becape completo e, então, a cada dia, é feito um novo becape de todos os arquivos que foram alterados desde o último becape, seja ele completo ou não.

Comentários:

O becape diferencial é realmente utilizado para diminuir a quantidade de fitas a serem lidas. No entanto, isso é feito a partir de um becape completo e, então é feito um novo becape apenas de arquivos novos ou alterados desde o último backup completo ou incremental.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







27
82




Gabarito: Errado

14. (CONSULPAM  /  Câmara  de  Juiz  de  Fora  –  MG  –  2018) Fazer  backup  de  um  computador significa,  basicamente,  realizar  uma  cópia  de  segurança.  Este  é  um  processo  para  salvar documentos  importantes  e  manter  arquivos  pessoais  protegidos,  em  caso  de  eventuais problemas. Podemos fazer backup utilizando, EXCETO:

a) DVD.
b) Impressoras.
c) HD externo.
d) CD.

Comentários:

Galera,  podemos  fazer  backup  em  um  DVD,  HD  Externo ou  CD.  Não  é  possível  fazer  backup utilizando impressoras.

Gabarito: Letra B

15. (FAUGRS / TJ-RS - 2018) Como se denomina o tipo de backup que contém somente arquivos que    foram    criados    (novos)    ou    modificados    desde    o    último    backup    realizado, independentemente do tipo deste último backup?

a) Diferencial.
b) Incremental.
c) Completo.
d) Espelhamento (mirroring).
e) Inteligente.

Comentários:

Essa  questão  comete  um  deslize  muito  comum  em  várias  outras  questões!  Ela  oferece  como resposta  Backup  Incremental.  No  entanto,  o  Backup  Incremental  não  copia  arquivos  criados  ou modificados desde o último backup realizado independentemente do tipo deste último backup.
Se tivermos um arranjo com Backup Normal, depois um Backup Incremental, depois um Backup Diferencial e depois outro Backup Incremental, esse último copia os dados desde o último Backup Normal ou Incremental anterior. Se considerarmos que ele copia os dados desde o último backup de qualquer tipo, poderíamos inferir que ele copia os dados desde o último backup diferencial – e isso não ocorre porque o backup diferencial não desmarca o atributo de arquivamento. Logo, eu acredito que a questão deveria ter sido anulada.

Gabarito:
Letra B
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







28
82




16. (AOCP / TRT-1ª Região – 2018) O backup de arquivos é altamente recomendado para prevenir a perda de dados importantes. Dos recursos apresentados a seguir, qual NÃO serve para fazer backup de arquivos?


a) Flash drive.
b) Memória RAM.
c) HD externo.
d) Nuvem.
e) Fita magnética.


Comentários:

Todos esses meios podem ser utilizados para fazer backup de arquivos, exceto a Memória RAM. Por que? Por conta de sua volatilidade!

Gabarito: Letra B

17. (FADESP / BANPARÁ – 2018) Sobre cópias de segurança (backup) é correto afirmar que:

a) o backup diferencial realiza uma cópia completa de todos os dados.
b)  sistemas  de  recuperação  de  backup  utilizam  banco  de  dados  sem  operação  dos  usuários quando realiza um backup.
c) o backup incremental utiliza mais espaço em disco que outros tipos de backup.
d) sistemas de recuperação de backup utilizam jobs para gerenciar o tempo e os tipos de backup realizados.
e) o backup diferencial é o mais seguro dos tipos de backup.


Comentários:

(a) Errado, esse é o backup completo; (b) Errado, sistemas de recuperação de backup necessitam da operação de usuários; (c) Errado, ele é o que utiliza menos espaço entre os tipos tradicionais de backup; (e) Errado, não é possível fazer essa afirmação.

(d)  Correto.  Jobs  nada  mais  são  que  procedimentos  que  podem  ser  programados  para  serem executados  em  um  determinado  momento  ou  a  partir  de  um  determinado  gatilho.  No  caso  de sistemas  de  recuperação  de  backup,  utilizam-se  jobs  para  gerenciar  o  tempo  de  execução  de backups e seus tipos.

Gabarito: Letra D

18. (CESGRANRIO / BANCO DA AMAZÔNIA - 2018) O gerente de sistemas pediu que o analista fizesse um backup diferencial. Sendo assim, ele deve fazer um backup também chamado de:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







29
82




a) Backup incremental b) Backup completo (full) c) Backup full deduplicado d) Backup em array de discos e) Backup incremental cumulativo 
Comentários:

O backup diferencial é também conhecido como backup incremental cumulativo.

Gabarito: Letra E

19. (COMPERVE  /  SESAP/RN  –  2018) O  backup  é  um  procedimento  realizado  para  garantir a segurança de dados em sistemas computacionais. A cerca desse procedimento, foram feitas as afirmações seguintes.

I Recomenda-se realizar o backup de uma partição em outra partição no mesmo disco, uma vez que, havendo falha no disco, os dados serão facilmente recuperados.

II O primeiro backup criado para preservar os dados de um sistema é o backup diferencial.

III O backup incremental copia apenas os arquivos criados ou modificados desde o último backup normal.

IV Realizar backups diferenciais ou incrementais requer menos espaço de armazenamento que o backup normal.

Das afirmações, estão corretas 
a) II e III.
b) I e II.
c) III e IV.
d) I e IV.

Comentários:

(I)  Errado,  não  é  recomendável  fazer  o  backup  de  arquivos  no  mesmo  dispositivo  de  origem;  (II) Errado,  é  um  backup  completo;  (III)  Correto,  ele  copia  arquivos  criados  ou  modificados  desde  o último backup normal/completo; (IV) Correto, o backup normal é o que ocupa mais espaço.

Gabarito: Letra C

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







30
82



20. (IBFC  /  Pref.  Divinópolis/MG  -  2018) Assinale  a  alternativa  que  completa  correta  e respectivamente a lacuna da frase a seguir:

“Um  backup  ___________  copia  somente  os  arquivos  criados  ou  alterados  desde  o  último backup normal ou incremental, e os marca como arquivos que passaram por backup (o atributo de arquivo é desmarcado)”.

a)  Integral
b) de Cópia
c) Incremental
d) Diferencial

Comentários:

O backup  que copia somente os arquivos criados ou alterados desde o último backup normal ou incremental poderia ser o backup incremental ou diferencial. No entanto, a questão afirma que esse tipo de backup marca os arquivos que passaram por backup, desmarcando o atributo de arquivo.
Ora, quem desmarca (não marca) o atributo de arquivamento é o Backup Incremental.

Gabarito: Letra C

21. (UECE-CEV  /  DETRAN-CE  -  2018) Como  política  de  segurança  e  recuperação  de  dados, é recomendável realizar uma cópia dos arquivos e pastas alterados desde o último backup. Essa cópia de segurança é denominada:

a) atualização do sistema.
b) backup incremental.
c) compressão de dados.
d) volatilidade da informação.


Comentários:

Copia arquivos e pastas alterados desde o último backup é o... backup incremental!

Gabarito: Letra B

22. (COPERVE-UFSC / UFSC - 2018) Sobre os tipos de backup (cópias de segurança) de arquivos, é correto afirmar que:

a) no backup incremental são copiados os arquivos desde o último backup completo, ou seja, isso não se aplica a backups incrementais e diferenciais.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







31
82



b) no backup completo, no qual todos os arquivos são copiados, as vantagens são a rapidez na realização  do  backup  e  na  recuperação,  e  a  desvantagem  é  o  espaço  utilizado  para armazenamento.

c)  a  maior  desvantagem  do  backup  incremental  é  que seu  processo  de  recuperação  é  mais complexo e lento, pois são recuperadas as informações do último backup completo, seguido de todos os backups incrementais até o momento da falha.

d) no backup diferencial são copiados todos os dados alterados desde o último backup completo ou incremental.

e) a vantagem do backup diferencial sobre o incremental é que são armazenados menos dados desde o último backup completo.


Comentários:

(a) Errado. O backup incremental copia os arquivos desde o último backup normal ou incremental;
(b) Errado. A realização do backup é lenta, a recuperação é rápida e o espaço utilizado é grande; (c) Correto.  A  recuperação  é  realmente  mais  complexa  e lenta,  necessitando  do  último  backup completo e de todos os backups incrementais; (d) Correto. Não vejo nenhum erro nesse item; (e) Errado. O backup diferencial armazena mais dados que o backup incremental.

Gabarito: Letra C

23. (FCC / DPE-AM - 2018) Uma das vantagens de escolher o Backup do tipo diferencial, para ser adotado na Defensoria, é:

a) A recuperação requerer apenas o último Backup diferencial e o último Backup completo.
b) A menor quantidade de dados armazenado se comparado com o Backup incremental.
c) Requerer menor tempo de recuperação se comparado ao Backup completo.
d) A maior tolerância a falhas se comparado com o Backup completo.
e) Requerer um tempo menor para realizar o Backup se comparado com o Backup incremental.

Comentários:

(a)  Correto.  A  recuperação  realmente  necessita  apenas  do  último  backup  completo  e  do  último backup diferencial; (b) Errado. Ele armazena mais dados que o backup incremental; (c) Errado. O tempo  de  recuperação  é  maior  se  comparado  ao  backup  completo;  (d)  Errado.  Ele  é  menos tolerante a falhas que o backup completo; (e) Errado. Ele necessita de um tempo maior para realizar o backup que o incremental.

Gabarito: Letra A

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







32
82



24. (FCC  /  TRF-5ª  Região  -  2017) Dentre  os  vários  tipos  de  backup,  o  Técnico  escolheu  o  tipo Diferencial, pois:

a) ocupa menos espaço de armazenamento se comparado com o backup do tipo Incremental.

b)  a  velocidade  para  a  recuperação  do  backup  é  maior,  se  comparada  com  a  do  backup completo.

c) os tamanhos dos backups diferenciais não crescem progressivamente como ocorre no backup incremental.

d)  cada  backup  diferencial  armazena  apenas  as  modificações  realizadas  desde  o  backup diferencial anterior.

e)  para  a  recuperação  são  necessários  apenas  o  último  backup  completo  e  o  último  backup diferencial.


Comentários:

(a) Errado, ele ocupa mais espaço; (b) Errado, a velocidade de recuperação é menor; (c) Errado, eles crescem progressivamente em contraste com o que ocorre no backup incremental; (d) Errado, ele armazena  as modificações realizadas desde  o último backup normal ou incremental anterior; (e) Correto, ele realmente só necessita do último backup completo e do último backup diferencial.

Gabarito: Letra E

25. (FCC / TST – 2017) Em  uma  situação  hipotética,  um  Analista  de  Suporte em  Tecnologia  da Informação deve escolher o tipo de Backup a ser utilizado no TST. Para tanto, deve considerar que:


a)  para  a  recuperação  dos  dados  de  um  backup  diferencial  são  necessários  apenas  o  último backup diferencial e o último backup completo.

b) a recuperação dos dados de um backup diferencial é mais seguro e integro que em um backup completo.

c) o backup incremental ocupa mais espaço de armazenamento se comparado com o backup diferencial.

d)  para  a  recuperação  dos  dados  de  um  backup  incremental  são necessários  apenas  o  último backup incremental e o último backup completo.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







33
82



e) a recuperação dos dados de um backup do tipo completo é mais demorado que em um backup incremental.

Comentários:

(a) Correto, o backup diferencial necessita apenas do último backup diferencial e do último backup completo; (b) Errado, o backup completo possui uma recuperação mais segura e íntegra; (c) Errado, o  backup  diferencial  ocupa  mais  espaço  que  o  incremental;  (d)  Errado,  são  necessários  o  último backup  completo  e  todos  os  backups  incrementais  subsequentes;  (e)  Errado,  a  recuperação  de dados de um backup completo é mais lenta que em um backup incremental.

Gabarito: Letra A

26. (IBFC / TJ-PE – 2017) Considerando os conceitos de cópias de segurança, ficou-se em dúvida quanto ao atributo de arquivo ser marcado ou não. Os tipos de arquivos nos quais o atributo de arquivo é desmarcado são:

a) Backup Incremental e o Backup Diferencial b) Backup Diferencial e o Backup Diário c) Backup Diário e o Backup Normal d) Backup Diferencial e o Backup Normal e) Backup Incremental e o Backup Normal 
Comentários:



Vamos  relembrar? Atributo  de  arquivo  desmarcado  significa  que  ele  não  possui  o  atributo  de arquivamento (A), logo ele não está marcado como um arquivo que sofreu backup. Quem faz isso?
Tanto o backup incremental quanto backup normal fazem o backup e desmarcam (não marcam) o atributo de arquivamento.

Gabarito: Letra E

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







34
82



27. (QUADRIX / CONTER – 2017) Com relação aos tipos e formas de backup, leia as afirmativas a seguir.

I.  O  backup  incremental  é  a  cópia  de  todos  os  dados  que  foram  modificados  desde  o  último backup de qualquer tipo.

II.  No  backup  diferencial,  com  exceção  da  primeira execução,  quando  é  semelhante  ao incremental, serão copiados todos os dados alterados desde o backup completo anterior.

III.  A  operação  de  um  hot  backup  tem  como  característica  permitir  que  o  sistema  possa permanecer em execução enquanto é realizada.

Está correto o que se afirma em:

a) I e II, somente.
b) II e III, somente.
c) I e III, somente.
d) todas.
e) nenhuma.


Comentários:
(I) Errado. O backup incremental copia os arquivos criados ou modificados desde o último backup normal ou incremental, mas a questão considerou a questão como correta; (II) Correto. O backup diferencial  realmente  copia  todos  os  dados  alterados  desde  o  backup  completo  anterior  (e  do último backup incremental, quando na primeira execução); (III) Correto. Hot Backup nada mais é do que realizar um backup com sistemas em funcionamento, isto é, você não tem que parar o sistema para realizar o backup.

Gabarito: Letra D

28. (QUADRIX  /  CONTER  –  2017) Caso  o  usuário  deseje  realizar  a  cópia  de  todos  os arquivos disponíveis em seu computador para o dispositivo de backup, independentemente de versões anteriores ou de alterações nos arquivos desde a última cópia de segurança, o tipo de backup mais indicado será o:

a) completo.
b) incremental.
c) diferencial.
d) contínuo.
e) periódico.

Comentários:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







35
82



Se  é  independente  de  versões  anteriores  ou de  alterações  nos  arquivos  desde  a  última  cópia  de segurança, recomenda-se utilizar um backup completo.

Gabarito: Letra A

29. (FCC / ARTESP – 2017) Considere, por hipótese, que a ARTESP utiliza uma estratégia de backup conforme mostra a figura abaixo, na qual a escala vertical representa a quantidade de dados.



A figura ilustra a estratégia de backup ..I.., que é semelhante a um backup ..II.. na primeira vez em  que  é  realizado,  na  medida  em  que  irá  copiar  todos  os  dados  alterados  desde  o  backup anterior. No entanto, cada vez que é executado após o primeiro backup, serão copiados todos os dados alterados desde o backup ..III.. anterior e não com relação ao último backup.

As lacunas I, II e III são preenchidas, correta e respectivamente, por:

a) diferencial − incremental − completo b) diferencial − completo − incremental c) incremental − completo − completo d) incremental − diferencial − diferencial e) completo − diferencial − incremental 
Comentários:

Notem que domingo houve um backup completo e, nos dias seguintes, houve backups diferenciais – sempre acumulando as diferenças do backup anterior. Dessa forma, a figura ilustra a estratégia de  backup  diferencial,  que  é  semelhante  a  um  backup  incremental  na  primeira  vez  em  que  é realizado,  na  medida  em  que  irá  copiar  todos  os  dados  alterados  desde  o  backup  anterior.  No entanto,  cada  vez  que  é  executado  após  o  primeiro  backup,  serão  copiados  todos  os  dados alterados desde o backup completo anterior e não com relação ao último backup.

Gabarito: Letra A

30. (EDUCA / CRQ-19ª Região - 2017) Backup é uma cópia de segurança. O termo em inglês é muito utilizado por empresas e pessoas que guardam documentos, imagens, vídeos e outros arquivos no  computador  ou  na  nuvem,  hospedados  em  redes  online  como  Dropbox  e  Google  Drive.
Podemos dividir o termo BACKUP em alguns tópicos.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







36
82



Assinale a alternativa CORRETA que apresenta o tipos de backup:

I. Backup Completo (Full).
II. Backup Diferencial.
III. Backup Incremental.
IV. Backup Intermediário.
V. Backup Suplementar.

Estão CORRETAS:

a) I e II apenas.
b) I, II e III apenas.
c) III, IV e V apenas.
d) II e V apenas.
e) I, II, III e V apenas.

Comentários:

Todos são tipos de backup, exceto o Backup Intermediário e Suplementar – esses não existem!

Gabarito: Letra B

31. (IBFC / EBSERH - 2017) A  maioria  das  políticas  de  backup  empregam  o  conceito  de  backup completo, backup incremental e backup diferencial. Se desejarmos que no momento de restore de  dados  seja  utilizado  o  menor  número  de  mídias,  uma  boa  prática/política  para  dados estratégicos empresariais seria de realizar:

a) um backup completo mensal e um backup diferencial diário b) um backup completo mensal e um backup incremental semanal c) um backup diferencial semanal e backup incremental diário d) um backup completo mensal e um backup incremental diário e) um backup incremental mensal e backup diferencial semanal 
Comentários:

Se desejarmos que no momento de restore de dados seja utilizado o menor número de mídias, uma boa  prática/política  para  dados  estratégicos  empresariais  seria  de  realizar  um  backup  completo mensal  e  um  backup  diferencial  diário. Por que?  Porque  backups  completos semanais  são  muito onerosos e backups diferenciais diários são ideais visto que – em caso de restauração – necessita- se apenas de duas mídias: uma para o backup completo e uma para o último backup diferencial.

Gabarito: Letra A

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







37
82



32. (CRO-SC / CRO-SC - 2016) Sobre o tipo de backup que copia somente os arquivos alterados ou criados depois do último backup incremental é do tipo:

a) Diferencial.
b) Diário.
c) Cópia.
d) Normal.

Comentários:

A  questão  trata  do  backup  diferencial, em  que  são  copiados  dados  criados ou  alterados desde  o último backup normal ou incremental.

Gabarito: Letra A

33. (FCC / TRT-20ª Região - 2016) Um backup completo é executado na sexta-feira e um backup incremental  é  executado  todos  os  dias  a  partir  deste  dia.  No  sábado  são  acrescentados  5 arquivos,  que  são  copiados  no  backup  incremental.  No  domingo  alguns  arquivos  são modificados e somente estes arquivos são copiados no backup incremental. Na segunda-feira os dados do sistema são corrompidos, havendo a necessidade de restauração a partir do backup.
Pode-se concluir que, para restaurar os dados ao estado imediatamente anterior à ocorrência do problema, será necessário restaurar:

a) apenas os backups incrementais realizados.
b) todos os backups completos já realizados no sistema até segunda-feira.
c) apenas os backups incrementais realizados no sábado e no domingo.
d)  somente  o  backup  completo  realizado  na  sexta-feira  e  o  backup  incremental  realizado  no domingo.
e) o backup completo e todos os backups incrementais realizados no período em questão.


Comentários:

Questão  extensa,  mas  a  única  coisa  que  importa  é  que  foram  realizados  um  backup  completo  e vários backups incrementais. Nós sabemos que, em caso de falha e restauração, é necessário tanto o backup completo quanto todos os backups incrementais do período.

Gabarito: Letra E

34. (INAZ DO PARÁ / Prefeitura de Jacundá - PA - 2016) Backup  é  um  termo inglês  que  tem  o significado de cópia de segurança. Como se chama o backup que contém apenas os arquivos que foram criados ou modificados a partir do último backup realizado, e que, depois de fazer a cópia do arquivo, desmarca o atributo (flag) de arquivamento?

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







38
82



a) Diferencial
b) Incremental
c) Completo
d) Seletivo
e) Full


Comentários:

Quem desmarca o atributo de arquivamento é o Backup Incremental!

Gabarito: Letra B

35. (IBFC / EBSERH - 2016) Assinale, das alternativas abaixo, a única que identifica corretamente o tipo de backup que na realização de um restore será necessário apenas o último backup full e, dos vários backups realizados depois do full, somente o último backup:

a) matricial
b) incremental
c) diário
d) diferencial
e) linear


Comentários:

Opa... quando eu necessito apenas do último backup completo (full) e do último backup diferencial, trata-se do backup diferencial.

Gabarito: Letra D

36. (IBFC / EBSERH - 2016) Existem  vários  tipos  de  backup.  Assinale,  das  alternativas  abaixo,  o backup que tem como principal característica a de copiar todos os dados que foram modificados desde o último backup de qualquer tipo:

a) diário
b) full
c) diferencial
d) normal
e) incremental


Comentários:

Essa  questão  comete  um  deslize  muito  comum  em  várias  outras  questões!  Ela  oferece  como resposta  Backup  Incremental.  No  entanto,  o  Backup  Incremental  não  copia  arquivos  criados  ou Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







39
82



modificados desde o último backup de qualquer tipo. Se tivermos um arranjo com Backup Normal, depois um Backup Incremental, depois um Backup Diferencial e depois outro Backup Incremental, esse  último  copia  os  dados  desde  o  último  Backup  Normal  ou  Incremental  anterior.  Se considerarmos que ele copia os dados desde o último backup de qualquer tipo, poderíamos inferir que  ele  copia  os  dados  desde  o  último  backup  diferencial  –  e  isso  não  ocorre  porque  o  backup diferencial não desmarca o atributo de arquivamento. Logo, eu acredito que a questão deveria ter sido anulada.

Gabarito: Letra E

37. (COPEVE-UFAL / UFAL - 2016) Dadas as afirmativas sobre os conceitos de backup de dados, 
I. O objetivo do backup é fazer cópias de todos os arquivos do sistema operacional.
II. O objetivo do backup é fazer cópias de arquivos do usuário.
III. Os backups podem ser do tipo completo ou normal, diferencial e incremental.
IV.  O  primeiro  backup  diferencial  e  o  primeiro  backup  incremental  terão  o  mesmo  conteúdo (backup completo), porém, a partir do segundo ciclo de cópia, o backup diferencial tem como base o último backup completo, ao passo que o backup incremental tem como base os dados copiados na fase anterior de um backup incremental.

Verifica-se que estão corretas apenas:

a) I e II.
b) I e III.
c) III e IV.
d) I, II e IV.
e) II, III e IV.


Comentários:

(I)  Errado,  não  há  necessidade  de  fazer  cópias  de  arquivos  de  sistema;  (II)  Correto,  arquivos  dos usuários são passíveis de backup; (III) Correto, são todos tipos de backup; (IV) Correto, impecável, perfeito... não há nada a acrescentar.

Gabarito: Letra E

38. (IDECAN / UERN - 2016) Analise as afirmativas sobre procedimentos de backup.

I.  O  backup  de  cópia  copia  todos  os  arquivos  selecionados  e  os  marca  como  arquivos  que passaram por backup.

II. O backup diferencial copia arquivos criados ou alterados desde o último backup normal ou incremental e os marca como arquivos que passaram por backup.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







40
82




III.O backup incremental copia somente os arquivos criados ou alterados desde o último backup normal ou incremental e os marca como arquivos que passaram por backup.

Está(ão) correta(s) apenas a(s) afirmativa(s):

a) I.
b) II.
c) III.
d) II e III.


Comentários:

(I) Errado, ele não os marca como arquivos que passaram por backup; (II) Errado, ele não os marca como  arquivos  que  passaram  por  backup;  (III)  Correto,  essa  é  a  descrição  perfeita  de  backup incremental.

Gabarito: Letra C

39. (Instituto Legatus / Prefeitura de Passagem Franca do Piauí – PI - 2016) “Trata-se  de uma cópia de segurança dos dados ou programas que permite restaurar elementos perdidos em caso de uma falha ou perda dos dados”. O texto fala da técnica conhecida como:

a) backup
b) dashboard
c) recovery
d) firmware
e) temporary


Comentários:

Cópia de segurança? Então, é backup!

Gabarito: Letra A

40. (IESES  /  BAHIAGÁS  -  2016) Considere  o  cenário  apresentado  a  seguir,  no  qual  um administrador de sistemas realizou as seguintes tarefas de backup na pasta "COMPRAS":

Dia 01 23:59 - Backup Full 1 Dia 02 23:59 - Backup Diferencial 1 Dia 03 23:59 - Backup Full 2 Dia 04 23:59 - Backup Diferencial 2 Dia 05 23:59 - Backup Diferencial 3 Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







41
82




No  dia  06  alguém  excluiu  acidentalmente  toda  a  pasta  e  o  administrador  precisa  recuperar  a mesma no estado que ela se encontrava no dia 05. Sendo assim, quais backups ele necessitará para realizar o restore (rotina de recuperação dos arquivos)?

a) Backup Full 1 e Backup Full 2.
b) Somente o Backup Full 2 c) Backup Full 1, Backup Diferencial 1, Backup Diferencial 2.
d) Backup Full 1 e Backup Diferencial 1.
e) Backup Full 2 e Backup Diferencial 3.


Comentários:

Nós  sabemos  que  a  restauração  de  dados  do  backup  diferencial  necessita  do  último  backup completo e do último backup diferencial, logo: Backup Full 2 e Backup Diferencial 3.

Gabarito: Letra E

41. (FCC  /  DPE-RR  -  2015) Os  backups  realizados  para  atender  aos  requisitos  de  arquivamento podem ser categorizados como completos, incrementais e diferenciais. O backup incremental:

a) copia os dados que foram modificados desde o último backup completo ou incremental, o que for mais recente.

b) é bem mais lento do que o backup completo, pois é necessário selecionar cada arquivo que foi modificado desde o último backup completo.

c) copia todos os dados nos volumes de produção, indistintamente, porém, em alta velocidade.

d) é, dentre os tipos de backup, o mais lento e que necessita de mais espaço de armazenamento, porém, a restauração é muito rápida.

e)  copia  os  dados  que  foram  modificados  desde  o  último  backup,  sendo  mais  lento  do  que  o backup diferencial, porém, mais rápido na restauração dos dados.

Comentários:

(a)  Correto,  ele  copia  dados  criados  ou  modificados  desde  o  último  backup  completo  ou incremental; (b) Errado, é mais rápido que o backup completo; (c) Errado, não copia todos os dados indistintamente; (d) Errado, é o mais rápido dentre os tipos de backup e necessita de menos espaço de armazenamento; (e) Errado, é mais rápido que o backup diferencial e mais lento na restauração dos dados.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







42
82



Gabarito: Letra A

42. (FCC  /  TRE-PB  -  2015) Considere  que  o  administrador  de  um  servidor  adotou  a  política  de backup  que  utiliza  a  combinação  do  backup  normal  e incremental.  Para  que  o  administrador possa restaurar os dados, ele precisará:

a) de todos os conjuntos de backups normais e de todos os conjuntos de backups incrementais.
b) de todos os conjuntos de backups normais e apenas do último backup incremental.
c) apenas do último backup normal e do último backup incremental.
d) apenas do último backup normal e de todos os conjuntos de backups incrementais.
e) apenas do último backup incremental.


Comentários:

Em  um  arranjo  de  backup  normal  e  incremental,  para restaurar  os  dados  basta  o  último backup normal e todos os backups incrementais subsequentes.

Gabarito: Letra D

43. (FCC / DPE-SP - 2015) Em uma semana, um backup completo é executado na noite de segunda- feira e um backup incremental é executado todas as noites seguintes, até quinta-feira. Na terça- feira, um novo arquivo é acrescentado, e não há alterações nos arquivos anteriores. Na quarta- feira,  nenhum  arquivo  é  acrescentado,  mas  um  arquivo  acrescentado  na  segunda-feira  é modificado. Na quinta-feira, um novo arquivo é acrescentado, e não há alterações nos arquivos anteriores. Na manhã de sexta-feira, há corrupção de dados, o que exige a restauração de todos os dados a partir dos backups realizados na semana. A solução correta, neste caso, é restaurar o backup:

a) realizado na quinta-feira.
b) completo e aplicar os backups incrementais realizados na terça-feira, quarta-feira e quinta- feira.
c) completo e o backup realizado na quinta-feira.
d) completo realizado na segunda-feira.
e) realizado na terça-feira, na quarta-feira e na quinta-feira, depois, o backup completo.


Comentários:

Como  se  trata  de  um  arranjo  de  backups  normal  e  incremental, para  restaurar  os  dados  basta  o último  backup  completo  (de  segunda-feira)  e  todos  os  backups  incrementais  subsequentes  (até quinta-feira).

Gabarito: Letra B

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







43
82



44. (IDECAN  /  PRODEB  -  2015) “Em  uma  empresa  de  venda  de  materiais  para  construção  é utilizado um sistema para o controle de entradas e saídas do estoque. Preocupado com o grande volume de dados e a importância desses para a organização, o dono do empreendimento optou por contratar uma empresa de serviços de informática para montar uma estrutura de backup dos dados. Após um estudo dos processos da empresa, os profissionais contratados montaram uma estrutura que realiza semanalmente uma cópia completa com todos os dados selecionados e  em  paralelo  outra  que,  duas  vezes  por  dia,  copia somente  os  dados  que  foram  criados  ou alterados  desde  o  último  backup  completo.”  Os  profissionais  criaram,  respectivamente, backups do tipo:

a) Normal e diário.
b) Total e diferencial.
c) Diferencial e diário.
d) Normal e incremental.


Comentários:

Após um estudo dos processos da empresa, os profissionais contratados montaram uma estrutura que  realiza  semanalmente  uma  cópia  completa  com  todos  os  dados  selecionados  ( Backup
Normal/Total)  e  em  paralelo  outra  que,  duas  vezes  por  dia,  copia  somente  os  dados  que  foram criados ou alterados desde o último backup completo (Backup Diferencial). No entanto, a banca considerou correta a Letra D – eu discordo completamente!

Gabarito:
Letra D

45. (CESPE / MEC - 2015) Diferentemente dos becapes diferenciais, os becapes incrementais são acumulativos.

Comentários:

Não,  a  questão  inverteu  os  conceitos:  diferentemente  dos  becapes  incrementais,  os  becapes diferenciais são acumulativos.

Gabarito: Errado

46. (CESPE  /  MEC  -  2015) O  becape  incremental  copia  apenas  os  arquivos  que  não  foram modificados desde o último becape.

Comentários:

Na verdade, o becape incremental copia apenas os arquivos que foram modificados desde o último becape.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







44
82



Gabarito: Errado

47. (CESPE / MEC - 2015) Um becape completo consiste na cópia de todos os arquivos para a mídia de becape.

Comentários:

Perfeito, um becape completo copia tudo para a mídia de becape!

Gabarito: Correto

48.(IESES  /  TRE-MA  -  2015) Assinale  a  alternativa  correta  com  relação  aos  tipos  de  backup existentes.

a) Total; Parcial e Diário.
b) Normal; Cópia e Diferencial.
c) Completo; Diário e Incremental.
d) Completo; Incremental; Diferencial.

Comentários:

(a) Errado, não existe Backup Parcial; (b) Correto, todos são tipos de backup; (c) Correto, todos são tipos  de  backup;  (d)  Correto,  todos  são  tipos  de  backup.  Essa  questão  deveria  ter  sido  anulada, porque há três respostas corretas, mas não foi :( 
Gabarito: Letra D

49. (IESES  /  TRE-MA  -  2015) Assinale  a  alternativa  correta  com  relação  a  definição  de  backup incremental e diferencial.

a) No backup incremental o tamanho dos arquivos é maior e o tempo para restauração também é menor.

b) No backup diferencial o tamanho dos arquivos é maior e o tempo para restauração também maior.

c) No backup incremental o tamanho dos arquivos é menor e o tempo para restauração também é menor.

d)  O  backup  diferencial  é  feito  com  base  nas  alterações  desde  o  último  backup  completo,  o tamanho do backup vai aumentando progressivamente.

Comentários:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







45
82




(a)  Errado,  o  tamanho  dos  arquivos  é  menor  e  o  tempo  para  restauração  é  maior;  (b)  Errado,  o tempo para restauração é menor; (c) Errado, o tempo para restauração é maior; (d) Correto, ele é realmente feito com base nas alterações desde o último backup completo e o tamanho do arquivo de backup vai aumentando progressivamente.

Gabarito: Letra D

50. (PR-4 UFRJ / UFRJ - 2015) Um  administrador  de  servidores  deseja  realizar  um  processo  de backup que inclui a realização de uma cópia completa de todos os arquivos de um determinado volume às 06 horas da manhã, e cópias horárias entre 07 e 22 horas que contenham, cada uma delas, todos os arquivos modificados desde a cópia das 06 horas. O tipo de backup das cópias horárias deverá ser:

a) Incremental.
b) Diferencial.
c) Normal.
d) Sequencial.
e) Sazonal.


Comentários:

Se cada cópia horária deve conter todos os arquivos modificados desde a cópia de 6h da manhã (que foi um backup completo), então trata-se de um backup diferencial.

Gabarito: Letra B

51. (CESPE  /  EMAP  -  2015) O  uso  do  becape  em  nuvem  para  sistemas  de  armazenamento  de imagens  tem  como  vantagem  a  salvaguarda  das  cópias em  ambientes  fisicamente  seguros  e geograficamente distantes.

Comentários:

Perfeito, perfeito, perfeito! O armazenamento em nuvem nos dá essa grande vantagem!
Gabarito: Correto

52. (CESPE / MS - 2013) A restauração completa de um sistema levará mais tempo com o uso do becape diferencial que com o do becape completo.

Comentários:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







46
82



Correto! Para restaurar um sistema com base em um becape completo, basta restaurar o becape do dia anterior. Para restaurar um sistema com base em um becape diferencial, deve-se restaurar o becape completo e o último becape diferencial.

Gabarito: Correto

53. (CESPE / MS - 2013) O becape incremental requer o uso de maior espaço para armazenamento que o becape diferencial.

Comentários:

Noooope!  O  becape  diferencial  não  desmarca  o  atributo  de  arquivamento,  logo  ele  acumula  as mudanças. Já o becape incremental desmarca o atributo de arquivamento, logo ele não acumula as mudanças, ele só copia os arquivos salvos e modificados.

Gabarito: Errado

54. (CESPE  /  MPU  -  2013) O  becape  completo  deve  ser  realizado  com  maior  frequência  que  o becape incremental.

Comentários:

Galera, lembrem-se que o becape completo leva muuuuuito tempo para ser realizado, logo ele não é indicado para ser realizado com grande frequência. O ideal é fazer um backup completo e vários becapes incrementais ou diferenciais – esses, sim, devem ocorrer com maior frequência.

Gabarito:
Errado

55. (CESPE / TJ-CE - 2014) A respeito de becape, assinale a opção correta.

a)  No  planejamento  de  uma  política  de  becape,  deve-se  considerar  a  verificação  da periodicidade e da quantidade de dados a serem armazenados.

b) A realização periódica de teste de restauração não é considerada uma boa prática de becape, ainda que os dados estejam armazenados em fitas.

c) Na medição do desempenho do becape, não se deve considerar a mídia utilizada.

d) Não é recomendado que se utilizem discos rígidos para armazenar becapes.

e) Os dispositivos ópticos são os melhores hardware disponíveis para a gravação de cópias de segurança no caso de ser necessário o armazenamento de grandes volumes de dados.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







47
82



Comentários:

(a) Correto. É claro que se deve considerar a verificação da periodicidade e da quantidade de dados a  serem  armazenados;  (b)  Errado.  É  claro  que  é  recomendável!  O  teste  de  restauração  testa  a eficiência  da  eventual  restauração  de  um  becape  e  é  recomendável  que  seja  realizado periodicamente; (c) Errado. É claro que devemos considerar a mídia utilizada – para cada mídia, o desempenho  do  becape  é  diferente;  (d)  Errado.  Essa é  uma  das  mídias  recomendadas  para armazenar becapes; (e) Errado. Para grandes volumes de dados, são recomendadas mídias como as fitas magnéticas.

Gabarito: Letra A

56. (CESPE / TRE-RS - 2015) Assinale a opção correta relativamente a becapes.

a) Compressão e encriptação são opções relevantes nas estratégias de becape para colaborar na economia de espaço de armazenamento e largura de banda e na confidencialidade de dados sensíveis da organização.

b)  As  desvantagens  dos  becapes  full  incluem  o  demorado  tempo  para  as  restaurações  e  a complexidade de gerenciamento dos itens que devem ser incluídos nas cópias de segurança.

c) Os becapes incrementais incluem os arquivos que foram alterados desde o último becape full;
os processos de restauração daqueles são mais rápidos que os destes.

d)  Nos  becapes  diferenciais,  o  uso  do  espaço  de  armazenamento  é  mais  eficiente  que  nos incrementais: o modelo de organização da gravação nos becapes diferenciais favorece o uso das áreas contíguas dos dispositivos de armazenamento.

e) Na estratégia de becape de dados críticos de uma organização, a opção sobre a frequência de realização  do  becape  deve  considerar  o  cenário  mediano  entre  o  pior  e  o  melhor  caso relativamente ao tempo, especificamente considerando o volume potencial de dados perdidos, a probabilidade estatística de um sinistro e o tempo médio para restauração do becape.

Comentários:

(a) Correto. Galera, esse item está impecável! A compressão de dados colabora para a economia de espaço de armazenamento e a largura de banda colabora na confidencialidade de dados sensíveis da  organização;  (b)  Errado.  Becape  Full  demoram  pouco  tempo  para  restaurar  e  tem  uma  baixa complexidade de gerenciamento – para restaurar, basta utilizar o último becape full; (c) Errado. Os processos de restauração de becapes incrementais são mais lentos que os de becape full; (d) Errado.
Nos  becapes  incrementais,  o  uso  do  espaço  de  armazenamento  é  mais  eficiente  que  nos diferenciais;  (e)  Errado.  A  estratégia  de  becape  de  dados  críticos  de  uma  organização  deve considerar o pior cenário.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







48
82




Gabarito: Letra A

57. (CESPE / SESA-ES - 2013) Com relação a procedimentos de segurança, assinale a opção correta.

a) O becape mais seguro é o incremental, mediante o qual é copiado o arquivo original.

b)  A  vantagem  do  becape  incremental,  em  relação  aos  outros  tipos  de  becape,  é  trabalhar independentemente de outros procedimentos de becape.

c)  O  procedimento  de  becape  completo  consiste  em  copiar  todos  os  arquivos  para  a  mídia apropriada, previamente selecionada.

d) Obtém-se maior eficiência na recuperação de dados e informações, mediante a utilização em conjunto de becapes diferenciais e becapes incrementais.

e)  Para  que  arquivos  sejam  salvos  de  maneira  segura,  o  becape  deve  ser  realizado  tanto  na memória ROM quanto na memória RAM.

Comentários:

(a) Errado, a questão não fala sob qual critério é mais seguro, logo é impossível afirmar; (b) Errado, ele  depende  do  becape  completo  inicial;  (c)  Correto,  o  becape  completo  realmente  copia  os arquivos para a mídia apropriada, previamente selecionada; (d) Errado, é necessária a realização de um becape completo inicial; (e) Errado, não faz sentido armazenar becapes na Memória RAM.

Gabarito:
Letra C

58. (CESPE / TRE-BA - 2017) A política atual de becape de determinada organização consiste em um becape completo feito todos os domingos; e becapes incrementais realizados de segunda a sábado. Considerando que, todos os dias, haja entrada de novos dados e que, também todos os dias, seja efetuado becape, assinale a opção correta acerca dessa situação hipotética.

a) Se o becape incremental for substituído pelo becape diferencial, passar-se-á a ocupar menos espaço de memória a cada becape diário, mas o tempo de execução do restore será aumentado.

b)  Sob  a  referida política  atual  de  becape,  para  a garantia  da  totalidade  e  da  integridade dos arquivos em eventual operação de restauração, será obrigatório acrescentar à rotina um becape diferencial para cada becape incremental.

c) Se o becape incremental fosse substituído pelo becape completo, além da ocupação de menor espaço de memória a cada becape diário, a execução do restore seria mais rápida.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







49
82



d)  Caso,  em  determinada  semana,  seja  necessário  restaurar  o  becape  até  quinta-feira,  será suficiente o becape da sexta-feira dessa mesma semana.

e) Caso se tivesse optado pelo becape diferencial em lugar do becape incremental e, nesse novo cenário hipotético, houvesse a necessidade de restaurar o becape até sexta-feira, bastaria, para isso, dispor dos arquivos completos e do dessa sexta-feira.

Comentários:

(a)  Errado,  o  becape  diferencial  ocupa  mais  espaço;  (b)  Errado,  o  backup  incremental  permite  a recuperação  e  a  integralidade  dos  dados  recuperados,  sem  necessidade  de  que  se  faça  qualquer outro  tipo  de  backup  diário  além  do  previsto  no  método  de  backup  incremental;  (c)  Errado,  o becape  completo  ocuparia  mais  espaço;  (d)  Errado,  para  uma  política  de  backup  incremental,  a restauração  vai  precisar  do  backup  completo  +  todos  backups  incrementais;  (e)  Correto.  Para  a recuperação  de  um  backup  diferencial,  basta  usar  o último  backup  completo  e  o  último  backup diferencial.  No  caso  apresentado,  será  necessário  utilizar  o  backup  diferencial  da  própria  sexta- feira.

Gabarito:
Letra E

59. (CESPE / SERPRO - 2013) Para  recuperar  um  sistema  em  que  eram  feitos  ciclos  de  becape compostos por becape normal e becapes incrementais, deve-se usar o último incremental, que conterá todos os dados.

Comentários:

Na verdade, deve-se usar o último becape completo e todos os becapes incrementais.

Gabarito:
Errado

60. (CESPE / MS - 2013) Se for executado, na segunda-feira, um becape completo e, nos outros dias em que a política ocorre, for feito becape diferencial, então um arquivo criado na terça-feira será incluído somente em um dos becapes.

Comentários:

Na verdade, os dados modificados da terça estarão em todos os becapes diferenciais da semana.

Gabarito: Errado

61. (CESPE / PC-AL - 2012) Em virtude de todos os becapes diferenciais executados incluírem todos os arquivos alterados desde o último becape completo, a recuperação de dados é mais rápida utilizando-se becapes diferenciais do que becapes incrementais.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







50
82




Comentários:

Perfeito! Para recuperar becapes diferenciais, basta o último becape completo e o último becape diferencial – os becapes incrementais precisariam de todos os becapes incrementais.

Gabarito: Correto

62. (CESPE / TJ-SE - 2015) Os níveis de granularidade de um becape são completo, diferencial e aleatório.

Comentários:

Os becapes podem ser classificados como completos, diferenciais e incrementais – aleatório, não!

Gabarito: Errado

63. (CESPE / UNIPAMPA - 2015) A frequência com que se realiza becape tende a variar conforme o nível de atualização e(ou) de criação de arquivos.

Comentários:

Galera, o ideal é que becapes estejam sempre atualizados! Se há um alto nível de atualização e/ou criação de arquivos, a frequência de realização de becapes também tendem a variar.

Gabarito: Correto

64. (CESPE / TRF – 1ª Região - 2017) Uma organização que prioriza a eficiência e a otimização no uso do espaço de armazenamento dos becapes de dados deve adotar estratégias embasadas em becapes completos e em becapes diferenciais combinados.

Comentários:

Claro que não! Deve-se priorizar estratégias embasadas em becapes diferenciais (ou incrementais) e, não, becapes completos.

Gabarito: Errado

65. (CESPE / BACEN - 2013) Tanto  o  becape  incremental,  quanto  o  diferencial  copiam  arquivos criados  ou  alterados  desde  o  último  becape normal, e  o  becape incremental não  desmarca  o atributo de arquivo.

Comentários:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







51
82




Na verdade, o becape incremental desmarca o atributo de arquivo – é o becape diferencial que não desmarca o atributo de arquivo.

Gabarito: Errado

66. (CESPE / SERPRO – 2013) Becape quente e frio são métodos utilizados em equipamentos com e sem refrigeração, respectivamente.

Comentários:

Hahaha... não, galera! Bacape Quente (Hot Backup) é aquele que pode ser executado sem que seja necessário interromper as atividades do banco de dados (Online). Já o Becape Frio (Cold Backup) exige a parada das atividades do banco de dados (Offline) para a sua realização.

Gabarito: Errado

67. (CESPE  /  UNIPAMPA  -  2013) O  becape  incremental,  procedimento  mediante  o  qual são copiados apenas os arquivos criados ou alterados desde o último becape, é mais demorado e seguro que o becape completo, pois, por intermédio do software responsável pela cópia, são verificadas as datas de todos os arquivos para averiguar-se se eles foram alterados.

Comentários:

Errado, ele é mais rápido que o becape completo. É mais seguro? Não é possível afirmar sem indicar o critério. Além disso, a averiguação é feita pelo atributo de arquivamento e, não, por datas.

Gabarito: Errado

68. (CESPE / MPU - 2013) O  procedimento  de  becape  padrão  proporciona  confidencialidade, integridade e disponibilidade dos dados.

Comentários:

O procedimento de becape não proporciona por padrão confidencialidade dos dados. Segundo a Norma  de  Segurança  ISO  27002,  cópias  de  segurança  buscam  manter  a  integridade  e disponibilidade da informação e dos recursos de processamento de informação.

Gabarito: Errado

69. (CESPE / TCE-RO - 2013) Para executar um becape é suficiente copiar o arquivo em edição para outra pasta.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







52
82



Comentários:

Não é recomendável realizar cópias na mesma mídia de armazenamento do arquivo original, logo isso não é suficiente.

Gabarito:
Errado

70. (CESPE / TJ-SE - 2014) Mesmo com a realização de becapes totais e incrementais dos bancos de dados, é possível haver perda de dados em casos de desastres.

Comentários:

Ué, galera... claro que é possível! Um becape não vai impedir a perda de dados em casos de becape.

Gabarito:
Correto

71. (CESPE / TJ-SE - 2014) O  becape  total  de  um  banco  de  dados  permite  que  esse  banco  seja restaurado a qualquer ponto temporal específico.

Comentários:

Qualquer ponto temporal? Não, não há como restaurar dados para um ponto temporal anterior ao becape  total,  por  exemplo!  Ele  só  conseguirá  recuperar  dados  até  o  momento  da  realização  do becape.

Gabarito: Errado

72. (CESPE / CPRM - 2013) Considere que, em uma empresa, seja realizado becape de segunda- feira a sexta-feira. Considere, ainda, que seja executado becape completo na segunda-feira e que sejam executados becapes do tipo incremental de terça-feira a sexta-feira. Nessa situação, o becape realizado na quinta-feira não contemplará os dados do becape realizado na segunda- feira, mas contemplará os dados que foram modificados na quinta-feira.

Comentários:

Perfeito! Por  que?  Porque  a  recuperação  do  becape  incremental  necessita  do  último  becape completo (segunda-feira) e de todos os becapes incrementais (terça, quarta, quinta, etc). Logo, o becape  realizado  na  quinta-feira  realmente  não  contemplará  os  dados  do  becape  realizado  na segunda-feira (que foi o completo), mas contemplará os dados modificados do becape realizado na quinta-feira (incremental).

Gabarito:
Correto

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







53
82



73. (CESPE / CPRM - 2013) O becape dos dados que emprega uma combinação de becapes normal e incremental é um método mais rápido e requer menor espaço de armazenamento, em relação aos demais tipos de becape. Entretanto, por meio desse becape, a recuperação de arquivos pode tornar-se difícil e lenta, pois o conjunto de becape poderá estar armazenado em diversos discos ou fitas.

Comentários:

Perfeito!  O  becape  incremental  +  normal  é  realmente  mais  rápido  e  requer  menor  espaço  de armazenamento em relação aos demais tipos de becape. Ademais, a recuperação pode realmente ser  difícil  e  lenta  porque  a  restauração  necessita do  último  becape completo  e  todos os  becapes incrementais.

Gabarito: Correto

74. (CESPE / FUB - 2018) O becape diferencial, utilizado para diminuir a quantidade de fitas a serem lidas e gravadas, é feito a partir de um becape completo e, então, a cada dia, é feito um novo becape de todos os arquivos que foram alterados desde o último becape, seja ele completo ou não.

Comentários:

Na  verdade,  é  feito  um  novo  becape  de  todos  os  arquivos  que  foram  alterados  desde  o  último becape completo ou incremental.

Gabarito: Errado

75. (CESPE / PF - 2013) Imediatamente após a realização de um becape incremental utilizando-se um software próprio de becape, há expectativa de que esteja ajustado o flag archive de todos os arquivos originais que foram copiados para uma mídia de becape.

Comentários:

Perfeito! Após o becape incremental desmarca-se o atributo de arquivamento.

Gabarito: Correto

76. (CESPE / TCE-SC - 2016) O becape do tipo incremental provê o uso mais eficiente do espaço de armazenamento, uma vez que não gera cópias duplicadas de arquivos, porém suas restaurações são mais lentas e mais complexas em comparação aos processos dos becapes full e diferencial.

Comentários:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







54
82



Perfeito, perfeito, perfeito! Item impecável... ele realmente faz um uso mais eficiente do espaço de armazenamento  e  não  gera  duplicações  de  arquivos,  no  entanto  a  restauração  é  mais  lenta  e complexa porque necessita do último becape completo e todos os becapes incrementais.

Gabarito: Correto

77. (CESPE / SEDF - 2017) Situação hipotética: Uma organização realiza becape completo a cada 180 dias, becape incremental a cada 7 dias e realiza testes de recuperação total dos dados com restauração real do último becape a cada 45 dias. O último becape completo ocorreu há 64 dias e o último teste de recuperação total foi bem-sucedido. Assertiva: Nessa situação, se ocorrer, hoje,  um  desastre  com  o  sistema  de  armazenamento,  a  organização  poderá  garantir,  para efeitos de auditoria, que terá certeza de recuperar e restaurar os dados armazenados em becape até a data de 19 dias atrás.

Comentários:

A questão parece complexa, mas é bem simples! Se o último becape completo ocorreu há 64 dias e os testes de recuperação ocorrem a cada 45 dias, então – em caso de desastres – a organização só poderá garantir a recuperação de 19 dias atrás (64-45 = 19). Vejam um exemplo:

Dia 001 – Backup Completo ...
Dia 045 – Teste de Recuperação ...
Dia 090 – Teste de Recuperação ...
Dia 135 – Teste de Recuperação ...
Dia 180 – Exemplo de Último Backup Completo ...
Dia 225 – Teste de Recuperação ...
Dia 244 – Dia Atual
...
Dia 270 – Teste de Recuperação ...

Notem que, se o último backup completo ocorreu no dia 180, o último teste de recuperação total ocorreu no dia 225 e o dia atual é o 244, um desastre hoje recuperaria dados armazenados até o dia 225 – logo, 19 dias atrás!

Gabarito: Correto

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







55
82



78. (CESPE / ICMBIO - 2014) O  uso  do  becape  do  tipo  incremental  permite  que  sejam  copiados apenas os arquivos gravados desde o último becape normal ou incremental.

Comentários:

Perfeito!  O  becape  incremental  copia  os  arquivos  criados  ou  alterados  desde  o  último  becape normal ou incremental.

Gabarito: Correto

79. (CESPE / TJ-SE - 2014) Becapes podem ser realizados para atender a três propósitos distintos:
recuperação de desastres, recuperação operacional e arquivamento.

Comentários:

Perfeito, são todos propósitos possíveis!

Gabarito: Correto

80. (VUNESP / Pref RP - 2018) A política de backup de uma empresa estabelece como requisito principal o menor tempo para a restauração. Para atender a esse requisito, deve-se selecionar, dentre os tipos conhecidos, o backup 
a) completo.
b) diferencial.
c) diferencial+incremental.
d) incremental.
e) progressivo.

Comentários:

No incremental, a restauração do backup é mais trabalhosa. Como assim, Professor? Pensa comigo:
um backup completo é feito no domingo, e depois backups incrementais são feitos diariamente até sexta-feira. Se um disco rígido de uma máquina queima no sábado, eu precisarei comprar um novo disco  rígido,  buscar  o  backup  completo  mais  todos  os  backups  incrementais  de  segunda,  terça, quarta, quinta e sexta, e inserir tudo no disco rígido novo. Agora se eu tenho já o backup completo do dia, ele basta para recuperar os dados e, por isso, é mais rápido.

Gabarito: Letra A

81. (IDIB  / CRO  BA  –  2017) Acerca  da  realização  de  cópias  de  seguranças,  analise  as  seguintes afirmativas:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







56
82



I.  Os  backups  dos  dados  armazenados  em  um  computador  são  importantes,  não  só  para recuperar  eventuais  falhas,  mas  também  evitar  consequências  de  uma  possível  infecção  por vírus, ou de uma invasão.

II. Um backup é a cópia de dados de um dispositivo de armazenamento a outro para que possam ser restaurados em caso da perda dos dados originais.

III. Atualmente são utilizados disquetes para backup de dados nas empresas.

Analisando as afirmativas acima, marque a alternativa verdadeira.

a) Apenas as afirmativas I e II estão corretas.
b) Apenas as afirmativas II e III estão corretas.
c) Apenas a afirmativa II está correta.
d) Apenas a afirmativa I está correta.

Comentários:

Pessoal, o Backup é um serviço que garante que você pode sempre recuperar informações de forma confiável e tempestiva. Em geral, recomenda-se gravar em alguma mídia removível ou em algum local seguro em que nenhum acidente poderia danificar o original ou a cópia.

Assim, a única alternativa errada é a de número III, tendo em vista que os disquetes são dispositivos antigos e não mais utilizados.


Gabarito: Letra A

82. (IBFC  /  DIVIPREV  -  2018) Para  a  realização  de  cópias  de  segurança  (backup), um  típico armazenamento de dados magnético é o dispositivo:

a)   DVD
b)   HD
c)   BluRay
d)   SSD

Comentários:

Pessoal,  o  hard  disk  (HD)  é  um  equipamento  que  permite  o  armazenamento  de  uma  grande quantidade de dados. Dentre as opções apresentadas, ele é o mais indicado para realizar cópia de segurança, ou backup, por ser um dispositivo não volátil (mantem os dados até mesmo quando o computador  é  desligado)  e  por  permitir  que  os  dados  sejam  apagados  e  colocados  novamente, desde que respeitado seu limite de capacidade.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







57
82



Gabarito: Letra B

83. (IESES / Assistente Administrativo (CRO SC) - 2016) O tipo de backup que copia somente os arquivos alterados ou criados depois do último backup incremental é do tipo:

a) Diferencial.
b) Normal.
c) Cópia.
d) Diário.

Comentários:

Também  conhecido  como  Backup  Incremental  Cumulativo,  o  Backup  Diferencial  copia  todos  os dados que foram criados ou modificados desde o último backup completo ou incremental.

Gabarito: Letra A

84.(IESES / Técnico Judiciário (TRE MA) - 2015) Fazer uma cópia de segurança ou back-up ficou mais  fácil  hoje  em  dia.  É  possível  copiar  dados  em um  HD  externo,  pen-drive  ou  até  “nas nuvens”. Analise as afirmativas e assinale a INCORRETA:

a)  Três  estratégias  básicas  existem  para  realização  de  cópias:  incrementais,  completas  e diferenciais.

b) Cópias de segurança devem ser guardadas em local apropriado e atualizadas.

c)  Os  dados  contidos  em  discos  rígidos  podem  sofrer  danos  ou  ficar  inutilizados  por  vários motivos: choque do disco, vírus, defeito no hardware ou eliminação acidental.

d) Devido à segurança, muitas empresas preferem fazer suas cópias de segurança na nuvem ao invés de fazer localmente.

Comentários:

(a)  Correto,  todas  são  estratégias  básicas  para  cópias  de  segurança;  (b)  Correto,  essa  é  uma recomendação óbvia; (c) Correto, todas essas ocasiões podem causar danos ou inutilizar um disco rígido;  (d)  Errado,  em  termos  de  segurança,  ambos  são  igualmente  seguros  e  possuem  suas vantagens e desvantagens.

Gabarito: Letra D

85. (IESES  /  Agente  Administrativo  (CRA  SC)  -  2013) Assinale  a  alternativa  que  diz  respeito  a seguinte definição:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







58
82




“Este tipo de backup fornece um backup dos arquivos modificados desde que foi realizado um backup completo. Normalmente salva somente os arquivos que são diferentes ou novo desde o último backup completo, mas isso pode variar em diferentes programas de backup. Juntos, um backup completo e um backup desse tipo incluem todos os arquivos no computador, alterados e inalterados.”

a) Backup incremental.
b) Backup de referência.
c) Backup normal.
d) Backup diferencial.

Comentários:

Este tipo de backup fornece um backup dos arquivos modificados desde que foi realizado um backup completo. Também chamado de Total, Normal ou Full, trata-se do backup que faz uma cópia de todos os dados de uma unidade.

Gabarito:
Letra D

86. (CETAP / Prefeitura de São Miguel do Guamá/PA - 2016) Em Tecnologia da Informação é denominado backup o processo de cópia e armazenagem de dados, de modo que estes dados possam ser eventualmente recuperados em caso de perda. Leia as seguintes descrições de dois tipos de backup:

I - Copia apenas os arquivos que foram alterados ou criados desde o último backup completo, deste  modo  ocupando  maior  espaço  nas  mídias  de  armazenamento.  Contudo,  os  dados  são mais facilmente recuperados.

II  -  Faz  a  cópia  de  todos  os  arquivos  alterados  ou criados  desde  o  último  backup  (completo, diferencial ou incremental).

Assinale a alternativa correta que contém os tipos de backup de acordo com as descrições I e II, respectivamente:

a) I- Backup Completo, II- Backup Diferencial.
b) I- Backup Diferencial, II- Backup Incremental.
c) I- Backup Incremental, II- Backup Diferencial.
d) I- Backup Incremental, II- Backup Completo.

e) I- Backup Diferencial, II- Backup Completo.

Comentários:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







59
82



(I) Backups diferencial e incremental são capazes de copiar os arquivos alterados ou criados desde o  último  backup  completo,  no  entanto  aquele  que  ocupa  maior  espaço  de  armazenamento  é  o backup é o backup diferencial;

(II) A banca deu como resposta Backup Incremental, no entanto eu discordo veementemente visto que esse tipo de backup não copia dados desde o backup diferencial anterior. Na minha opinião, caberia recurso!

Gabarito: Letra B
































Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







60
82



LISTA DE QUESTÕES

1. (CESPE  /  IFF  /  Conhecimento  Gerais  -  2018) Na  primeira  vez  que  se  realiza  uma  cópia  de segurança, seja de um servidor ou de um computador pessoal, o tipo de becape mais indicado é o:

a) diferencial.
b) incremental
c) periódico.
d) diário.
e) completo.

2. (FCC / SABESP/ Estagiário - 2017) Uma organização possui a política de realizar backup todos os  dias  e  todos  os  dados  são  copiados  diariamente, independentemente  de  terem  sido modificados ou não, para dispositivos do tipo fita magnética, disco magnético ou óptico, DVD ou blu-ray. Esta organização realiza backup do tipo:

a) completo
b) incremental
c) diferencial
d) progressivo
e) cumulativo

3. (CESPE  /  PC-GO  /  Agente  de  Polícia  -  2016) Com  relação  aos  procedimentos  de  becape, assinale a opção correta.

a) O becape incremental deve ser feito depois de realizada cópia completa de todos os arquivos de interesse.

b) A cópia completa deve ser feita periodicamente, para copiar os arquivos que sofreram alguma modificação na última cópia incremental.

c)  Na  cópia  incremental,  não  é  necessário  especificar  os  intervalos  de  tempo  em  que  houve alterações nos arquivos.

d) O becape incremental não utiliza dados recuperados das cópias completas.

e)    Na    cópia    incremental,    os    arquivos    copiados    anteriormente    são    recopiados, independentemente do ponto de recuperação definido.



Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







61
82



4. IBFC  /  MGS/  Técnico  em  Informática  -  2016) Um  backup  incremental  copia  somente  os arquivos criados ou alterados desde o último backup normal ou incremental, e os marca como arquivos que passaram por backup. Portanto:

a) o atributo de arquivo não é desmarcado.
b) o atributo e a seguridade do arquivo não é desmarcado.
c) o atributo de arquivo é desmarcado.
d) o atributo e a seguridade do arquivo é desmarcado.


5. (FCC / DPE-SP/ Oficial de Defensoria Pública - 2015) Marcos Paulo fez um backup incremental de seus arquivos. Ele aplicou uma função que copia:

a)  somente os arquivos criados ou alterados desde o último backup normal ou incremental e os marca como arquivos que passaram por backup (o atributo de arquivo é desmarcado).

b) todos os arquivos selecionados e os marca como arquivos que passaram por backup (ou seja, o atributo de arquivo é desmarcado).

c) todos os arquivos selecionados que foram modificados no dia de execução do backup diário.

d) todos os arquivos selecionados, mas não os marca como arquivos que passaram por backup (ou seja, o atributo de arquivo não é desmarcado).

e) arquivos criados ou alterados desde o último backup normal ou incremental. Não marca os arquivos como arquivos que passaram por backup (o atributo de arquivo não é desmarcado).


6. (VUNESP / CM PRADÓPOLIS – 2016) Ao manipular arquivos e pastas, é importante ter cópias de segurança dos arquivos e pastas utilizados. O MS-Windows 7, em sua configuração padrão, possui recursos para fazer cópias de segurança de arquivos e pastas. Assinale a alternativa que contém o nome dado ao procedimento de cópias de segurança.

a) Limpeza de Disco.
b) Clone.
c) Sincronização.
d) Fragmentação.
e) Backup.

7. (VUNESP / PC SP – 2014) Recomenda-se que um usuário de computador sempre tenha uma cópia  de  segurança  de  seus  arquivos.  A  operação  que  realiza  este  procedimento  é  conhecida como:

a) Digitalização.
b) Codificação.
c) Certificação Digital.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







62
82



d) Decodificação.
e) Backup.

8. (CRESCER CONSULTORIAS / Prefeitura de Lagoa Alegre – PI – 2019) Fazer backup de  100 gigabytes de dados todas as noites quando talvez 10 gigabytes de dados foram alterados não é uma boa prática. Por este motivo, que tipo de backup deve ser utilizado?

a) Backup Completo
b) Backup Diferencial c) Backup Incremental d) Backup Delta

9. (QUADRIX / CRESS-SC – 2019) O backup é um procedimento no qual os dados são copiados, preferencialmente, de um dispositivo para outro.

10. (FADESP  /  DETRAN-PA  –  2019) Com  relação  aos  tipos  de  backup,  analise  as  seguintes afirmativas.

I. O backup completo faz a cópia de todos os arquivos destinados a ele, independente de versões anteriores ou de alterações nos arquivos desde o último backup.

II. O backup incremental faz a cópia dos arquivos que foram alterados ou criados desde o último backup completo ou incremental.

III. Da mesma forma que o backup incremental, o backup diferencial só copia arquivos criados ou  alterados  desde  o  último  backup.  No  entanto,  a  diferença  deste para  o  incremental  é  que cada backup diferencial mapeia as modificações em relação ao último backup completo.

A sequência que expressa corretamente o julgamento das afirmativas é:

a) I – F; II – F; III – V.
b) I – V; II – F; III – F.
c) I – V; II – V; III – F.
d) I – V; II – V; III – V.
e) I – F; II – F; III – F.

11. (IBFC / MGS – 2019) Quanto aos conceitos básicos referentes às cópias de segurança (backup), analise as afirmativas abaixo, dê valores Verdadeiro (V) ou Falso (F):

( ) o backup diferencial armazena todos os dados alterados desde o último backup full.
( ) o backup incremental proporciona na sua execução o maior tempo, e de mídia, de backup.
( ) no backup diferencial, a recuperação de dados necessita de vários conjuntos de mídia.

Assinale a alternativa que apresenta a sequência correta de cima para baixo.:
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA ==12b2d8==








63
82




a) V - F - F
b) V - V - F
c) F - V - V
d) F - F - V

12. (IBADE / Câmara de Porto Velho – 2018) O backup é vital para a preservação dos dados. Com o  objetivo  de  ganhar  eficiência  foi  criada  uma  técnica  grava  apenas  as  alterações  ocorridas desde o último backup e assim sucessivamente. A esse tipo de backup dá-se o nome de:

a) Journal.
b) Full.
c) Incremental.
d) Diferencial.
e) Molecular.

13. (CESPE / FUB – 2018) O becape diferencial, utilizado para diminuir a quantidade de fitas a serem lidas e gravadas, é feito a partir de um becape completo e, então, a cada dia, é feito um novo becape de todos os arquivos que foram alterados desde o último becape, seja ele completo ou não.

14. (CONSULPAM  /  Câmara  de  Juiz  de  Fora  –  MG  –  2018) Fazer  backup  de  um  computador significa,  basicamente,  realizar  uma  cópia  de  segurança.  Este  é  um  processo  para  salvar documentos  importantes  e  manter  arquivos  pessoais  protegidos,  em  caso  de  eventuais problemas. Podemos fazer backup utilizando, EXCETO:

a) DVD.
b) Impressoras.
c) HD externo.
d) CD.

15. (FAUGRS / TJ-RS - 2018) Como se denomina o tipo de backup que contém somente arquivos que    foram    criados    (novos)    ou    modificados    desde    o    último    backup    realizado, independentemente do tipo deste último backup?

a) Diferencial.
b) Incremental.
c) Completo.
d) Espelhamento (mirroring).
e) Inteligente.


Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







64
82



16. (AOCP / TRT-1ª Região – 2018) O backup de arquivos é altamente recomendado para prevenir a perda de dados importantes. Dos recursos apresentados a seguir, qual NÃO serve para fazer backup de arquivos?


a) Flash drive.
b) Memória RAM.
c) HD externo.
d) Nuvem.
e) Fita magnética.


17. (FADESP / BANPARÁ – 2018) Sobre cópias de segurança (backup) é correto afirmar que:

a) o backup diferencial realiza uma cópia completa de todos os dados.
b)  sistemas  de  recuperação  de  backup  utilizam  banco  de  dados  sem  operação  dos  usuários quando realiza um backup.
c) o backup incremental utiliza mais espaço em disco que outros tipos de backup.
d) sistemas de recuperação de backup utilizam jobs para gerenciar o tempo e os tipos de backup realizados.
e) o backup diferencial é o mais seguro dos tipos de backup.


18. (CESGRANRIO / BANCO DA AMAZÔNIA - 2018) O gerente de sistemas pediu que o analista fizesse um backup diferencial. Sendo assim, ele deve fazer um backup também chamado de:

a) Backup incremental b) Backup completo (full) c) Backup full deduplicado d) Backup em array de discos e) Backup incremental cumulativo 
19. (COMPERVE  /  SESAP/RN  –  2018) O  backup  é  um  procedimento  realizado  para  garantir a segurança de dados em sistemas computacionais. A cerca desse procedimento, foram feitas as afirmações seguintes.

I Recomenda-se realizar o backup de uma partição em outra partição no mesmo disco, uma vez que, havendo falha no disco, os dados serão facilmente recuperados.

II O primeiro backup criado para preservar os dados de um sistema é o backup diferencial.

III O backup incremental copia apenas os arquivos criados ou modificados desde o último backup normal.

IV Realizar backups diferenciais ou incrementais requer menos espaço de armazenamento que o backup normal.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







65
82



Das afirmações, estão corretas 
a) II e III.
b) I e II.
c) III e IV.
d) I e IV.

20. (IBFC  /  Pref.  Divinópolis/MG  -  2018) Assinale  a  alternativa  que  completa  correta  e respectivamente a lacuna da frase a seguir:

“Um  backup  ___________  copia  somente  os  arquivos  criados  ou  alterados  desde  o  último backup normal ou incremental, e os marca como arquivos que passaram por backup (o atributo de arquivo é desmarcado)”.

a)  Integral
b) de Cópia
c) Incremental
d) Diferencial

21. (UECE-CEV  /  DETRAN-CE  -  2018) Como  política  de  segurança  e  recuperação  de  dados, é recomendável realizar uma cópia dos arquivos e pastas alterados desde o último backup. Essa cópia de segurança é denominada:

a) atualização do sistema.
b) backup incremental.
c) compressão de dados.
d) volatilidade da informação.


22. (COPERVE-UFSC / UFSC - 2018) Sobre os tipos de backup (cópias de segurança) de arquivos, é correto afirmar que:

a) no backup incremental são copiados os arquivos desde o último backup completo, ou seja, isso não se aplica a backups incrementais e diferenciais.

b) no backup completo, no qual todos os arquivos são copiados, as vantagens são a rapidez na realização  do  backup  e  na  recuperação,  e  a  desvantagem  é  o  espaço  utilizado  para armazenamento.

c)  a  maior  desvantagem  do  backup  incremental  é  que seu  processo  de  recuperação  é  mais complexo e lento, pois são recuperadas as informações do último backup completo, seguido de todos os backups incrementais até o momento da falha.

d) no backup diferencial são copiados todos os dados alterados desde o último backup completo ou incremental.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







66
82




e) a vantagem do backup diferencial sobre o incremental é que são armazenados menos dados desde o último backup completo.


23. (FCC / DPE-AM - 2018) Uma das vantagens de escolher o Backup do tipo diferencial, para ser adotado na Defensoria, é:

a) A recuperação requerer apenas o último Backup diferencial e o último Backup completo.
b) A menor quantidade de dados armazenado se comparado com o Backup incremental.
c) Requerer menor tempo de recuperação se comparado ao Backup completo.
d) A maior tolerância a falhas se comparado com o Backup completo.
e) Requerer um tempo menor para realizar o Backup se comparado com o Backup incremental.

24. (FCC  /  TRF-5ª  Região  -  2017) Dentre  os  vários  tipos  de  backup,  o  Técnico  escolheu  o  tipo Diferencial, pois:

a) ocupa menos espaço de armazenamento se comparado com o backup do tipo Incremental.

b)  a  velocidade  para  a  recuperação  do  backup  é  maior,  se  comparada  com  a  do  backup completo.

c) os tamanhos dos backups diferenciais não crescem progressivamente como ocorre no backup incremental.

d)  cada  backup  diferencial  armazena  apenas  as  modificações  realizadas  desde  o  backup diferencial anterior.

e)  para  a  recuperação  são  necessários  apenas  o  último  backup  completo  e  o  último  backup diferencial.


25. (FCC / TST – 2017) Em  uma  situação  hipotética,  um  Analista  de  Suporte em  Tecnologia  da Informação deve escolher o tipo de Backup a ser utilizado no TST. Para tanto, deve considerar que:


a)  para  a  recuperação  dos  dados  de  um  backup  diferencial  são  necessários  apenas  o  último backup diferencial e o último backup completo.

b) a recuperação dos dados de um backup diferencial é mais seguro e integro que em um backup completo.

c) o backup incremental ocupa mais espaço de armazenamento se comparado com o backup diferencial.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







67
82



d)  para  a  recuperação  dos  dados  de  um  backup  incremental  são necessários  apenas  o  último backup incremental e o último backup completo.

e) a recuperação dos dados de um backup do tipo completo é mais demorado que em um backup incremental.


26. (IBFC / TJ-PE – 2017) Considerando os conceitos de cópias de segurança, ficou-se em dúvida quanto ao atributo de arquivo ser marcado ou não. Os tipos de arquivos nos quais o atributo de arquivo é desmarcado são:

a) Backup Incremental e o Backup Diferencial b) Backup Diferencial e o Backup Diário c) Backup Diário e o Backup Normal d) Backup Diferencial e o Backup Normal e) Backup Incremental e o Backup Normal 
27. (QUADRIX / CONTER – 2017) Com relação aos tipos e formas de backup, leia as afirmativas a seguir.

I.  O  backup  incremental  é  a  cópia  de  todos  os  dados  que  foram  modificados  desde  o  último backup de qualquer tipo.

II.  No  backup  diferencial,  com  exceção  da  primeira execução,  quando  é  semelhante  ao incremental, serão copiados todos os dados alterados desde o backup completo anterior.

III.  A  operação  de  um  hot  backup  tem  como  característica  permitir  que  o  sistema  possa permanecer em execução enquanto é realizada.

Está correto o que se afirma em:

a) I e II, somente.
b) II e III, somente.
c) I e III, somente.
d) todas.
e) nenhuma.


28. (QUADRIX  /  CONTER  –  2017) Caso  o  usuário  deseje  realizar  a  cópia  de  todos  os arquivos disponíveis em seu computador para o dispositivo de backup, independentemente de versões anteriores ou de alterações nos arquivos desde a última cópia de segurança, o tipo de backup mais indicado será o:

a) completo.
b) incremental.
c) diferencial.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







68
82



d) contínuo.
e) periódico.

29. (FCC / ARTESP – 2017) Considere, por hipótese, que a ARTESP utiliza uma estratégia de backup conforme mostra a figura abaixo, na qual a escala vertical representa a quantidade de dados.



A figura ilustra a estratégia de backup ..I.., que é semelhante a um backup ..II.. na primeira vez em  que  é  realizado,  na  medida  em  que  irá  copiar  todos  os  dados  alterados  desde  o  backup anterior. No entanto, cada vez que é executado após o primeiro backup, serão copiados todos os dados alterados desde o backup ..III.. anterior e não com relação ao último backup.

As lacunas I, II e III são preenchidas, correta e respectivamente, por:

a) diferencial − incremental − completo b) diferencial − completo − incremental c) incremental − completo − completo d) incremental − diferencial − diferencial e) completo − diferencial − incremental 
30. (EDUCA / CRQ-19ª Região - 2017) Backup é uma cópia de segurança. O termo em inglês é muito utilizado por empresas e pessoas que guardam documentos, imagens, vídeos e outros arquivos no  computador  ou  na  nuvem,  hospedados  em  redes  online  como  Dropbox  e  Google  Drive.
Podemos dividir o termo BACKUP em alguns tópicos.

Assinale a alternativa CORRETA que apresenta o tipos de backup:

I. Backup Completo (Full).
II. Backup Diferencial.
III. Backup Incremental.
IV. Backup Intermediário.
V. Backup Suplementar.

Estão CORRETAS:

a) I e II apenas.
b) I, II e III apenas.
c) III, IV e V apenas.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







69
82



d) II e V apenas.
e) I, II, III e V apenas.

31. (IBFC / EBSERH - 2017) A  maioria  das  políticas  de  backup  empregam  o  conceito  de  backup completo, backup incremental e backup diferencial. Se desejarmos que no momento de restore de  dados  seja  utilizado  o  menor  número  de  mídias,  uma  boa  prática/política  para  dados estratégicos empresariais seria de realizar:

a) um backup completo mensal e um backup diferencial diário b) um backup completo mensal e um backup incremental semanal c) um backup diferencial semanal e backup incremental diário d) um backup completo mensal e um backup incremental diário e) um backup incremental mensal e backup diferencial semanal 
32. (CRO-SC / CRO-SC - 2016) Sobre o tipo de backup que copia somente os arquivos alterados ou criados depois do último backup incremental é do tipo:

a) Diferencial.
b) Diário.
c) Cópia.
d) Normal.

33. (FCC / TRT-20ª Região - 2016) Um backup completo é executado na sexta-feira e um backup incremental  é  executado  todos  os  dias  a  partir  deste  dia.  No  sábado  são  acrescentados  5 arquivos,  que  são  copiados  no  backup  incremental.  No  domingo  alguns  arquivos  são modificados e somente estes arquivos são copiados no backup incremental. Na segunda-feira os dados do sistema são corrompidos, havendo a necessidade de restauração a partir do backup.
Pode-se concluir que, para restaurar os dados ao estado imediatamente anterior à ocorrência do problema, será necessário restaurar:

a) apenas os backups incrementais realizados.
b) todos os backups completos já realizados no sistema até segunda-feira.
c) apenas os backups incrementais realizados no sábado e no domingo.
d)  somente  o  backup  completo  realizado  na  sexta-feira  e  o  backup  incremental  realizado  no domingo.
e) o backup completo e todos os backups incrementais realizados no período em questão.


34. (INAZ DO PARÁ / Prefeitura de Jacundá - PA - 2016) Backup  é  um  termo inglês  que  tem  o significado de cópia de segurança. Como se chama o backup que contém apenas os arquivos que foram criados ou modificados a partir do último backup realizado, e que, depois de fazer a cópia do arquivo, desmarca o atributo (flag) de arquivamento?

a) Diferencial
b) Incremental
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







70
82



c) Completo
d) Seletivo
e) Full


35. (IBFC / EBSERH - 2016) Assinale, das alternativas abaixo, a única que identifica corretamente o tipo de backup que na realização de um restore será necessário apenas o último backup full e, dos vários backups realizados depois do full, somente o último backup:

a) matricial
b) incremental
c) diário
d) diferencial
e) linear


36. (IBFC / EBSERH - 2016) Existem  vários  tipos  de  backup.  Assinale,  das  alternativas  abaixo,  o backup que tem como principal característica a de copiar todos os dados que foram modificados desde o último backup de qualquer tipo:

a) diário
b) full
c) diferencial
d) normal
e) incremental


37. (COPEVE-UFAL / UFAL - 2016) Dadas as afirmativas sobre os conceitos de backup de dados, 
I. O objetivo do backup é fazer cópias de todos os arquivos do sistema operacional.
II. O objetivo do backup é fazer cópias de arquivos do usuário.
III. Os backups podem ser do tipo completo ou normal, diferencial e incremental.
IV.  O  primeiro  backup  diferencial  e  o  primeiro  backup  incremental  terão  o  mesmo  conteúdo (backup completo), porém, a partir do segundo ciclo de cópia, o backup diferencial tem como base o último backup completo, ao passo que o backup incremental tem como base os dados copiados na fase anterior de um backup incremental.

Verifica-se que estão corretas apenas:

a) I e II.
b) I e III.
c) III e IV.
d) I, II e IV.
e) II, III e IV.


38. (IDECAN / UERN - 2016) Analise as afirmativas sobre procedimentos de backup.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







71
82



I.  O  backup  de  cópia  copia  todos  os  arquivos  selecionados  e  os  marca  como  arquivos  que passaram por backup.

II. O backup diferencial copia arquivos criados ou alterados desde o último backup normal ou incremental e os marca como arquivos que passaram por backup.

III.O backup incremental copia somente os arquivos criados ou alterados desde o último backup normal ou incremental e os marca como arquivos que passaram por backup.

Está(ão) correta(s) apenas a(s) afirmativa(s):

a) I.
b) II.
c) III.
d) II e III.


39. (Instituto Legatus / Prefeitura de Passagem Franca do Piauí – PI - 2016) “Trata-se  de uma cópia de segurança dos dados ou programas que permite restaurar elementos perdidos em caso de uma falha ou perda dos dados”. O texto fala da técnica conhecida como:

a) backup
b) dashboard
c) recovery
d) firmware
e) temporary


40. (IESES  /  BAHIAGÁS  -  2016) Considere  o  cenário  apresentado  a  seguir,  no  qual  um administrador de sistemas realizou as seguintes tarefas de backup na pasta "COMPRAS":

Dia 01 23:59 - Backup Full 1 Dia 02 23:59 - Backup Diferencial 1 Dia 03 23:59 - Backup Full 2 Dia 04 23:59 - Backup Diferencial 2 Dia 05 23:59 - Backup Diferencial 3 
No  dia  06  alguém  excluiu  acidentalmente  toda  a  pasta  e  o  administrador  precisa  recuperar  a mesma no estado que ela se encontrava no dia 05. Sendo assim, quais backups ele necessitará para realizar o restore (rotina de recuperação dos arquivos)?

a) Backup Full 1 e Backup Full 2.
b) Somente o Backup Full 2 c) Backup Full 1, Backup Diferencial 1, Backup Diferencial 2.
d) Backup Full 1 e Backup Diferencial 1.
e) Backup Full 2 e Backup Diferencial 3.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







72
82



41. (FCC  /  DPE-RR  -  2015) Os  backups  realizados  para  atender  aos  requisitos  de  arquivamento podem ser categorizados como completos, incrementais e diferenciais. O backup incremental:

a) copia os dados que foram modificados desde o último backup completo ou incremental, o que for mais recente.

b) é bem mais lento do que o backup completo, pois é necessário selecionar cada arquivo que foi modificado desde o último backup completo.

c) copia todos os dados nos volumes de produção, indistintamente, porém, em alta velocidade.

d) é, dentre os tipos de backup, o mais lento e que necessita de mais espaço de armazenamento, porém, a restauração é muito rápida.

e)  copia  os  dados  que  foram  modificados  desde  o  último  backup,  sendo  mais  lento  do  que  o backup diferencial, porém, mais rápido na restauração dos dados.

42. (FCC  /  TRE-PB  -  2015) Considere  que  o  administrador  de  um  servidor  adotou  a  política  de backup  que  utiliza  a  combinação  do  backup  normal  e incremental.  Para  que  o  administrador possa restaurar os dados, ele precisará:

a) de todos os conjuntos de backups normais e de todos os conjuntos de backups incrementais.
b) de todos os conjuntos de backups normais e apenas do último backup incremental.
c) apenas do último backup normal e do último backup incremental.
d) apenas do último backup normal e de todos os conjuntos de backups incrementais.
e) apenas do último backup incremental.


43. (FCC / DPE-SP - 2015) Em uma semana, um backup completo é executado na noite de segunda- feira e um backup incremental é executado todas as noites seguintes, até quinta-feira. Na terça- feira, um novo arquivo é acrescentado, e não há alterações nos arquivos anteriores. Na quarta- feira,  nenhum  arquivo  é  acrescentado,  mas  um  arquivo  acrescentado  na  segunda-feira  é modificado. Na quinta-feira, um novo arquivo é acrescentado, e não há alterações nos arquivos anteriores. Na manhã de sexta-feira, há corrupção de dados, o que exige a restauração de todos os dados a partir dos backups realizados na semana. A solução correta, neste caso, é restaurar o backup:

a) realizado na quinta-feira.
b) completo e aplicar os backups incrementais realizados na terça-feira, quarta-feira e quinta- feira.
c) completo e o backup realizado na quinta-feira.
d) completo realizado na segunda-feira.
e) realizado na terça-feira, na quarta-feira e na quinta-feira, depois, o backup completo.

44. (IDECAN  /  PRODEB  -  2015) “Em  uma  empresa  de  venda  de  materiais  para  construção  é utilizado um sistema para o controle de entradas e saídas do estoque. Preocupado com o grande Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







73
82



volume de dados e a importância desses para a organização, o dono do empreendimento optou por contratar uma empresa de serviços de informática para montar uma estrutura de backup dos dados. Após um estudo dos processos da empresa, os profissionais contratados montaram uma estrutura que realiza semanalmente uma cópia completa com todos os dados selecionados e  em  paralelo  outra  que,  duas  vezes  por  dia,  copia somente  os  dados  que  foram  criados  ou alterados  desde  o  último  backup  completo.”  Os  profissionais  criaram,  respectivamente, backups do tipo:

a) Normal e diário.
b) Total e diferencial.
c) Diferencial e diário.
d) Normal e incremental.


45. (CESPE / MEC - 2015) Diferentemente dos becapes diferenciais, os becapes incrementais são acumulativos.

46. (CESPE  /  MEC  -  2015) O  becape  incremental  copia  apenas  os  arquivos  que  não  foram modificados desde o último becape.

47. (CESPE / MEC - 2015) Um becape completo consiste na cópia de todos os arquivos para a mídia de becape.

48.(IESES  /  TRE-MA  -  2015) Assinale  a  alternativa  correta  com  relação  aos  tipos  de  backup existentes.

a) Total; Parcial e Diário.
b) Normal; Cópia e Diferencial.
c) Completo; Diário e Incremental.
d) Completo; Incremental; Diferencial.

49. (IESES  /  TRE-MA  -  2015) Assinale  a  alternativa  correta  com  relação  a  definição  de  backup incremental e diferencial.

a) No backup incremental o tamanho dos arquivos é maior e o tempo para restauração também é menor.

b) No backup diferencial o tamanho dos arquivos é maior e o tempo para restauração também maior.

c) No backup incremental o tamanho dos arquivos é menor e o tempo para restauração também é menor.

d)  O  backup  diferencial  é  feito  com  base  nas  alterações  desde  o  último  backup  completo,  o tamanho do backup vai aumentando progressivamente.
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







74
82




50. (PR-4 UFRJ / UFRJ - 2015) Um  administrador  de  servidores  deseja  realizar  um  processo  de backup que inclui a realização de uma cópia completa de todos os arquivos de um determinado volume às 06 horas da manhã, e cópias horárias entre 07 e 22 horas que contenham, cada uma delas, todos os arquivos modificados desde a cópia das 06 horas. O tipo de backup das cópias horárias deverá ser:

a) Incremental.
b) Diferencial.
c) Normal.
d) Sequencial.
e) Sazonal.


51. (CESPE  /  EMAP  -  2015) O  uso  do  becape  em  nuvem  para  sistemas  de  armazenamento  de imagens  tem  como  vantagem  a  salvaguarda  das  cópias em  ambientes  fisicamente  seguros  e geograficamente distantes.

52. (CESPE / MS - 2013) A restauração completa de um sistema levará mais tempo com o uso do becape diferencial que com o do becape completo.

53. (CESPE / MS - 2013) O becape incremental requer o uso de maior espaço para armazenamento que o becape diferencial.

54. (CESPE  /  MPU  -  2013) O  becape  completo  deve  ser  realizado  com  maior  frequência  que  o becape incremental.

55. (CESPE / TJ-CE - 2014) A respeito de becape, assinale a opção correta.

a)  No  planejamento  de  uma  política  de  becape,  deve-se  considerar  a  verificação  da periodicidade e da quantidade de dados a serem armazenados.

b) A realização periódica de teste de restauração não é considerada uma boa prática de becape, ainda que os dados estejam armazenados em fitas.

c) Na medição do desempenho do becape, não se deve considerar a mídia utilizada.

d) Não é recomendado que se utilizem discos rígidos para armazenar becapes.

e) Os dispositivos ópticos são os melhores hardware disponíveis para a gravação de cópias de segurança no caso de ser necessário o armazenamento de grandes volumes de dados.

56. (CESPE / TRE-RS - 2015) Assinale a opção correta relativamente a becapes.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







75
82



a) Compressão e encriptação são opções relevantes nas estratégias de becape para colaborar na economia de espaço de armazenamento e largura de banda e na confidencialidade de dados sensíveis da organização.

b)  As  desvantagens  dos  becapes  full  incluem  o  demorado  tempo  para  as  restaurações  e  a complexidade de gerenciamento dos itens que devem ser incluídos nas cópias de segurança.

c) Os becapes incrementais incluem os arquivos que foram alterados desde o último becape full;
os processos de restauração daqueles são mais rápidos que os destes.

d)  Nos  becapes  diferenciais,  o  uso  do  espaço  de  armazenamento  é  mais  eficiente  que  nos incrementais: o modelo de organização da gravação nos becapes diferenciais favorece o uso das áreas contíguas dos dispositivos de armazenamento.

e) Na estratégia de becape de dados críticos de uma organização, a opção sobre a frequência de realização  do  becape  deve  considerar  o  cenário  mediano  entre  o  pior  e  o  melhor  caso relativamente ao tempo, especificamente considerando o volume potencial de dados perdidos, a probabilidade estatística de um sinistro e o tempo médio para restauração do becape.

57. (CESPE / SESA-ES - 2013) Com relação a procedimentos de segurança, assinale a opção correta.

a) O becape mais seguro é o incremental, mediante o qual é copiado o arquivo original.

b)  A  vantagem  do  becape  incremental,  em  relação  aos  outros  tipos  de  becape,  é  trabalhar independentemente de outros procedimentos de becape.

c)  O  procedimento  de  becape  completo  consiste  em  copiar  todos  os  arquivos  para  a  mídia apropriada, previamente selecionada.

d) Obtém-se maior eficiência na recuperação de dados e informações, mediante a utilização em conjunto de becapes diferenciais e becapes incrementais.

e)  Para  que  arquivos  sejam  salvos  de  maneira  segura,  o  becape  deve  ser  realizado  tanto  na memória ROM quanto na memória RAM.

58. (CESPE / TRE-BA - 2017) A política atual de becape de determinada organização consiste em um becape completo feito todos os domingos; e becapes incrementais realizados de segunda a sábado. Considerando que, todos os dias, haja entrada de novos dados e que, também todos os dias, seja efetuado becape, assinale a opção correta acerca dessa situação hipotética.

a) Se o becape incremental for substituído pelo becape diferencial, passar-se-á a ocupar menos espaço de memória a cada becape diário, mas o tempo de execução do restore será aumentado.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







76
82



b)  Sob  a  referida política  atual  de  becape,  para  a garantia  da  totalidade  e  da  integridade dos arquivos em eventual operação de restauração, será obrigatório acrescentar à rotina um becape diferencial para cada becape incremental.

c) Se o becape incremental fosse substituído pelo becape completo, além da ocupação de menor espaço de memória a cada becape diário, a execução do restore seria mais rápida.

d)  Caso,  em  determinada  semana,  seja  necessário  restaurar  o  becape  até  quinta-feira,  será suficiente o becape da sexta-feira dessa mesma semana.

e) Caso se tivesse optado pelo becape diferencial em lugar do becape incremental e, nesse novo cenário hipotético, houvesse a necessidade de restaurar o becape até sexta-feira, bastaria, para isso, dispor dos arquivos completos e do dessa sexta-feira.

59. (CESPE / SERPRO - 2013) Para  recuperar  um  sistema  em  que  eram  feitos  ciclos  de  becape compostos por becape normal e becapes incrementais, deve-se usar o último incremental, que conterá todos os dados.

60. (CESPE / MS - 2013) Se for executado, na segunda-feira, um becape completo e, nos outros dias em que a política ocorre, for feito becape diferencial, então um arquivo criado na terça-feira será incluído somente em um dos becapes.

61. (CESPE / PC-AL - 2012) Em virtude de todos os becapes diferenciais executados incluírem todos os arquivos alterados desde o último becape completo, a recuperação de dados é mais rápida utilizando-se becapes diferenciais do que becapes incrementais.

62. (CESPE / TJ-SE - 2015) Os níveis de granularidade de um becape são completo, diferencial e aleatório.

63. (CESPE / UNIPAMPA - 2015) A frequência com que se realiza becape tende a variar conforme o nível de atualização e(ou) de criação de arquivos.

64. (CESPE / TRF – 1ª Região - 2017) Uma organização que prioriza a eficiência e a otimização no uso do espaço de armazenamento dos becapes de dados deve adotar estratégias embasadas em becapes completos e em becapes diferenciais combinados.

65. (CESPE / BACEN - 2013) Tanto  o  becape  incremental,  quanto  o  diferencial  copiam  arquivos criados  ou  alterados  desde  o  último  becape normal, e  o  becape incremental não  desmarca  o atributo de arquivo.

66. (CESPE / SERPRO – 2013) Becape quente e frio são métodos utilizados em equipamentos com e sem refrigeração, respectivamente.

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







77
82



67. (CESPE  /  UNIPAMPA  -  2013) O  becape  incremental,  procedimento  mediante  o  qual são copiados apenas os arquivos criados ou alterados desde o último becape, é mais demorado e seguro que o becape completo, pois, por intermédio do software responsável pela cópia, são verificadas as datas de todos os arquivos para averiguar-se se eles foram alterados.

68. (CESPE / MPU - 2013) O  procedimento  de  becape  padrão  proporciona  confidencialidade, integridade e disponibilidade dos dados.

69. (CESPE / TCE-RO - 2013) Para executar um becape é suficiente copiar o arquivo em edição para outra pasta.

70. (CESPE / TJ-SE - 2014) Mesmo com a realização de becapes totais e incrementais dos bancos de dados, é possível haver perda de dados em casos de desastres.

71. (CESPE / TJ-SE - 2014) O  becape  total  de  um  banco  de  dados  permite  que  esse  banco  seja restaurado a qualquer ponto temporal específico.

72. (CESPE / CPRM - 2013) Considere que, em uma empresa, seja realizado becape de segunda- feira a sexta-feira. Considere, ainda, que seja executado becape completo na segunda-feira e que sejam executados becapes do tipo incremental de terça-feira a sexta-feira. Nessa situação, o becape realizado na quinta-feira não contemplará os dados do becape realizado na segunda- feira, mas contemplará os dados que foram modificados na quinta-feira.

73. (CESPE / CPRM - 2013) O becape dos dados que emprega uma combinação de becapes normal e incremental é um método mais rápido e requer menor espaço de armazenamento, em relação aos demais tipos de becape. Entretanto, por meio desse becape, a recuperação de arquivos pode tornar-se difícil e lenta, pois o conjunto de becape poderá estar armazenado em diversos discos ou fitas.

74. (CESPE / FUB - 2018) O becape diferencial, utilizado para diminuir a quantidade de fitas a serem lidas e gravadas, é feito a partir de um becape completo e, então, a cada dia, é feito um novo becape de todos os arquivos que foram alterados desde o último becape, seja ele completo ou não.

75. (CESPE / PF - 2013) Imediatamente após a realização de um becape incremental utilizando-se um software próprio de becape, há expectativa de que esteja ajustado o flag archive de todos os arquivos originais que foram copiados para uma mídia de becape.

76. (CESPE / TCE-SC - 2016) O becape do tipo incremental provê o uso mais eficiente do espaço de armazenamento, uma vez que não gera cópias duplicadas de arquivos, porém suas restaurações são mais lentas e mais complexas em comparação aos processos dos becapes full e diferencial.

77. (CESPE / SEDF - 2017) Situação hipotética: Uma organização realiza becape completo a cada 180 dias, becape incremental a cada 7 dias e realiza testes de recuperação total dos dados com Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







78
82



restauração real do último becape a cada 45 dias. O último becape completo ocorreu há 64 dias e o último teste de recuperação total foi bem-sucedido. Assertiva: Nessa situação, se ocorrer, hoje,  um  desastre  com  o  sistema  de  armazenamento,  a  organização  poderá  garantir,  para efeitos de auditoria, que terá certeza de recuperar e restaurar os dados armazenados em becape até a data de 19 dias atrás.

78. (CESPE / ICMBIO - 2014) O  uso  do  becape  do  tipo  incremental  permite  que  sejam  copiados apenas os arquivos gravados desde o último becape normal ou incremental.

79. (CESPE / TJ-SE - 2014) Becapes podem ser realizados para atender a três propósitos distintos:
recuperação de desastres, recuperação operacional e arquivamento.

80. (VUNESP / Pref RP - 2018) A política de backup de uma empresa estabelece como requisito principal o menor tempo para a restauração. Para atender a esse requisito, deve-se selecionar, dentre os tipos conhecidos, o backup 
a) completo.
b) diferencial.
c) diferencial+incremental.
d) incremental.
e) progressivo.

81. (IDIB  / CRO  BA  –  2017) Acerca  da  realização  de  cópias  de  seguranças,  analise  as  seguintes afirmativas:

I.  Os  backups  dos  dados  armazenados  em  um  computador  são  importantes,  não  só  para recuperar  eventuais  falhas,  mas  também  evitar  consequências  de  uma  possível  infecção  por vírus, ou de uma invasão.

II. Um backup é a cópia de dados de um dispositivo de armazenamento a outro para que possam ser restaurados em caso da perda dos dados originais.

III. Atualmente são utilizados disquetes para backup de dados nas empresas.

Analisando as afirmativas acima, marque a alternativa verdadeira.

a) Apenas as afirmativas I e II estão corretas.
b) Apenas as afirmativas II e III estão corretas.
c) Apenas a afirmativa II está correta.
d) Apenas a afirmativa I está correta.

82. (IBFC  /  DIVIPREV  -  2018) Para  a  realização  de  cópias  de  segurança  (backup), um  típico armazenamento de dados magnético é o dispositivo:

Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







79
82



a)   DVD
b)   HD
c)   BluRay
d)   SSD

83. (IESES / Assistente Administrativo (CRO SC) - 2016) O tipo de backup que copia somente os arquivos alterados ou criados depois do último backup incremental é do tipo:

a) Diferencial.
b) Normal.
c) Cópia.
d) Diário.

84.(IESES / Técnico Judiciário (TRE MA) - 2015) Fazer uma cópia de segurança ou back-up ficou mais  fácil  hoje  em  dia.  É  possível  copiar  dados  em um  HD  externo,  pen-drive  ou  até  “nas nuvens”. Analise as afirmativas e assinale a INCORRETA:

a)  Três  estratégias  básicas  existem  para  realização  de  cópias:  incrementais,  completas  e diferenciais.

b) Cópias de segurança devem ser guardadas em local apropriado e atualizadas.

c)  Os  dados  contidos  em  discos  rígidos  podem  sofrer  danos  ou  ficar  inutilizados  por  vários motivos: choque do disco, vírus, defeito no hardware ou eliminação acidental.

d) Devido à segurança, muitas empresas preferem fazer suas cópias de segurança na nuvem ao invés de fazer localmente.

85. (IESES  /  Agente  Administrativo  (CRA  SC)  -  2013) Assinale  a  alternativa  que  diz  respeito  a seguinte definição:

“Este tipo de backup fornece um backup dos arquivos modificados desde que foi realizado um backup completo. Normalmente salva somente os arquivos que são diferentes ou novo desde o último backup completo, mas isso pode variar em diferentes programas de backup. Juntos, um backup completo e um backup desse tipo incluem todos os arquivos no computador, alterados e inalterados.”

a) Backup incremental.
b) Backup de referência.
c) Backup normal.
d) Backup diferencial.

86. (CETAP / Prefeitura de São Miguel do Guamá/PA - 2016) Em Tecnologia da Informação é denominado backup o processo de cópia e armazenagem de dados, de modo que estes dados Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







80
82



possam ser eventualmente recuperados em caso de perda. Leia as seguintes descrições de dois tipos de backup:

I - Copia apenas os arquivos que foram alterados ou criados desde o último backup completo, deste  modo  ocupando  maior  espaço  nas  mídias  de  armazenamento.  Contudo,  os  dados  são mais facilmente recuperados.

II  -  Faz  a  cópia  de  todos  os  arquivos  alterados  ou criados  desde  o  último  backup  (completo, diferencial ou incremental).

Assinale a alternativa correta que contém os tipos de backup de acordo com as descrições I e II, respectivamente:

a) I- Backup Completo, II- Backup Diferencial.
b) I- Backup Diferencial, II- Backup Incremental.
c) I- Backup Incremental, II- Backup Diferencial.
d) I- Backup Incremental, II- Backup Completo.

e) I- Backup Diferencial, II- Backup Completo.
























Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 







81
82



GABARITO
1. LETRA E
2. LETRA A
3. LETRA A
4. LETRA C
5. LETRA A
6. LETRA E
7. LETRA E
8. LETRA C
9. CORRETO
10. LETRA D
11. LETRA A
12. LETRA C
13. ERRADO
14. LETRA B
15. LETRA B
16. LETRA B
17. LETRA D
18. LETRA E
19. LETRA C
20. LETRA C
21. LETRA B
22. LETRA C
23. LETRA A
24. LETRA E
25. LETRA A
26. LETRA E
27. LETRA D
28. LETRA A
29. LETRA A
30. LETRA B
31. LETRA A
32. LETRA A
33. LETRA E
34. LETRA B
35. LETRA D
36. LETRA E
37. LETRA E
38. LETRA C
39. LETRA A
40. LETRA E
41. LETRA A
42. LETRA D
43. LETRA B
44. LETRA B
45. ERRADO
46. ERRADO
47. CORRETO
48.LETRA D
49. LETRA D
50. LETRA B
51. CORRETO
52. CORRETO
53. ERRADO
54. ERRADO
55. LETRA A
56. LETRA A
57. LETRA C
58. LETRA E
59. ERRADO
60. ERRADO
61. CORRETO
62. ERRADO
63. CORRETO
64. ERRADO
65. ERRADO
66. ERRADO
67. ERRADO
68. ERRADO
69. ERRADO
70. CORRETO
71. ERRADO
72. CORRETO
73. CORRETO
74. ERRADO
75. CORRETO
76. CORRETO
77. CORRETO
78. CORRETO
79. CORRETO
80. LETRA A
81. LETRA A
82. LETRA B
83. LETRA A
84.LETRA D
85. LETRA D
86. LETRA B
Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 








82
82





Diego Carvalho, Renato da Costa, Thiago Rodrigues Cavalcanti Aula 07
Informática p/ SEFAZ-CE (Auditor Fiscal) Com Videoaulas - 2020 www.estrategiaconcursos.com.br 1225432
06315057411 - EVA CELESTE DE SOUZA 