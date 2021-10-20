Negrito, itálico e sublinhado

Coloque qualquer texto em negrito, adicionando a tag:

<b>

no início do texto, e a tag de fechamento:

</b>

no início do texto, e a tag de fechamento:

</b>

onde você quiser que o atributo negrito termine.

Isto é <b>negrito</b>.

Isto é negrito.

Para deixar o texto em itálico, use as seguintes tags da mesma maneira:

<i>.....</i>

Isto é <i>itálico</i>.

Isto é itálico.

Para sublinhar, use as seguintes tags:

<u>.....</u>

Isto é <u>sublinhado</u>.

Isto é sublinhado.

Quebras de linha e parágrafos

Apesar de um texto digitado ter marcas de parágrafo, tabulações e espaços extras, os navegadores não os enxergam. Você terá que usar tags para criar espaços em branco nos seus documentos HTML.

<br> cria uma quebra de linha. Você pode usar várias destas tags juntas para criar espaço em branco.

Esta linha está <br> quebrada.

Esta linha está
quebrada.

<p> cria um espaço a mais entre duas linhas de texto. Se você colocar <br> em uma linha de texto, ela irá somente quebrar a linha; se você usar <p>, ela vai quebrar a linha e criar um espaço extra.

Esta linha está <p> com um espaço a mais.

Esta linha está

com um espaço a mais.

<hr>cria um separador, ou linha horizontal.

Este é um separador: <hr>

Este é um separador:

Tabulações

Não existe uma tag HTML especificamente para criar uma "tabulação" dentro de um documento. Muitos web designers criam tabelas ou usam imagens em branco para criar espaço (tabelas e imagens serão explicados mais adiante neste artigo). Uma maneira de recuar texto é usar a tag <ul> para fazer o navegador pensar que você vai criar uma "lista". A lista recua o texto automaticamente. Feche com </ul> para "encerrar" o recuo. As tags <blockquote>...</blockquote> também recuam texto.

Outra alternativa é a tag <pre>. Esta tag é usada para exibir texto pré-formatado - texto exibido "como ele é". Qualquer espaço criado dentro das tags <pre> e </pre> vai aparecer no navegador como aparece no código.


Alterando a cor, o tipo e o tamanho das fontes

Altere a cor de qualquer texto, usando as tags: onde você substitui "cor" pelo nome da cor desejada em inglês.

<font color="cor">...</font> 

Isto é <font color="#000099">vermelho</font>.

Isto é vermelho.

Isto é <font color="green">verde</font>.

Isto é verde.

A maioria das cores padrão vai funcionar. Experimente também os "lights" (claros) e "darks" (escuros) como em "lightblue" ou "darkgreen". Você também pode especificar um número de cor hexadecimal, como: <font color="#864086">. Uma lista de códigos de cores hexadecimais pode ser encontrado em December.com: HTML (em inglês).

Se você quiser especificar a cor para o texto inteiro da sua página, coloque o atributo text="cor" dentro da tag <body>.

Exemplo: <body text="blue">

Mesmo que você atribua uma cor para o texto inteiro, ainda assim pode mudar a cor de qualquer parte do texto usando as tags acima.

Altere o tipo de fonte de qualquer texto, usando as tags:

<font face="tipo de fonte"> ... </font>

Isto é <font face="arial">arial</font>.

Isto é Arial.

Isto é <font face="geneva">geneva</font>.

Isto é Geneva.

(Observação: Se o tipo de fonte que você especificar não estiver instalado no computador do usuário, o padrão do navegador será usado, geralmente Courier ou Times New Roman; então é melhor escolher os tipos de fonte padrão se você quiser controlar o que é exibido no navegador do usuário.)

Altere o tamanho da fonte de qualquer texto, usando as tags:

<font size=valor>...</font>

Exemplo: <font size=4>

O tamanho de fonte padrão na maioria dos navegadores é "3", então quaisquer valores acima de 3 vão deixar o texto maior, e quaisquer valores menores que 3 vão deixá-lo menor.

Você também pode mudar o tamanho de fonte ao somar ou subtrair números do tamanho padrão.

Exemplo: <font size=+4>, ou <font size=-2>

A esta fonte <font size=+2>somamos 2</font>.

A esta fonte somamos 2.

A esta fonte <font size=+1>somamos 1</font>.

A esta fonte somamos 1.

Desta fonte <font size=-2>subtraímos 2</font>.

Desta fonte subtraímos 2.

Desta fonte <font size=-1>subtraímos 1</font>.

Desta fonte subtraímos 1.

Você também pode mudar o tamanho de fonte, usando as tags <small> (pequeno) e <big> (grande):

Este texto é <small>pequeno</small>.

Este texto é pequeno.

Este texto é <big>grande</big>.

Este texto é grande.

Tags de título também mudam o tamanho de uma fonte, criando um "título" em negrito para um parágrafo ou texto:

<h1>Este é um título H1.</h1>

Este é um título H1.
<h2>Este é um título H2.</h2>

Este é um título H2.
<h3>Este é um título H3.</h3>

Este é um título H3.
Encerre qualquer mudança de fonte com a tag:

</font>

Ou com o fechamento das tags específicas que você usou:

Exemplo: </small>, </big>, </H2>

Criando cor de plano de fundo
Mude a cor do plano de fundo da sua página, colocando bgcolor="cor" dentro da tag <body>.

Exemplo: <body bgcolor="yellow">

Conforme falamos na seção sobre mudança de cor de fonte, você pode usar as cores padrão ou um Código de Fonte Hexadecimal (em inglês).

Criando listas
Há três tipos de lista que você pode criar: desordenada, ordenada e descritiva

Uma lista lista desordenada é assim:

São Paulo

Rio de Janeiro

Mato Grosso

Uma lista desordenada tem marcadores e começa com a tag <ul> (abreviação de unordered list). A tag <li> (abreviação de List Item, ou item da lista) é usada antes de cada item da lista. A tag de fechamento </ul> encerra a lista.

Exemplo:

<ul>
<li>São Paulo
<li>Rio de Janeiro
<li>Mato Grosso
</ul>

O tipo de marcador pode ser trocado por "circle" (círculo), "square" (quadrado) ou "disc" (disco), adicionando uma especificação dentro da tag <ul>

<ul type="circle">
<li>São Paulo
<li>Rio de Janeiro
<li>Mato Grosso
</ul>

São Paulo

Rio de Janeiro

Mato Grosso

<ul type="square">
<li>São Paulo
<li>Rio de Janeiro
<li>Mato Grosso
</ul>

