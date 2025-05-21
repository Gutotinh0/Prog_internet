aula passada: (box models, block (uma tag que ocupatodo o espaço da tag), inline, display ( ela segue na mesma linha))




-SPAN TEXTO GENERICO

texto direto no body

#<a href="/">Texto no link</a></a>#

<span>Texto na div</span>

<div>Texto na div</div>

texto direto no body 2

<a href="/">texto no link 2</a>

<span>texto no span 2</span>


-Ao modificar o modo de escrita, o fluxo também é modificado.

body {
    writing-mode: vertical-lr;
}

display inline e block

Define como a caixa ( box model) ira se comportar

* inline
Respeita o fluco da escrita sem iniciar uma nova linha, não é possivel definir valores de 
width, height, margin (top/bottom) e etc. é o estilo padrão.

*block
Inicia uma nova linha e não permite que outros elementos sejam posicionados em sua linha. aceita todas as propriedades do box model. estilo inicial de estilos como h1, p, div e outros.


-----
pegadinha aula

"HTML""
<div class="esconde">
</div>

<div>
 Acesso o meu <a href="/" class="inlineblock">link    """ porque esta junto?: porque se estiver um espaço ele teria duas classes (EX: Inline #1 Block #2) """
 inline-block</a> aqui.
 </div>

 <div>Novo elemento de block</div>

 <div>
 Acesse o meu <a href="/"> link inline</a> aqui.
 </div>

 <div>Novo Elemento de bloco</div>

 "CSS"

 .inlineblock {
    display: inline-block;
 }

 .esconde {
    display: none;
 }

 .divdesign {
    margin-bottom: 30px;
 }

tipos {top, right, left e bottom}

-pra colocar uma classe no css vc coloca um . e o nome ca classe 

*None 
Remove o elemento completamente da tela.

*inline-block (poderia usar no header setando o tamanho com "width")
fabricio: deixar alinhados e respeitando o tamanho que les ocupam
aula: o elemento continua inline


-----
posicionamento: para posicionarmos complexos, como o da imagem abaixo. utilizamos as propriedades display grid (cs grid layout) e flex
