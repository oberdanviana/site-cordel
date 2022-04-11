Anotações de aprendizagem:
CSS:

@import url('https://fonts.googleapis.com/css2?family=Passion+One&display=swap');

@import url('https://fonts.googleapis.com/css2?family=Sriracha&display=swap');

:root {
  --fonte1: Verdana, Geneva, Tahoma, sans-serif;
  --fonte2: font-family: 'Passion One', cursive;
  --fonte3: 'Sriracha', cursive;
}

* {
  margin: 0px;
  padding: 0px;
  font-size: 1em; |tamanho padrão da fonte.|
} - |reseta as configurações padrão do navegador|

html, body {
  min-height: 100vh; - |tamanho mínimo da altura corpo do site|
  background-color: dark;
  font-family: var(--fonte1);
}

header {
  background-color: black;
  color: white;
  text-align: center;  |centralizou o texto|
}

header > h1 {
  padding-top: 50px;
  font-variant: small-caps; |colocou as letras do H1 em maiúsculas, mas a 1ª letra de cada palavra ficou maior.|
  font-family: var(--fonte2);
  font-size: 7vw; |tamanho da fonte 6% da lagura da tela, essa é uma das formas de manter o tamanho da fonte responsivo.|
}

header > p {
  padding-bottom: 50px; |deixou o texto centralizado, essa ação foi em conjunto com padding-top do h1.|
}

header a, footer a {
  color: white;
  text-decoration: none;
  font-weight: bolder; |deixou o link em negrito.|
}

header a:hover, footer a:hover {
  text-decoration: underline;
} |quando passar o mouse em cima o texto do link fica sublinhado.|

section {
  padding-top: 10vh;
  padding-bottom: 10vh; |colocou um padding de 10% da vh em cima e em baixo para facilitar o efeito paralaxe.|
  line-height: 2em; |colocou um espaçamento duplo entre as linhas do texto.|
  padding-left: 30px; |separou o texto do canto esquerdo da tela.|
  font-family: var(--fonte3);
  font-size: 3.5vw;
}

section.normal {
  background-color: white;
  color: black;
}

section.imagem {
  background-color: rgba(51, 51, 51); |essa cor não vai aparecer quando a imagem for colocada.|
  color: white;
}

section.imagem > p{
  display: inline-block; |com display inline-block essa section se transforma em uma caixa que se adapta ao tamanho do conteúdo.|
  padding: 5px;
  background-color: rgba(0, 0, 0, 0.253);
}

footer {
  background-color: black;
  color: white;
  text-align: center;
  padding: 10px;
}