São Paulo

Rio de Janeiro

Mato Grosso

Uma lista lista ordenada é assim:

laranjas

maçãs

bananas

Uma lista ordenada é uma lista de itens em uma ordem lógica numérica. Use as tags <ol> (abreviação de ordered list) e </ol> para começar e terminar este tipo de lista. A tag <li> também é usada na frente de cada item.

Exemplo:

<ol>
<li>laranjas
<li>maçãs
<li>bananas
</ol>

O tipo de organização pode ser alterado, adicionando uma designação de "tipo" dentro da tag <ol>.

<ol type="A"> ordena a lista com letras maiúsculas: (A, B, C...)

<ol type="a"> ordena a lista com letras minúsculas: (a, b, c...)

<ol type="I"> ordena a lista com números romanos: (I, II, III...)

<ol type="i"> ordena a lista com números romanos minúsculos: (i, ii, iii...)

Se você quiser começar sua lista com um valor específico, como "6", use as tags "start" (começar) e "value" (valor) a seguir:

<ol start=5>
<li value=6>

Uma lista descritiva cria uma lista de itens de texto com a segunda linha recuada:

Marshall Brain
Fundador da HowStuffWorks
Use as seguintes tags assim:

<dl>
<dt>Marshall Brain
<dd>Fundador da HowStuffWorks
</dl>

A tag <dt> (abreviação de descriptive list) corresponde ao texto que você quer que fique alinhado à margem e <dd> corresponde à linha que você quer que seja recuada.

Links para outros sites
Uma das melhores coisas das páginas de internet é a possibilidade de criar links para outras páginas na internet. Usando as tags âncora, você pode citar trabalhos de outras pessoas, apontar para outras páginas que você gosta, etc:

<a href="endereço">

Digite o título da página depois da tag âncora e feche com:

</a>

Exemplo:

<a href="http://www.hsw.com.br"> HowStuffWorks </a>

Vai ficar assim na sua página:

HowStuffWorks

Você também pode combinar listas com marcadores e links para criar uma lista de links.

Nova janela
Se você não quiser que os visitantes abandonem sua página quando clicarem em um link para outro site, adicione esta tag à sua tag âncora. Quando o visitante clica no link, ao invés de ele sair do seu site e entrar em outro, uma nova janela será aberta para mostrar o destino do link:

target="_blank"

Exemplo:
<a href="http://www.hsw.com.br" target="_blank">

Cor do link
Azul é a cor padrão para links. Mas você pode alterar as cores dos seus links, inserindo estas tags dentro da tag <body>:

link="cor"

vlink="cor"

Vlink são os "links visitados". Os links mudam de cor quando foram visitados. Se você não quiser que os links visitados mudem de cor, basta atribuir a mesma cor ao links e vlinks.

Exemplo: <body link="green" vlink="green">

Link para receber e-mail
Se você quiser receber e-mails das pessoas que visitarem seu site, use a tag âncora a seguir:

<a href="mailto:seu_endereco_de_email">

Digite novamente seu endereço de e-mail (ou o texto que você quiser para seu link) depois da tag. Feche a tag com:

</a>

Exemplo:

<a href="mailto:exemplo@howstuffworks.com"> Envie-me um e-mail </a>

Vai ficar assim na sua página:

Envie-me um e-mail

Criando links que levam para seu próprio site
As tags âncora não são usadas somente para criar links para outros sites na internet. Você também pode usá-las para exibir links que levam a informações localizadas dentro do seu próprio site. Neste caso, você pode omitir o prefixo "http://www" e incluir somente o nome do arquivo html:

Exemplo: <a href="empresa.htm"> Sobre a Empresa </a>

Para criar um link para uma parte específica da página, você precisará dar um nome às seção à qual está se referindo e colocar este nome dentro da tag âncora do link. Assim:

Dê um nome para qualquer seção do seu site, inserindo a tag a seguir imediatamente antes da seção específica à qual você quer que o link se refira. Você pode escolher qualquer palavra, letra ou caractere para usar como nome:

<a name="nome">

Exemplo: <a name="5">

Na tag âncora, você vai se referir a esta parte da página ao inserir um sinal de "#" na frente do nome. Se o link se referisse a um lugar dentro da página onde o link está, a tag âncora que liga à parte nomeada seria assim:

<a href="http://www.hsw.com.br/#5"> Sobre a Empresa </a>

Se o link se refere a um documento html que não a página onde o link está, inclua o nome do arquivo html também.

Exemplo: <a href="http://www.hsw.com.br/company.htm#5"> Sobre a Empresa </a>

Adicionando imagens e gráficos
Coloque qualquer imagem digital na sua página com a tag a seguir:

<img src="nome do arquivo de imagem.extensão">

As imagens na internet são ou arquivos GIF (pronuncia-se "guif") ou arquivos JPG (pronuncia-se "jota peg"). Qualquer imagem terá uma destas duas extensões, portanto se sua imagem chama "logo", será ou "logo.gif" ou "logo.jpg".

Não se esqueça de armazenar as imagens e gráficos que vão aparecer na sua página na mesma pasta onde está seu arquivo "html". Do contrário, seu computador não conseguirá encontrar a imagem que você quer exibir. Também não se esqueça de digitar o nome da imagem exatamente como ele está salvo na pasta - nomes de arquivo diferenciam maiúsculas e minúsculas.

Justificação
Por padrão, seu texto e suas imagens serão justificados à esquerda quando exibidos no navegador, o que significa que eles serão automaticamente alinhados à margem esquerda. Se você quiser "centralizar" qualquer parte da sua página, pode usar a tag a seguir:

<center>

Finalize a centralização com a tag de fechamento correspondente:

</center>

Você também pode criar códigos de "divisão"; uma palavra, uma linha de texto, ou uma página inteira podem ser justificados do jeito que você quiser.

Comece a divisão com a tag de divisão de alinhamento, incluindo a justificação que você quer para o texto ou imagem - ou seja, direita (right), esquerda (left), centro (center):

Exemplo: <div align="center">

Encerre a divisão de justificação de alinhamento com a tag:

</div>

Com o que acabou de aprender neste artigo, você pode começar a criar páginas de internet bem interessantes e atraentes. Tente criar uma página ou duas usando as ferramentas e tags que discutimos. Se você estiver ansioso para que o mundo veja sua obra de arte, então pule para o capítulo "Colocando sua página no ar" para aprender a publicar sua nova página.

Criando tabelas
A grande lista

