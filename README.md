# jogo-da-velha

Entrando no JavaScript

<<<<<<< HEAD
**Game** - Representação das posições
=======
# **_Game_** Representação das posições
>>>>>>> 452ecf51b2fcd97fc7b6521806b46624bf95e985

Representando o tabuleiro no JS:
Dentre os 9 quadrados, nós  teremos 3 opções de status, sendo elas o X, O ou vazio (padrão), portanto foi criada uma array representando cada quadrado.

PlayerTime: 
Como o nome já diz, a variável PlayerTime foi criada para gerir a vez do jogador, tendo como 0 ou 1.

Symbols: 
Após a verificação de quem é o jogador da vez, o symbols representará no board o X ou O.

HandleMove (representação de um movimento do jogador):
Lá no game.js criei a função handleMove com position como argumento. 
Executanto ficará como ao realizar o movimento, a posição do board escolhida será o symbols com o indice de playerTime. 
Dentro do handleMove existe um if pronto para alterar o playerTime, portanto sempre que um jogador jogar, automaticamente a vez irá para o outro jogador, portanto o symbols será diferente para cada jogada.

<<<<<<< HEAD
**Interface** - Reagir eventos do usuário
=======
# **_Interface_** Reagir eventos do usuário
>>>>>>> 452ecf51b2fcd97fc7b6521806b46624bf95e985

Representamos através do evento onLoad uma função que receberá todo o processo do game.

Primeira ação que tomamos é passar os elementos de classe .square (quadrados) para o js, ao passarmos para o JS, o .square virá em formato de array de 9 indices. 

Aplicamos o forEach na array squares uma função chamada de handleClick com o evento de 'click'. 

obs: Por via de testes, passamos o argumento 'evente' e executamos na função o console.log(event.target), isto fará com que apareça no console o elemento em que eu cliquei.

A função handleClick terá ações tanto na inferface.js quanto no game.js. O event.target se trasformará em uma variável chamada square, no square nós transformamos em mais uma variável o seu ID.
Após termos o ID, executamos a função handleMove que foi criada na parte do game.

Dentro do handleClick também terá a função updateSquares() que tem como objetivo pegar a posição do meu clique e passar para a variável symbol, após isso utilizamos o if para confirmar se o symbol é diferente de vazio, caso seja ele alterará o inner.html do square e passará a nova classe[symbol] que será X ou O.

![img1](https://user-images.githubusercontent.com/83314555/156480415-13d284af-1d21-4094-9230-3efc3933017b.png)

**Verificação do vencedor**

