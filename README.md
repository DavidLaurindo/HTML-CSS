# HTML
Estudos em HTML e CSS

Extensões VSCode:
Live Server(Abri um server local). Para ativar:(Crlt + Shift + P para abrir o terminal do VSCode e digitar: live server: open with server).

Todas as TAGs do HTML: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element

Validador: https://validator.w3.org/#validate_by_input

Box Model Resumido: https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model

Pseudo-classes: https://developer.mozilla.org/pt-BR/docs/Web/CSS/Pseudo-classes

Ctrl + Shift + i (formatar o documento HTML).

inline e block:
<p>parágrafo</p> é um block e só aceita tags do tipo inline.

## Tags
<p>Parágrafo</p>

<div></div> vem como display block com padrão.

<code>mostrar código</code>

<pre>mostra do mesmo jeito que esta escrito<pre> (usada também para mostrar código).

<style>Modificado CSS para pequenas formatações sem precisar de um css</style>

<h1 style="background: red;">cabeçalho</h1> (usa formatação css somente no h1).

<br>Quebra de linha (TAG sem corpo, não precisa fechar).

<hr>quebra de linha com um linha para dividir. (TAG sem corpo).

<q cite="link da citação">citação</q> (para adicionar texto com uma citação)

<blockquote cite="link da citação">citação<blockquote> (para usar fora de um <p>parágrafo</p>).

<b>Negrito</b>

<strong>Palavra destacada em negrito<strong> (tag com um acerta semântica. usada para dar força em alguma palavra).

<i>Itálico</i>

<em>ênfase</em> (igual o itálico mas a semantica é outra).

<s>risca a palavra</s> ( sem semântia. só para ter a palavra riscada fisicamente, sem lógica).

<del>risca a palavra<del> (semântica de algo que precisou ser apagado).

<ins>adiciona uma alinha em baixo da palavra</ins> (tag semântica, que algo foi adicionado no lugar de outra).

<u>adiciona uma linha em baixo da palavra</u> (sem semântica, somente físico).

<small>deixa o texto menor</small>

<sup>valor mais elevado</sup> (àquele número em cima no caso dos números elevados).

<sub>valor mais a baixo</sub> (ex: aquele 2 do H2O(ÁGUA) que fica mais em baixo).

<p><span style="color: red">alguma parte do texto</span></p> (span é inline e pode ser utilizado dentro de um block para modificar palavras). Também pode utilizar uma class="nome" para modificar somente ela no css. ex: <span classe="nome">palavra</span>

<headers>cabeçalho<headers>

<h1>Cabeçalho</h1> De h1 até h6

<a href="link">clique aqui</a> (gerar link).

<a href="link" target='_blank'>clique aqui</a> ('target'serve para expecificar se vai abrir outra aba, manter na mesma etc. VER LINK).
https://developers.google.com/search/docs/advanced/appearance/qualify-outbound-links?hl=pt-br

<img src="link da imagem" alt="descrição da imagem"> (caso o site so tenha uma imagem).

<img class="nome-da-imagem" src="link da imagem" alt="descrição da imagem"> (adicionado uma classe para sites com várias imagens). Também pode colocar um aimagem dentro de um href para ao clicar na imagem ir para o link.

## Atributos
id (h1 id="identificador-unico") - não pode repetir o id.
chamada no css: #identificador-unico {}

Classe (h1 id="identificador-unico" class="identificador") - pode repetir a classe como também pode usar junto com id caso precise. Também pode usar mais de uma classe ex: (class="borda-1 borda-2").
chamada no css: .identificador {}

### Listas:

li*4(cria 4 itens automaticamente).
li*quantas linhas da tabela.

<ul>Lista não ordenada</ul>
<ol>Lista ordenada</ol>
<li>itens de lista</li>

<dl>Lista com descrição</dl>
<dt>Itens</dt>
<dd>descrição do item</dd>

<ul>
  <li>item 01</li>
  <li>item 02</li>
  <li>item 03</li>
</ul>

<ol>
  <li>item 01</li>
  <li>item 02</li>
  <li>item 03</li>
</ol>
<ol type="A"></ol> (muda de números ordenados para A, B, C...)

<dl>
  <dt>café</dt>
  <dd>bebida preta quente</dd>
  <dt>Cerveja</dt>
  <dd>bebida alcolica</dd>