Confira a Grande Lista de Tags HTML

É um guia de referência em uma única página para impressão com todas as tags de HTML apresentadas neste artigo - de fácil acesso e em formato PDF para impressão mais fácil!

Atualmente, uma das ferramentas HTML mais usadas para criar páginas com visual mais organizado é a tabela. Quando você fica craque em tabelas, não apenas "cria" uma página, mas "desenha" uma.

A variedade de tabelas disponíveis é grande, e varia desde uma caixa simples até layouts bem complexos. Falaremos aqui sobre o básico das tabelas e também sobre alguns truques e dicas para você experimentar, para que você desenhe uma página legal e que as pessoas gostem de visitar.

Assim como toda informação que você quiser exibir na janela do navegador, a tabela também deve estar entre as tags <body> e </body> do seu documento HTML. Comece a tabela com a tag a seguir:

<table>

Cada linha horizontal em uma tabela começa com a tag:

<tr>

E cada conjunto de dados dentro da linha começa com a tag:

<td>

Pense na seguinte tabela:

A1

A2

B1

B2

C1

C2

Aqui temos três linhas e duas colunas.

Para criar o esqueleto desta tabela, as tags a seguir são usadas nesta ordem:

<table>

inicia a tabela

<tr>

inicia a primeira linha

<td>

inicia a primeira "célula" de dados (A1)

</td>

fecha a célula A1

<td>

inicia a segunda célula (A2)

</td>

fecha a célula A2

</tr>

fecha a primeira linha

<tr>

inicia a segunda linha

<td>

inicia a primeira célula de dados da segunda linha (B1)

</td>

fecha a célula B1

<td>

inicia a célula B2

</td>

fecha a célula B2

</tr>

fecha a segunda linha

<tr>

inicia a terceira linha

<td>

inicia a primeira célula de dados da terceira linha (C1)

</td>

fecha a célula C1

<td>

inicia a célula C2

</td>

fecha a célula C2

</tr>

fecha a terceira linha

</table>

fecha a tabela

Muitos designers gostam de recuar o texto do código para facilitar a leitura. Um exemplo de recuo é mostrado mais adiante.

Agora vamos adicionar dados e uma borda ao esqueleto da tabela. A borda é o contorno da tabela. A tag de borda (border="value") é colocada dentro da tag inicial da tabela. Você pode especificar a espessura do contorno, determinando um valor (vamos estabelecer o valor "1"). Uma boa idéia é experimentar valores diferentes para descobrir como eles ficam quando são exibidos no navegador. Se você não quiser bordas, coloque o valor "0".

(Observação: Mesmo que você não queira uma borda em volta da sua tabela, é sempre bom começar com uma borda visível, pelo menos até você resolver os "bugs" que podem afetar a forma como sua tabela é exibida.)

Digite (ou copie e cole) o código e os dados a seguir no seu documento HTML:

         
A1

A2

B1

B2

C1

C2

  
A tabela exibida no seu navegador deve ficar bem parecida com o diagrama do começo desta seção.

Há muitos atributos que você pode usar na tabela. A seguir discutiremos algumas tags para você formatar sua tabela de um jeito bem criativo.

Cor de fundo
Mude a cor de fundo (background color) da tabela toda com a tag "bgcolor" dentro da tag "table" inicial:

Exemplo: <table bgcolor="yellow">

Uma cor de fundo também pode ser atribuída a uma linha ou a uma célula dentro da tabela. Basta adicionar bgcolor="cor" à tag <tr> ou <td> para colorir aquela parte específica da tabela.

Exemplo: <tr bgcolor="yellow">

Tamanho da tabela
A largura (width) e altura (height) das linhas e colunas em uma tabela vão expandir automaticamente para acomodar a quantidade de dados e/ou o espaço da janela do navegador. Para especificar a largura e altura, coloque valores em pixels ou porcentagem dentro da tag "table" inicial:

Exemplo: <table width=300 height=400>

Largura e altura podem também ser especificadas para uma célula individual, em relação à tabela como um todo. Adicione width="valor" à tag <tr> ou <td> em questão.

É bom experimentar valores em pixels e em porcentagens para descobrir como eles ficam quando são exibidos no browser.

Preenchimento de célula (cellpadding)
A tag "cellpadding" especifica (em pixels) o espaço entre a borda de cada célula e os dados dentro de cada célula. Use este atributo dentro da tag "table":

Exemplo 1: <table border=1 cellpadding=5>

Esta tabela tem

cellpadding "5".

Exemplo 2: <table border=1 cellpadding=15>

Esta tabela tem

cellpadding "15".

Espaçamento de célula (cellspacing)
A tag "cellspacing" especifica (em pixels) o espaço entre uma célula e outra. Use este atributo dentro da tag "table":

Exemplo 1: <table border=1 cellspacing=5>

Esta tabela tem

cellspacing "5".

Exemplo 2: <table border=1 cellspacing=15>

Esta tabela tem

cellspacing "15".

Cabeçalhos de tabela
Para criar um "cabeçalho" em negrito e centralizado para uma coluna ou linha dentro da tabela, use a tag <th> no lugar da tag <td> no código para a primeira linha.

Exemplo:

         
Column 1

Column 2

A

B

C

D

  
Fica assim:

Coluna 1

Coluna 2

A

B

C

D

Alinhamento
Por padrão, todos os conteúdos das células dentro de uma tabela (com exceção dos cabeçalhos) são centralizados verticalmente e justificados à esquerda. Para mudar o alinhamento do conteúdo de uma célula, coloque as tags a seguir dentro das tags <td>, <th> ou <tr>:

No alinhamento horizontal, os valores podem ser "left" (esquerda), "right" (direita) ou "center" (centro):

Exemplo: <tr align="center">

Para alinhamento vertical, os valores podem ser "top" (topo), "bottom" (base) ou "middle" (meio):

Exemplo: <td valign="top">

Você pode também definir um alinhamento para a tabela inteira, estabelecendo o lugar onde ela aparece na página. Ao inserir as tags <align="right"> ou <align="left"> dentro da tag "table" inicial, o texto vai ficar em volta da tabela onde quer que ela esteja localizada. Ou, se você quiser que a tabela fique sozinha e sem texto à sua volta, use tags "division alignment" (divisão de alinhamento) antes e depois da tabela inteira.

Extensão de célula (cellspanning)
O "spanning" acontece quando uma célula ocupa o lugar de duas ou mais células na tabela. Um exemplo de spanning de coluna:

