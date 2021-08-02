# HTML-CSS
Estudos em HTML e CSS

Extensões VSCode:
Live Server(Abri um server local). Para ativar:(Crlt + Shift + P para abrir o terminal do VSCode e digitar: live server: open with server).

Todas as TAGs do HTML: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element

Validador: https://validator.w3.org/#validate_by_input

Ctrl + Shift + i (formatar o documento HTML).

inline e block:
<p>parágrafo</p> é um block e só aceita tags do tipo inline.

## Tags
<p>Parágrafo</p>

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