</dl>

### Tabelas:

<table>Tabelas</table>

<table>
  <thead>
    <tr>
      <th>Título 1</th>
    </tr>
  </thead>
</table>

## Formulários:

Links para estruturação de formulários e todos os tipos de INPUTS:
https://www.w3schools.com/html/html_form_input_types.asp

https://developer.mozilla.org/pt-BR/docs/Learn/Forms/How_to_structure_a_web_form

<form>Formulário</form>
O elemento <form> é o elemento que formalmente define o formulário e os atributos que definem a maneira como esse formulário se comporta. Sempre que você desejar criar um formulário HTML, você deve iniciá-lo usando este elemento, colocando todo o conteúdo dentro deste. Muitas tecnologias assistivas ou plugins de navegadores são capazes de descobrir elemetos <form> e de implementar ganchos especiais para torná-los mais fáceis de usar.

Nota: É estritamente proíbido aninhar um formulário dentro de outro formulário. Isto pode fazer com que os formulários se comportem de maneira imprevisível baseada no navegador que está sendo utilizado.

<form action="#" method="get" target="_blanck" autocomplete="off">

</form>
(autocomplete="off" usado para nao aparecer histórico do que foi escrito no formulário).
(target="_blank" para ele enviar o formulário para outra página. obs: para facilitar o entendimento no curso).

<input type="text" id="nome-campo" name="nome" placeholder="Seu nome" desabled/readonly requered> (não precisa fechar).
(name="" vai ser usado no back-end)
(placeholder="seu nome" vai aparecer como exemplo no formulário).
(desabled para desabilitar o input).
(readonly somente leitura do placeholder e mantem desabilitado o input).
(requered obriga o usuário a marcar ou responder o input).

<button type="submit">Enviar</button> (enviar formulário).
<button type="reset">Reset</button> (resetar formulário).

<input type="checkbox" id="dev" name="dev" value="sim" checked>
(values="sim" valor a ser enviado para back-end).
(checked já deixa a checkbox marcada por padrão).

                <p>
                    Gênero:<br>
                    <label for="feminino">feminino</label>  
                    <input type="radio" id="feminino" name="genero" value="feminino"><br>
                    <label for="dev">masculino</label>  
                    <input type="radio" id="masculino" name="genero" value="masculino"><br>
                    <label for="outro">outro</label>  
                    <input type="radio" id="outro" name="genero" value="outro"><br>
                </p> (utilizando radio)
                
<p>
  <label for="file">Sua Foto:</label>  
  <input type="file" id="file" name="file"
   accept=".png, .svg, image/*" multiple> (accept="" arquivos que irá aceitar).
   (multiple quer dizer que vai aceitar vários arquivos).
</p>                

 <p>
   <label for="number">Number:</label>  
   <input type="number" id="number" name="number" placeholder="Number"    min="10" max="50" step="5">
</p>   
(min e max correspondem ao máximo permitido de números)
(step é qm quantos e quantos números irá andar).            
                _________________________________________________
# CSS

link CSS: <link rel="stylesheet" href="./assets/css/style.css">

Unidades de medida: https://www.w3schools.com/cssref/css_units.asp

elemento floate vai usar somente o espaço dele e liberar os demais espaços.

----------------------------------------------------------------------------

Width e height para o conteúdo
box-sizing: border-box: o conteúdo estará ligado com padding e border.

display: inline; não pega certos atributos ex: width, height.

overflow: hidden;(ex: impede que o texto saia do conteúdo)
overflow: scroll;(cria uma barra de rolar para mostrar os conteúdos que nao couberam. Sempre irá criar a barra, mesmo o conteúdo estando ok)
overflow: auto; (quando o conteúdo passar vai criar uma barra automaticamente)

(width e heidth controlam o conteúdo. estão dentro do padding)
width: 100%;
max-width: 600px; (o máximo)
min-width: 0%; (o tamanho)
    
height: 100%;
max-height: 100%;
min-width: 0%;

margin: 0 auto;

overflow-y:  auto;

----------------------------------------------------------------------------
pode selecionar mais de uma tag por seleção:
h1, p{
  font-samily: #
}

*{
    margin: 0;
    padding: 0;
}

border(tamanho, cor e estilo da borda) ex: border: 15px solid black;

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

Remover sublinhado de link:
 text-decoration: none;