Esta célula ocupa a largura de duas colunas

Esta célula ocupa a largura de uma coluna

A

B

C

A tag <colspan=value> é colocada dentro da tag <td> onde ela se aplica. O código que foi escrito para o exemplo acima é:

         
Esta célula ocupa a largura de duas colunas

esta célula ocupa a largura de uma coluna

A

B

C

  
Um exemplo de spanning de linha:

Esta célula ocupa a altura de duas linhas

A

B

C

D

A tag <rowspan=value> é colocada dentro da tag <td> de onde ela se aplica. O código que foi escrito para o exemplo acima é:

         
Esta célula ocupa a altura de duas linhas

A

B

C

D

  
Você também pode aplicar na sua tabela muitos outros atributos que aprendeu no último capítulo, como tamanho, tipo e cor de fonte, inserir uma imagem, fazer uma lista e adicionar um link. Basta adicionar a tag apropriada na célula que você quer formatar, logo após a tag <td> dessa célula.

Experimente e pratique as várias ferramentas e tags que aprendeu neste artigo. As possibilidades são infinitas quando se trata de usar tabelas em uma página de Internet. Agrupe imagens e caixas coloridas sem borda para criar designs limpos, ou coloque tabelas sem borda dentro de tabelas sem borda, algumas com cor, outras sem, para criar layouts atraentes. Os limites de design de uma página de Internet se expandem com um pouco de imaginação, criatividade e um bom uso de tabelas.

Criando frames
Alguns web designers usam frames (molduras) em suas páginas, por uma questão de design e para fazer o site ficar mais amigável para o usuário. Frames não deixam você perder a referência durante a navegação, digamos assim. Você sabe que um site foi feito com base em frames quando uma parte da página fica parada e outra parte da mesma página muda quando você clica em um link. Para ver uma página com frames, visite The Birch Aquarium (em inglês).

A grande lista

Confira a Grande lista de tags de HTML. É um guia de referência em uma única página para impressão com todas as tags de HTML apresentadas neste artigo - de fácil acesso e em formato PDF para impressão mais fácil!

Na página do The Birch Aquarium, o topo e a base da página permanecem os mesmos, enquanto a parte do meio muda de acordo com o link escolhido. Esta página é separada em três frames, o que significa que três documentos HTML estão sendo exibidos ao mesmo tempo. Você pode escolher em quantas seções vai dividir sua página, de que maneira elas serão divididas e quais documentos HTML você quer colocar em cada frame.

Primeiro, é importante planejar bem sua página. Pense no layout em termos de linhas e colunas. Quantas seções horizontais, ou linhas, você quer exibir? Quantas seções verticais, ou colunas? De quanto espaço, em pixels ou porcentagem, você acha que cada seção vai precisar?

O documento frameset
O documento frameset é um HTML que instrui o navegador sobre como arrumar o conteúdo na página. No documento frameset, a tag "frameset" substitui a tag "body".

Você vai iniciar seu documento frameset no formato HTML normal:

<html><head><title>Título</title></head>

Em seguida, insira a tag "frameset":

Exemplo: <frameset rows="20%, 80%">

Esta tag indica que a página será dividida em duas seções, uma no topo e uma na base, conforme os dois valores indicados dentro da tag. Se fossem três seções, você colocaria três valores:

Exemplo: <frameset rows="10%, 50%, 40%">

Os números dizem ao navegador a quantidade de espaço, na janela do browser, que cada seção vai ocupar. Você pode usar valores percentuais ou em pixels. Um "*" também pode ser usado no lugar de um valor, indicando que uma seção em particular pode usar o espaço que estiver disponível na janela do navegador:

Exemplo: <frameset rows="100, *, 50">

Esta tag diz que a página será dividida em três seções. O primeiro frame (topo) ocupará 100 pixels de espaço, o frame da base ocupará 50 pixels, e o frame do meio vai ocupar o espaço que sobrar na janela do navegador.

Se sua página será dividida em colunas, use a tag frameset para colunas, junto com os números:

Exemplo: <frameset cols="200, *">

Esta tag diz ao browser para ele dividir a página em duas colunas. A coluna da esquerda vai ocupar 200 pixels de espaço. A coluna da direita vai ocupar o espaço que sobrar na janela do navegador.

Você também pode combinar framesets de linhas e colunas para criar layouts mais complexos. O "encadeamento" dos documentos frameset será discutido mais adiante neste artigo.

Adicionando a origem do frame
Se você ainda não criou os documentos HTML que vão ocupar cada frame na sua página, crie agora. Você pode usar os documentos HTML que criou nos capítulos anteriores.

Agora você vai adicionar ao seu documento frameset as tags "frame src", que dirão ao browser quais documentos HTML ele deve colocar em cada frame:

Exemplo:

                   
Este exemplo mostra um documento frameset que vai dividir a página em duas colunas, ou frames. No frame da esquerda, 200 pixels de espaço vão exibir o documento "links.htm". O resto da página, a coluna da direita, vai exibir o documento "information.htm". Você também viu ali as tags usadas para fechar um documento frameset:

</frameset>
</html>

Dando nomes aos frames
Geralmente, uma página tem frames para mostrar ou oferecer links para informações adicionais localizadas dentro do mesmo site. O site The Birch Aquarium é um exemplo de frames usados para exibir links para informações dentro do mesmo site. A barra do menu de links puxa informações para o frame do meio da página quando um link é clicado, sem atrapalhar os frames externos da página.

Para que o navegador saiba em qual frame colocar a informação linkada, você precisa dar "nomes" para os seus frames. Se você não especificar qual frame vai receber determinada informação, o frame do menu de links será substituído pela própria informação dos links, destruindo o visual e o propósito da sua página feita em frames.

Para dar nome a um frame, basta colocar a tag "name" (nome) dentro da tag "frame src" (origem do frame) no seu documento frameset. Você pode dar o nome que quiser para cada frame.

Exemplo:

<frame src="links.htm" name="menu">
<frame src="information.htm" name="info">

Depois de nomear o frame, você pode especificar em qual frame você quer que a informação do link seja colocada; para isto, adicione a tag "target" (destino), seguida do nome do frame.

Exemplo: <a href="http://www.hsw.com.br/company.htm" target="info"> Sobre a Empresa </a>

O browser agora sabe que precisa exibir a informação do link no frame chamado "info".

Salvando e visualizando seu documento
Como os documentos HTML comuns, os documentos frameset são salvos com extensões .htm ou .html. Não esqueça de colocar o arquivo frameset na mesma pasta dos documentos HTML que vão aparecer nos frames.

