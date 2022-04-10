Anotações de aprendizagem:
CSS:

* {
  margin: 0px;
  padding: 0px;
} - |reseta as configurações padrão do navegador|

html, body {
  min-height: 100vh; - |tamanho mínimo da altura corpo do site|
  background-color: dark;
}

header {
  background-color: black;
  color: white;
  text-align: center;  |centralizou o texto|
}

header > h1 {
  padding-top: 50px;
  font-variant: small-caps; |colocou as letras do H1 em maiúsculas, mas a 1ª letra de cada palavra ficou maior.|
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
}

section.normal {
  background-color: white;
  color: black;
}

section.imagem {
  background-color: rgba(51, 51, 51); |essa cor não vai aparecer quando a imagem for colocada.|
  color: white;
}

section.imagem {
  width: 400px; |criou uma caixa com uma cor transparente que facilitará a ler o texto quando a imagem for colocada.|
  background-color: rgba(0, 0, 0, 0.253);
}

footer {
  background-color: black;
  color: white;
  text-align: center;
  padding: 10px;
}
