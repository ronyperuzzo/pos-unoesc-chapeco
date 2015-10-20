</br></br>
#### Unoesc Chapecó
#### Pós-graduação em Desenvolvimento Web, Cloud e dispositivos móveis - WebMob
#### Disciplina: HTML5+CSS3
#### Professor: Jean Carlo Nascimento
#### Acadêmico(a): Rony Remus Peruzzo
### Artigo de revisão de CSS3

##### Funcionalidade: border-radius
##### O que é?
A propriedade CSS3 border-radius destina-se a definir bordas arredondadas. O arredondamento das bordas é feito com declaração de dois valores CSS de medida; o primeiro define o eixo horizontal (rx) de 1/4 de uma elipse e o segundo o eixo vertical (ry). O quarto de elipse assim definida é convenientemente inserida no canto vivo do box arredondando-o. O diagrama a seguir esclarece o esquema de arredondamento.
##### Onde usar:
Em qualquer elemento que possui o atributo border.
##### Como usar:
```css
seletor {border-radius:
[ <length> | <percentage> ]{1,4} [ / [ <length> | <percentage> ]{1,4} ]?);
}
```
##### Exemplo de uso
A sintaxe geral para aplicar borda arredondada é mostrada a seguir.

```css
seletor {
  border-top-left-radius: rx ry;
  border-top-right-radius: rx ry;
  border-bottom-right-radius: rx ry;
  border-bottom-left-radius: rx ry;
}

```
##### Referências:
[http://www.maujor.com/tutorial/interativo-css3/inc/borderradius.php](http://www.maujor.com/tutorial/interativo-css3/inc/borderradius.php)

</br></br>

##### Funcionalidade: Box shadow
##### O que é?
A propriedade CSS3 border-shadow destina-se a definir sombras em boxes ou qualquer tipo de elemento em sua página HTML usando apenas alguns códigos CSS.

##### Onde usar:
Em qualquer elemento que possui o atributo shadow.
##### Como usar:
```css
seletor { box-shadow: inset offsetX offsetY raioBlur spread cor; } 
```

##### Exemplo de uso
A sintaxe geral para aplicar as sombras é mostrada a seguir.

```html
<html>
<head>
  <title>Box-shadow em CSS3</title>
</head>
<body>
  <div id="sombra">
    <p>Esta é uma camada com sombra criada com CSS 3.</p>
  </div>
</body>
</html>
```
```css
#sombra{
  box-shadow: 5px 5px 0 #333;
  -webkit-box-shadow: 5px 5px 0 #333;
  -moz-box-shadow: 5px 5px 0 #333;
}
  
```
##### Referências:
[http://www.maujor.com/tutorial/interativo-css3/](http://www.maujor.com/tutorial/interativo-css3/)
[http://www.linhadecodigo.com.br/artigo/3633/entendendo-o-atributo-box-shadow-nas-css3.aspx#ixzz3p3qtCVP2](http://www.linhadecodigo.com.br/artigo/3633/entendendo-o-atributo-box-shadow-nas-css3.aspx#ixzz3p3qtCVP2)


</br></br>

##### Funcionalidade: Border-Image

##### O que é?
Utilizando o recurso border image do CSS3 é possível criar uma borda diferenciada utilizando imagem próprias. Com ele é possível então dar mais harmonia e personalidade ao seu layout.

##### Onde usar:
Em qualquer elemento que possui o atributo border.

##### Como usar:
Abaixo estão as finalidade de cada uma destas propriedades do border-image </br>
border-image-source </br>
  Define o endereço da imagem. </br>
border-image-slice </br>
  Define como a imagem será recortada para ser distribuída nas bordas. </br>
border-image-width </br>
  Define a espessura das bordas para inserção da imagem. </br>
border-image-outset </br>
  Define uma área externa à área da borda para onde a imagem será deslocada. </br>
border-image-repeat </br>
  Define como se dará a repetição da imagem. </br>
border-image </br>
  Declaração abreviada para as anteriores. </br>

A sintaxe geral para aplicar uma imagem na borda pode ser vista a seguir.
-moz-border-image: url("/imagens/borda.png) 15 15 15 15 / 15px 20px 30px 40px round stretch;

##### Exemplo de uso

```html
<html>
<head>
  <title>Box-shadow em CSS3</title>
</head>
<body>
 <div id="bordaimg">
    Vou colocar uma borda acima
 </div>
</body>
</html>
```
```css
#bordaimg{
  -moz-border-image: url(sello.png) 2 2 2 2 stretch stretch;
  -webkit-border-image: url(sello.png) 2 2 2 2 stretch stretch;
  padding:20px;
  width: 100px;
}
```
##### Referências:
[http://www.maujor.com/tutorial/css3-bordas-com-imagens.php](http://www.maujor.com/tutorial/css3-bordas-com-imagens.php)
</br>
[http://www.scriptcase.com.br/blog/border-image-no-css3/](http://www.scriptcase.com.br/blog/border-image-no-css3/)



##### Funcionalidade: Gradient

##### O que é?
É uma propriedade CSS que permite o preenchimento gradiente de um elemento.

##### Onde usar:
Em qualquer elemento que possui o atributo background.  

##### Como usar:
Palavras-chave definem a linha do gradiente conforme mostrado a seguir.

to right → transição de cores na horizontal da esquerda para a direita;
to left → transição de cores na horizontal da direita para a esquerda;
to top → transição de cores na vertical de baixo para cima;
to bottom → transição de cores na vertical de cima para baixo;
to top left → transição de cores a partir do canto superior esquerdo em direção ao centro;
to top right → transição de cores a partir do canto superior direito em direção ao centro;
to bottom left → transição de cores a partir do canto inferior esquerdo em direção ao centro;
to bottom right → transição de cores a partir do canto inferior direito em direção ao centro. 
EX: background-image: linear-gradient( to right, red, green, yellow, blue );

A utilização da propriedade pode variar de acordo com o navegador utilizado, segue alguns exemplos de sintax: </br>

Firefox 3.6+ </br>
  background-image: -moz-linear-gradient(green, red); </br>
Safari 5.1+, Chrome 10+ </br>
  background-image: -webkit-linear-gradient(green, red); </br>
Opera 11.10+ </br>
  background-image: -o-linear-gradient(green, red); </br>

##### Exemplo de uso

```html
<html>
<head>
  <title>Gradient</title>
</head>
<body>
 <div>
  Exemplo de gradiente   
 </div>
</body>
</html>
```
```css
div { 
  background-color: transparent;
  background-image:  linear-gradient( to right, red, transparent, blue ), url(../avatares/maujor82x82.jpg) center repeat-x; 
}
```
##### Referências:
[http://www.maujor.com/tutorial/css3-gradientes-lineares.php](http://www.maujor.com/tutorial/css3-gradientes-lineares.php)
</br>
[http://tableless.com.br/como-usar-gradient-no-css-de-forma-consciente/](http://tableless.com.br/como-usar-gradient-no-css-de-forma-consciente/)
[http://www.w3c.br/pub/Cursos/CursoCSS3/css-web.pdf](http://www.w3c.br/pub/Cursos/CursoCSS3/css-web.pdf)

</br></br>



##### Funcionalidade: Multiple Backgrounds

##### O que é?
É a funcionalidade que nos permite definir múltiplos backgrounds via CSS para um elemento.

##### Onde usar:
Em qualquer elemento que possui o atributo backgrounds.

##### Como usar:
A sintaxe é muito simples. Na verdade, é idêntica a sintaxe existente. Segue abaixo:

```css
div {
  width:600px;
  height:500px;
  border:1px solid black;
  background: url(gradiente-top.png) top left repeat-X,
              url(gradiente-baixo.png) bottom left repeat-X,
              url(gradiente-esquerda.png) top left repeat-Y,
              url(gradiente-direita.png) top right repeat-Y;
}
```

Veja que basta definirmos diversas vezes a propriedade URL com as imagens que escolher e pronto. Os atributos de posição e repetição continuam iguais!
É tão simples que dispensa grandes explicações. No exemplo acima usei 4 imagens em gradiente transparente. Duas para os lados e as outras duas para o topo e baixo.

##### Exemplo de uso

```html
<html lang="pt-br">
<head>
	<title></title>
	<meta charset="utf-8">
	</head>
<body>

<div>
	Um div.
</div>

</body>
</html>
```
```css
div {
		width:500px;
		height:500px;
		border:1px solid black;

		background-color:red;
		
		background: 
		url(gradiente-baixo.png) bottom right repeat-X,
		url(gradiente-esquerda.png) top left repeat-Y,
		url(gradiente-top.png) top right repeat-X,
		url(gradiente-direita.png) top right repeat-Y; 
	}
```
##### Referências:
[http://tableless.com.br/multiplos-backgrounds-com-css/](http://tableless.com.br/multiplos-backgrounds-com-css/)





