Quando você abre o documento frameset no navegador, tem que enxergar a tela dividida, com um documento HTML dentro de cada frame.

Removendo barras de rolagem e bordas
Se você prefere dar um visual "clean" para a sua página, sem barras de rolagem e bordas, você pode especificar em tags dentro da tag "frame src".

Remova as barras de rolagem com a tag "scrolling=no".

Exemplo: <frame src="links.htm" scrolling=no>

Remova as bordas com a tag "frameborder=0".

Exemplo: <frame src="links.htm" frameborder=0>

Você também pode especificar a largura e altura da margem de cada frame, adicionando as tags "marginwidth=valor" e "marginheight=valor". As margens podem ter quantos pixels você quiser. Estas tags devem ser inseridas dentro da tag "frame src".

Frames múltiplos
Pode-se combinar várias linhas e colunas de frames, criando documentos frameset dentro de outros documentos frameset. O conjunto de tags necessárias para criar este efeito pode ser bem complexo. Exemplo de uma página com frames "encadeados":



O documento frameset criado para este layout é:

                                              
                                              
Separado por partes, o que cada linha de tags "frame" indica é:

<frameset rows="20%, 80%">
Há duas linhas dentro deste documento. A linha de cima ocupa 20% do espaço vertical disponível. A de baixo, os outros 80%. De fato, estes valores especificam a altura de cada linha.

<frameset cols="70%, 30%">
Há colunas dentro da primeira linha. A coluna da esquerda ocupa 70% do espaço horizontal disponível e a coluna da direita, os 30% remanescentes. De fato, estes valores especificam a largura de cada coluna.

<frame src="logo.htm">
O documento HTM "logo" vai aparecer na primeira coluna da primeira linha.

<frame src="endereco.htm">
O documento HTM "endereco" vai aparecer na segunda coluna da primeira linha.

</frameset>
O frameset da primeira coluna está completo.

<frameset cols="85%, 15%>
Há duas colunas dentro da segunda linha. A coluna da esquerda ocupa 85% do espaço horizontal disponível. A da direita, os outros 15%.

<frame src="info.htm">
O documento HTM "info" vai aparecer na primeira coluna da segunda linha.

<frame src="links.htm">
O documento HTM "links" vai aparecer na segunda coluna da segunda linha.

</frameset>
O frameset da segunda coluna está completo.

</frameset>
O frameset inteiro está completo.

Frames são uma boa ferramenta para tornar a página mais atraente e dinâmica. Eles permitem que determinados aspectos da página permaneçam inalterados mesmo quando o usuário clica em um link para outra parte do site, ou para outro site totalmente diferente. Para continuar construindo a página dos seus sonhos, confira a próxima seção sobre imagens.

Figuras
Quando você começa a criar sua página, uma das primeiras coisas que vai querer adicionar são imagens. Os seres humanos valorizam o visual e as imagens podem mudar totalmente a cara do site.

Você pode usar imagens pequenas:



Imagens longas e finas:



Imagens maiores:

HowStuffWorks

Ou até mesmo animações:



Você pode usar pequenas imagens como marcadores customizados, como estes:

Primeira linha

Segunda linha

Terceira linha

Transforme um gráfico em marcador, adicionando a tag da imagem onde você quer que o marcador apareça; não é necessário usar a tag <ul>.

A grande lista

Confira a Grande lista de tags de HTML(em inglês). É um guia de referência em uma única página para impressão com todas as tags de HTML apresentadas neste artigo - de fácil acesso e em formato PDF para impressão mais fácil!

Imagens longas e finas podem ser usadas como separadores. Imagens maiores podem ser usadas como logos ou ilustrações - praticamente qualquer coisa que você imaginar.

Há duas maneiras de obter imagens gráficas: você pode baixá-las de vários sites de "clip art grátis" na Internet, ou pode criá-las você mesmo. Alguns sites que oferecem gráficos e animações gratuitos são Page Works, A-1 All Free Clip Art, e The Free Graphics Store (em inglês). Você também pode visitar The Free Site, Web Places e Free Graphics (em inglês) para acessar diretórios de sites de imagens gratuitas.

Digamos que você vá a um site de gráficos grátis e goste de uma imagem. Se você clicar com o botão direito na imagem, um menu vai abrir e uma das opções será "Salvar imagem como...". Salve a imagem na pasta onde sua página está guardada.

Se você quiser criar suas próprias imagens, vai precisar de um programa que edite arquivos GIF e JPG. Um muito programa de edição de imagens muito popular disponível na Internet é o Paint Shop Pro. Você pode baixar uma cópia aqui (em inglês). Com um pouco de prática e um mínimo de habilidade artística, logo você estará criando imagens como um profissional!

Como descrevemos nas "Tags básicas de formatação HTML", as imagens são inseridas em uma página com a tag:

<img src="nome do arquivo">

Você também pode usar uma imagem como link para outra página ou elemento. Para isto, basta inserir a tag "img src" depois da tag âncora. Não se esqueça de incluir "border=0" ou a sua imagem vai ganhar uma borda feia.

Exemplo: <a href=http://www.hsw.com.br><img src="hswlogo.jpg" border=0></a>

Neste exemplo, se o usuário clicar na imagem "hswlogo.jpg", será levado à homepage da HowStuffWorks em http://www.hsw.com.br.

Qualquer imagem digital também pode ser usada como plano de fundo (background) para sua página. Basta adicionar background="nome do arquivo de imagem" dentro da tag <body>.

Exemplo: <body background="hsw-logo.jpg">

Etiquetas
Outra tag útil, mas não obrigatória, que você pode adicionar à sua imagem é "alt". Esta tag dá uma etiqueta para sua imagem, e aparece quando o usuário passa o mouse sobre ela. Também aparece antes da imagem quando sua página está carregando no navegador, prendendo a atenção do usuário enquanto a imagem carrega. Você pode escrever a mensagem que quiser usando a tag "alt".

Exemplo: <img src="hswlogo.jpg" alt="Informações Corporativas da HSW">

Alinhamento de figura
O alinhamento horizontal das imagens na sua página é formatado usando as tags e técnicas explicadas na seção sobre justificação. Uma rápida revisão:

Use a tag <div align=.".."> antes da tag de imagem para centralizar ou justificar à direita ou à esquerda.

Use a tag </div> depois da tag de imagem para encerrar a justificação.

Use a tag <align=.".."> dentro da tag "img src" para fazer o texto ficar em volta da imagem.