Fonte de todos os sistemas operacionais:
 font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;

#### Alguns seletores de atributo:
 .pai h1+p{
    color: red;
}(Adjacent sibling select. usar o + para selecionar"!ver a documentação")
(seleciona o <p> que vem logo depois do h1).

.pai h1~p{
    color: red;
}(gerenal sibling select).
(Seleciona todos os <p> que vem depois do h1)
---------------------------------------------------------------
fade in out no :hover
.heading{
    transition: all 600ms ease-in-out;
}
.heading:hover{
    background: blue;
}(pequena animação)
------------------------------------------------------------
p:not(.meio){
    color: blue;
}(negação, todos os <p> do html menos o que estiver a classe .meio).
Link: https://developer.mozilla.org/pt-BR/docs/Web/CSS/:not

---------------------------------------------------------------------------
ul li:nth-child(even){/*seleciona somente filhos pares*/
    background-color: chartreuse;
}
ul li:nth-child(odd){/*seleciona todos os ímpares*/
    background-color: crimson;
}
ul li:nth-child(3n){/*vai acionar a cada 3 filhos*/
    background-color: darkmagenta;
}
ul li:nth-child(3n+5){/*a partir do quinto filho vai começar a contagem de 3 em 3*/
    background-color: darksalmon;
}

nth-child()
link: https://developer.mozilla.org/pt-BR/docs/Web/CSS/:nth-child
--------------------------------------------------------------------------
Pseudo-elementos
link:https://developer.mozilla.org/pt-BR/docs/Web/CSS/Pseudo-elements

----------------------------------------------------------------------------
### Especificidade

Prioridades:
1: ID
2: CLASSES, ATRIBUTOS E PSEUDO-CLASSES
3: ELEMENTOS E PSEUDO-ELEMENTOS

links:
https://developer.mozilla.org/pt-BR/docs/Web/CSS/Specificity

https://www.w3.org/TR/selectors-3/#specificity

https://specificity.keegan.st/

----------------------------------------------------------------------------

p{
  font-size: inherit; (Para herdar os atributos)
  color: initial; (para não herdar)
}

-------------------------------------------------------------------------------
### Texto

p{
  font-size: 20px (tamanho da fonte)
  font-style: italic; (estilo da fonte)
  fonte-weight: bold;
  direction: ltr;(direção do texto)
  letter-spacing: 2px; (espaço entre as letras)
  world-spacing: 10px; (espaço entre as palavras)
  line-height: 25px; (altura da linha)
  text-align: left; (alinhamento do texto)
  text-decoration: overline (decoração do texto)
  text-indent: 50px; (espaços nos parágrafos auomaticamente)
  text-shadow: 2px 2px 2px(esfumaçado) red; (sombra no texto)
}

propriedades de texto: https://www.w3schools.com/css/css_text.asp

-------------------------------------------------------------------------------
z-index: 1 (conteúdo vai ficar por cima)
z-index: 2 (conteúdo vai ficar por baixo)
z-index: -1 (leva o conteúdo para traz de todos os elementos)

-------------------------------------------------------------------------------
## @media

link: https://developer.mozilla.org/pt-BR/docs/Web/CSS/Media_Queries/Using_media_queries

link: https://www.w3schools.com/cssref/css3_pr_mediaquery.asp

link: https://devfacts.com/media-queries-breakpoints-2021/

-------------------------------------------------------------------------------
 
 scroll-behavior: smooth; (usa-se no CSS para a página ir descendo com animação).

 ------------------------------------------------------------------------------

 ### Borda arredondada

 border-top-left-radius: 150px;
 border-radius: 150px (mesma borda com atalho)
 ex: border-radius 100px 100px 100px 100px(cima direita baixo e esquerdo)

 border-radius: 50%; (cria um círculo)

 ### sombras no elemento

 box-shadow: 0 0 0 0 blue;
 ex: box-shadow: -10px 10px 0 0 cor;

## Flex-box

link: https://developer.mozilla.org/pt-BR/docs/Learn/CSS/CSS_layout/Flexbox#um_aparte_no_modelo_flex

justify-content: ; está mechendo com o eixo principal

assistir flexbox no curso javaScript

display: flex;
flex-direction: row;
justify-content: space-between;
flex-wrap: wrap;
align-item: center;
align-content: center;
background: yellow;
height: 10px;

