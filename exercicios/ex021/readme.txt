TIPOS DE CAIXAS

- BOX BLOCK LEVEL:  Esse tipo de caixa sempre se inicia em uma nova linha e vai ocupar a largura total da tela ou <section> na qual foi inserida independente do tamanho do seu conteúdo. 

Um exemplo de tag box level é <h1 - h6> </h1 - /h6> onde um novo parágrafo é iniciado em uma nova linha e ocupará toda a largura disponível no local em que foi inserido.


- BOX INLINE LEVEL - Esse tipo de caixa sempre se inicia a partido do ponto em que sua tag é chamada independente do local onde foi iniciada, sempre ocupará apenas o tamanho de seu conteúdo e só ficará maior caso seja estipulado via CSS.

Um exemplo de tag inline level é <a> </a> onde o tamnho da sua box dependerá apenas do tamnho das informações adicionadas no interior da tag.




COMANDOS CSS

- margin: auto; - utilizada para centralizar caixas horizontalmente.

- outline-width: (x)px; - determina uma linha de (x)px de larura entre a margin e a borda do conteúdo.  Lembrando que o valor definido para o outline será descontado do valor da margin.

margin-width: 30px;
outline-width: 10px;

nesse caso o resultado final teremos uma margin com 20px e uma outline com 10px.

*** Lembramos que outline não é utilizado com tanta frequência.




SHORTHANDS

Para os seletores margin, outline e border podemos utilizar shorthands em suas funções mais utilizadas. Segue a ordem que devemos respeitar:

largura 
estilo
cor

border: 10px solida green;

margin: 25px dotted blue;

outline: 2px dashed white;


Outra forma de aplicação:

margin: 10px auto 10px auto; 

No caso acima as margens direita e esquerda ficaram com seus valores em automatico isso centralizaria o box horizontalmente.




FUNÇÃO INLINE

Vamos supor que estamos usando uma tag que por natureza é do tipo box level mas não desejamos que a mesma ocupe toda a largura da <section>, utilizando CSS podemos denominar essa tag em questão como inline block.

Exemplo:

<h1> Exemplo de título</h1>


<style> 
 h1{
    display: inline;
 }
</style>

A partir desse momento a tag <h1> deixou de ser do tipo block level e se tornou inline level, com isso passa a ocupar somente o tamanho de seu conteúdo tendo seu comportamento similar a de qualquer outra tag do tipo inline level.





FUNÇÃO BLOCK

Assim como no exemplo acima agora temos o caso oposto onde estamos utilizando uma tag do tipo inline level e desejamos que a mesma se comporto como um block level.

Exemplo:

<a href="#">links são exemplos de caixas inline-level</a>


<style> 
 a{
    display: block;
 }
</style>

A partir desse momento a tag <a> se comportará como um block level e ocupará toda a largura da <section> disponível ou o valor de altura e largura definidos nas CSS.