Insira estas tags dentro da tag "img src" para fazer o alinhamento vertical das imagens em relação ao texto:

align="bottom"
O texto fica alinhado à base da figura.

HowStuffWorks TEXTO

<img src="http://static.hsw.com.br/gif/hsw-logo3.gif" alt="HowStuffWorks" border=0 align="bottom">


align="top"
O texto fica alinhado ao topo da figura.

HowStuffWorks TEXTO

<img src="http://static.hsw.com.br/gif/hsw-logo3.gif" alt="HowStuffWorks" border=0 align="top">


align="middle"
O texto fica alinhado ao meio da figura.

HowStuffWorks TEXTO

<img src="http://static.hsw.com.br/gif/hsw-logo3.gif" alt="HowStuffWorks" border=0 align="middle">


Em cada um dos exemplos acima, a imagem está justificada à esquerda por padrão, então o texto aparece à direita. Se você quiser o texto à esquerda e a imagem à direita, você pode adicionar a tag de alinhamento de figura <div align> discutida acima.

Se as suas imagens não funcionarem...

Recebemos muitos e-mails de pessoas com problemas para adicionar imagens às páginas. Quando GIFs e JPGs dão erro, aparecem como um pequeno X vermelho, assim:



Quando você encontra este problema na página, significa que você não digitou o nome correto do arquivo da imagem. Os passos para corrigir o problema são:

Comece por simplificar o processo. Coloque o arquivo HTML e o arquivo da imagem na mesma pasta. Renomeie o arquivo da imagem para xyz.gif (ou xyz.jpg). Crie uma tag assim <img src="xyz.gif"> na sua página HTML. Visualize a página no navegador. Se você ainda vir o X vermelho ao invés da imagem, então...

Confira se o arquivo renomeado está mesmo com o nome xyz.gif. Em uma máquina com UNIX, letras maiúsculas e minúsculas fazem diferença, então confira se o que deveria ser maiúsculo está maiúsculo, e o que deveria ser minúsculo está minúsculo. O nome Xyz.gif é totalmente diferente de xyz.gif para o UNIX.

Em uma máquina rodando Windows, o sistema operacional às vezes adiciona sufixos ao nome do arquivo sem avisar você. Por exemplo, você pode ver xyz.gif no Explorer, mas o Windows pode ter renomeado o arquivo para xyz.gif.gif. O jeito mais fácil de ver se isto aconteceu é usar o comando dir no prompt do MS-DOS, pois ali você vê os nomes reais dos arquivos. Se o Windows estiver de fato adicionando sufixos, você pode desabilitar esta função na caixa de diálogo de Opções do Explorer.



Quando você encontra este problema na página, significa que você não digitou o nome correto do arquivo da imagem. Os passos para corrigir o problema são:

Comece por simplificar o processo. Coloque o arquivo HTML e o arquivo da imagem na mesma pasta. Renomeie o arquivo da imagem para xyz.gif (ou xyz.jpg). Crie uma tag assim <img src="xyz.gif"> na sua página HTML. Visualize a página no navegador. Se você ainda vir o X vermelho ao invés da imagem, então...

Confira se o arquivo renomeado está mesmo com o nome xyz.gif. Em uma máquina com UNIX, letras maiúsculas e minúsculas fazem diferença, então confira se o que deveria ser maiúsculo está maiúsculo, e o que deveria ser minúsculo está minúsculo. O nome Xyz.gif é totalmente diferente de xyz.gif para o UNIX.

Em uma máquina rodando Windows, o sistema operacional às vezes adiciona sufixos ao nome do arquivo sem avisar você. Por exemplo, você pode ver xyz.gif no Explorer, mas o Windows pode ter renomeado o arquivo para xyz.gif.gif. O jeito mais fácil de ver se isto aconteceu é usar o comando dir no prompt do MS-DOS, pois ali você vê os nomes reais dos arquivos. Se o Windows estiver de fato adicionando sufixos, você pode desabilitar esta função na caixa de diálogo de Opções do Explorer.



Quando você encontra este problema na página, significa que você não digitou o nome correto do arquivo da imagem. Os passos para corrigir o problema são:

Comece por simplificar o processo. Coloque o arquivo HTML e o arquivo da imagem na mesma pasta. Renomeie o arquivo da imagem para xyz.gif (ou xyz.jpg). Crie uma tag assim <img src="xyz.gif"> na sua página HTML. Visualize a página no navegador. Se você ainda vir o X vermelho ao invés da imagem, então...

Confira se o arquivo renomeado está mesmo com o nome xyz.gif. Em uma máquina com UNIX, letras maiúsculas e minúsculas fazem diferença, então confira se o que deveria ser maiúsculo está maiúsculo, e o que deveria ser minúsculo está minúsculo. O nome Xyz.gif é totalmente diferente de xyz.gif para o UNIX.

Em uma máquina rodando Windows, o sistema operacional às vezes adiciona sufixos ao nome do arquivo sem avisar você. Por exemplo, você pode ver xyz.gif no Explorer, mas o Windows pode ter renomeado o arquivo para xyz.gif.gif. O jeito mais fácil de ver se isto aconteceu é usar o comando dir no prompt do MS-DOS, pois ali você vê os nomes reais dos arquivos. Se o Windows estiver de fato adicionando sufixos, você pode desabilitar esta função na caixa de diálogo de Opções do Explorer.



Criando GIFs animados
GIFS animados dão movimento e brilho à sua página. Uma boa ferramenta para criar GIFs animados é The GIF Construction Set (em inglês). Com esta ferramenta, ou outra parecida, você pode criar quadros diferentes em uma seqüência animada e colocar todos eles em uma única imagem. Um exemplo de cinco quadros e um GIF animado criado a partir deles:











O GIF animado final:







Colocando sua página no ar
Depois de criar uma página, você vai querer colocá-la em um servidor para todo mundo ver. Muitas empresas e instituições oferecem espaço gratuito para publicar suas páginas. A AOL oferece espaço gratuito para seus assinantes e muitas faculdades oferecem espaço a seus alunos. Há também muitos sites comerciais que oferecem espaço gratuito. A única desvantagem destas opções é que você vai provavelmente ter que exibir o banner de anúncio do site no topo da sua página ou dentro dela. Algumas destas fontes comerciais gratuitas são:

Geocities

Tripod

Homestead

Você também tem a opção de pagar um serviço de hospedagem para ter espaço na Internet. A maioria dos sites profissionais segue por este caminho. Serviços de hospedagem podem fornecer a seus clientes grandes quantidades de espaço, opções especiais e confiabilidade. Usar um serviço de hospedagem também permite que você use um nome de domínio, um endereço só seu.

A grande lista

Confira esta excelente ferramenta de referência HTML:

Grande lista de tags de HTML

É um guia de referência em uma única página, para impressão, com todas as tags de HTML apresentadas neste artigo - de fácil acesso e em formato PDF para impressão mais fácil!

Se você está interessado em ter seu próprio domínio, visite a página das Registros.br (em inglês) ou (http://www.registro.br). Você pode checar a disponibilidade dos domínios e comprar um que você goste. O custo de um contrato de um ano é geralmente menor se você tiver um serviço de hospedagem, então quando você for comprar um domínio, entre em contato com um serviço de hospedagem antes. A maioria dos serviços de hospedagem registra o domínio para você e fornece soluções de rede com números de IP e outras informações necessárias para o registro.

Existe uma grande variedade de serviços de hospedagem disponíveis em várias faixas de preço. Não esqueça, porém, que quando a esmola é demais o santo desconfia. Você pode dar de cara com servidores lentos, serviço que cai, falta de suporte, frustração e decepção.

Boas ferramentas
Depois de colocar sua página em um servidor, vai querer saber como anda o tráfego do seu site. Sites como Show Stat, Hit Box, ou Site Meter (em inglês) oferecem este serviço de graça e fornecem estatísticas bem completas. Se você quiser ter apenas um contador simples na página, o FastCounter (em inglês) é uma boa ferramenta.

Há várias ferramentas que você pode usar para melhorar seu site. Por exemplo, esta ferramenta gratuita (em inglês) vai checar se seu site tem erros de ortografia, o tempo que a página leva para carregar, as meta tags, a compatibilidade com o navegador, etc.

Meta tags
Se você está pensando em colocar suas páginas em ferramentas de busca (em inglês) - assunto do próximo capítulo -  você vai precisar adicionar Metatags à sua página. As duas Metatags mais comuns deixam você descrever a página e especificar um conjunto de palavras-chave para ela, além de declarar várias outras coisas. As Metatags sempre aparecem entre as tags <HEAD> e </HEAD> do código-fonte HTML. As Metatags que aparecem no topo da página principal da HowStuffWorks são:

<Meta Name="Description" Content="O índice para mais de 50 artigos fantásticos da 'HowStuffWorks' articles!">

<Meta Name="keywords" Content="como as coisas funcionam, o jeito que as coisas funcionam,informação, tutoriais, explicação, explica, entendimento, diga-me, alunos, professores, estudar, educativo">

<Meta http-equiv="PICS-Label" content='(PICS-1.1 "http://www.rsac.org/ratingsv01.html" l gen true comment "RSACi North America Server" for "http://www.hsw.com.br" on "1998.09.23T01:29-0800" r (n 0 s 0 v 0 l 0))'>

<Meta Name="keywords" Content="como as coisas funcionam, o jeito que as coisas funcionam,informação, tutoriais, explicação, explica, entendimento, diga-me, alunos, professores, estudar, educativo">

<Meta http-equiv="PICS-Label" content='(PICS-1.1 "http://www.rsac.org/ratingsv01.html" l gen true comment "RSACi North America Server" for "http://www.hsw.com.br" on "1998.09.23T01:29-0800" r (n 0 s 0 v 0 l 0))'>

A primeira tag é uma descrição da página. As ferramentas de busca usam este texto diretamente em suas listagens. Se você não tiver uma meta tag de descrição, de duas, uma: ou a ferramenta de busca deixa sua descrição em branco ou usa uma ou duas frases do início da sua página como descrição.

A segunda tag indica um conjunto de palavras-chave extras para a página. As ferramentas de busca geralmente indexam cada palavra na página, mas em muitos casos você não vai usar no texto da sua página uma determinada palavra que pode ser usada por alguém à procura da sua página. Se você sabe que as pessoas geralmente escrevem errado uma determinada palavra, você pode também colocá-la na lista de palavras-chave.

A terceira tag é uma tag de classificação da RSAC. Veja abaixo uma descrição do que o sistema de classificação RSAC faz, tirada do site da RSAC em www.rsac.org (em inglês): 

"O Conselho Consultivo de Software Recreativo é uma organização independente, sem fins lucrativos, localizada em Washington, D.C, que dá ao público, principalmente aos pais, o poder de tomar decisões conscientes sobre a mídia eletrônica, através de um sistema consultivo aberto e objetivo para conteúdos. O sistema RSACi fornece aos consumidores informações sobre os níveis de sexo, nudez, violência, linguagem ofensiva (vulgar ou motivada por ódio) em jogos de computador e sites da Internet. Até hoje, o RSACi já foi integrado ao navegador da Microsoft, Internet Explorer; e ao programa Cyber Patrol, da MicroSystems. A CompuServe (nos Estados Unidos e na Europa) também já se comprometeu a classificar todo seu conteúdo com o sistema RSACi".
Alguns navegadores são configurados para bloquear páginas que não estejam classificadas, então, ao classificar seu site você evita problemas com estes navegadores. Ao classificar seu conteúdo pela RSAC, você mostra para as pessoas exatamente que tipo de conteúdo está fornecendo. Quando você classificar sua página, pode usar este selo:



Há várias outras tags que você vai encontrar nos códigos-fonte HTML de outras páginas na Internet. Muitas ferramentas HTML adicionam tags automaticamente. Por exemplo, estas são duas tags que o Microsoft Word automaticamente aplica a uma página se você usá-lo para criar um HTML:

<META HTTP-EQUIV="Content-Type" CONTENT="text/html; charset=windows-1252">

<META NAME="Generator" CONTENT="Microsoft Word 97">

<META NAME="Generator" CONTENT="Microsoft Word 97">

Em todos os casos, as meta tags não afetam a forma como sua página aparece no navegador. A descrição e as palavras-chave são as mais comuns.

Promovendo seu site
Depois que você passou horas criando seu site e o colocou em um servidor, você vai querer que todos o vejam. Mas para fazer as pessoas visitarem seu site, você precisa promovê-lo. Muito poucas pessoas vão encontrar seu site por acidente - alguma coisa tem que levá-las até lá.

Há muitas técnicas diferentes que podem ser usadas para atrair as pessoas até seu site. Este capítulo vai ensinar como aumentar o tráfego do seu site.

Cadastro em ferramentas de busca
Ferramentas de busca (em inglês) lêem as páginas da Internet e indexam todas as palavras da página. Usuários das ferramentas de busca podem encontrar sua página através de palavras-chave. O bom das ferramentas de busca é que elas trazem para você tudo o que tiver determinada palavra ou conjunto de palavras. A parte ruim é que as ferramentas de busca também trazem muita coisa que não tem nada a ver com o que você está procurando.

Do ponto de vista de promoção na Internet, uma coisa boa das ferramentas de busca é que é fácil cadastrar seu site nelas. Cada uma delas tem em algum lugar da página um link chamado "cadastre um site", ou algo parecido. Por este link, você poderá preencher um formulário (alguns mais extensos que outros) pedindo para cadastrar seu site. Seu site não será adicionado imediatamente, e às vezes será necessário fazer o cadastro várias vezes antes de seu site ser listado. Uma ferramenta de busca é diferente da outra. Além disso, cadastre cada uma das suas páginas individualmente para ter certeza de que as palavras-chave de cada página foram incluídas.

Abaixo, uma lista dos endereços das páginas de cadastro de sites de algumas das ferramentas de busca mais importantes:

Alta Vista

AOL Search (em inglês)

Google (em inglês)

HotBot (em inglês)

Lycos (em inglês)

WebCrawler (em inglês)

Cadastro em sites de links
Um site de links lista vários sites em algum tipo de estrutura hierárquica. Cada site é colocado em uma categoria e recebe uma pequena descrição. O Yahoo é o melhor exemplo deste tipo de site, mas há muitos outros que fazem a mesma coisa de maneiras diferentes.

A maioria destes sites é muito lenta na inclusão de novos sites porque alguém precisa analisar cada site cadastrado antes de ele ser adicionado à lista de links. Os links a seguir apontam para alguns destes sites, pois você precisa conhecê-los para descobrir qual categoria se refere ao seu site antes de adicionar um endereço. Assim que você encontrar a categoria apropriada, procure o botão "Adicionar endereço" para adicionar seu site. (Sites abaixo em inglês).

Jayde Online Directory

LookSmart

Nerd World

Northern Light

Open Directory

Yahoo!

Serviços de listagem de empresas
Se o seu site é relacionado a negócios, você deve cadastrá-lo em todos os sites a seguir. Estes sites vão listar sua empresa em seus diretórios (alguns não cobram nada, outros cobram).   (Sites abaixo em inglês)

AllSearchEngines

b2bFreeNet

SuperPages

Biz Land

Business Search Engines

EZDirectory

SmallBiz

Cadastro em sites de reconhecimento
Sites de reconhecimento apresentam seu site para o mundo (geralmente por uma hora ou um dia, como um site único, ou "legal") ou dão algum tipo de prêmio, que você pode exibir na forma de uma logo estampada em seu site. Em todos eles, é necessário fazer um cadastro para ser reconhecido. Os sites a seguir são alguns dos sites de reconhecimento mais populares (em inglês):

Cool Site of the Day

Seven Wonders of the Web

Web 100

Webby Awards

Wow! Web Wonders

Serviços de cadastro
As empresas listadas abaixo vão cadastrar seu site em centenas de ferramentas de busca (algumas delas cobram por isso). A maioria delas também oferece outros serviços de promoção na Internet. Muitos oferecem informação sobre como você mesmo pode promover seu site: basta visitá-los para buscar algumas idéias.

É importante salientar que estes serviços de cadastro em ferramentas de busca não fazem nada que você não possa fazer sozinho. Você pode cadastrar seu site tão bem quanto eles, e tudo o que você precisa saber está aqui. É simplesmente uma questão de otimizar seu tempo, (sites abaixo em inglês):

Add Me!

SiteAdd

URL Submitter

123 Add URL

Register

Submit It

Link recíproco
Link recíproco é uma troca. A idéia é buscar sites que tenham a ver com os seus e enviar um e-mail para eles pedindo para colocarem um link para seu site. Em troca, você oferece um link de volta aos sites deles no seu.

A melhor maneira de conseguir links recíprocos é navegar na Internet em busca de sites relacionados e enviar e-mails para eles. O índice de respostas é de cerca de 25%. Mas não custa tentar, e quanto mais links você tiver na Internet, mais tráfego você vai conseguir. Um link no lugar certo pode fazer uma GRANDE diferença no tráfego de um site novo.

A seguir um site que oferece recursos para criar links recíprocos (em inglês):

Link Exchange Index

Anúncio pago
Se você precisa de tráfego pra ontem, uma das melhores soluções é pagar para sites que têm bastante tráfego anunciarem seu serviço. Anúncios pagos geralmente aparecem como tiras finas, longas e piscantes no topo das páginas e são chamados de banners (mas há vários outros tipos de anúncios - veja Como funciona a publicidade na Internet para mais detalhes). Alguns exemplos de banners:







A maioria dos grandes sites, com tráfego em torno de 10 mil ou mais visitas por dia, têm programas-padrão de anúncios. O preço gira em torno de R$32 a R$150 por 1.000 apresentações do seu anúncio. O principal é você encontrar um site que direcione seus anúncios especificamente ao público que está interessado na sua mensagem.

Para mais informações sobre banners, confira Como funcionam os banners. Os links a seguir oferecem informações sobre programas de anúncios de algumas das maiores ferramentas de busca. A maioria das ferramentas de busca oferece algum tipo de propaganda - procure na homepage e você vai encontrar um link para informações sobre propaganda no site (em inglês):

Lycos Advertising

MSN Advertising

Yahoo! Web Launch

Yahoo! Advertising

Webcrawler Advertising

Mais informações sobre promoção de sites
Os artigos a seguir serão úteis para você aprender mais sobre promoção e marketing de sites (em inglês):

Web Digest for Marketers

NETrageous

Idéias
Se você encontrar uma página legal, dê uma espiada no código HTML para ver como ela foi feita, usando a ferramenta "Exibir código-fonte".  Esta é uma excelente maneira de aprender novas técnicas de HTML.

Se você quiser dar uma olhada em um conjunto de sites de visual bárbaro para tirar algumas idéias, visite a Affluent Lifestyles(em inglês). Esta página tem links para cerca de 100 sites - e muitos deles são fantásticos. Veja principalmente os sites dos fabricantes de jóias e das montadoras. Quando você encontrar um legal, dê uma espiada no código HTML.

Para muito mais informações sobre HTML, páginas de Internet e assuntos relacionados, confira os links na próxima página.
