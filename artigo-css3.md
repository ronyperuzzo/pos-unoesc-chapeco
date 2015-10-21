#### Unoesc Chapecó
#### Pós-graduação em Desenvolvimento Web, Cloud e dispositivos móveis - WebMob
#### Disciplina: HTML5+CSS3
#### Professor: Jean Carlo Nascimento
#### Acadêmico(a): Rony Remus Peruzzo
### Artigo de revisão de CSS3

##### Funcionalidade: (1) Box-shadow

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
[http://www.maujor.com/tutorial/interativo-css3/](http://www.maujor.com/tutorial/interativo-css3/)</br>
[http://www.linhadecodigo.com.br/artigo/3633/entendendo-o-atributo-box-shadow-nas-css3.aspx#ixzz3p3qtCVP2](http://www.linhadecodigo.com.br/artigo/3633/entendendo-o-atributo-box-shadow-nas-css3.aspx#ixzz3p3qtCVP2)

</br></br>

##### Funcionalidade: (2) Border-Image

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
  <title>Border-Image em CSS3</title>
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

</br></br>

##### Funcionalidade: (3) border-radius

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

##### Funcionalidade: (4) Gradient

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
[http://tableless.com.br/como-usar-gradient-no-css-de-forma-consciente/](http://tableless.com.br/como-usar-gradient-no-css-de-forma-consciente/) </br>
[http://www.w3c.br/pub/Cursos/CursoCSS3/css-web.pdf](http://www.w3c.br/pub/Cursos/CursoCSS3/css-web.pdf)

</br></br>

##### Funcionalidade: (5) Multiple Backgrounds

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
   <title>Background Multiplos</title>
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
[http://tableless.com.br/multiplos-backgrounds-com-css/](http://tableless.com.br/multiplos-backgrounds-com-css/) </br>

</br></br>

##### Funcionalidade: (6) Pointer Events

##### O que é?
A propriedade pointer-events permite controlar sob qualquer circustancia um elemento gráfico particular podendo ser o alvo do evento do mouse. Quando essa propriedade não é especificada, as mesmas características do valor visiblePainted é aplicada no conteúdo SVG.
Além de indicar que este elemento não é o alvo do evento do mouse, o valor none instrui o evento do mouse a "passar" o elemento e tudo que está "abaixo" deste elemento.

##### Onde usar:
Em elementos onde você deseja controlar as funções ou eventos do mouse.

##### Como usar:
A sintax formal: 
	auto | none | visiblePainted | visibleFill | visibleStroke | visible | painted | fill | stroke | all | inherit
```css
	pointer-events: auto;
	pointer-events: none;
	pointer-events: visiblePainted;
	pointer-events: visibleFill;
	pointer-events: visibleStroke;
	pointer-events: visible;
	pointer-events: painted;
	pointer-events: fill;
	pointer-events: stroke;
	pointer-events: all;
	pointer-events: inherit;
```

##### Exemplo de uso

```html
<html lang="pt-br">
<head>
   <title>Pointer Events</title>
   <meta charset="utf-8">
</head>
<body>
 	<ul>
  	<li><a href="https://developer.mozilla.org">MDN</a></li>
  	<li><a href="http://example.com">example.com</a></li>
	</ul>
</body>
</html>
```
```css
a[href="http://example.com"] {
  pointer-events: none;
}
```

##### Referências:
[https://developer.mozilla.org/pt-BR/docs/Web/CSS/pointer-events/](https://developer.mozilla.org/pt-BR/docs/Web/CSS/pointer-events/) </br>

</br> </br>

##### Funcionalidade: (7) Animations

##### O que é?
CSS Animation manipula características dos elementos, transformando-os modificando por meio de transições os valores das propriedades definidas dos elementos.

##### Onde usar:
Em princípio pode ser utilizado em qualquer elemento css.

##### Como usar:
CSS Animation permite que modifiquemos propriedades do CSS e tenhamos o resultado ali, na hora.
Para isso, usaremos uma propriedade chamada transition. Essa propriedade é divida em 3 propriedades: transition-property que é a propriedade que deverá ser animada, transition-duration é quanto tempo a transição irá durar, e transition-timing-function é o tipo de transição.

##### Exemplo de uso	

```html
<html lang="pt-br">
<head>
   <title>CSS Animation</title>
   <meta charset="utf-8">
</head>
<body>
	<div class="div1">
		<p>Testando css animations!</p>
	</div>
</body>
</html>
```
```css
	.div1 {
		border: 10px solid black;
		width: 250px;
		height:250px;
		background:lightgray;
		-webkit-transform: rotate(0deg);
	  -webkit-transition: background 1s linear, -webkit-transform 0.5s linear;
	}
		
	.div1:hover {
		background: red;
		width: 250px;
		-webkit-transform: rotate(-360deg);
	}
		
```
##### Referências:
[http://tableless.com.br/introducao-ao-css-animation/] (http://tableless.com.br/introducao-ao-css-animation/) </br>

</br> </br>

##### Funcionalidade: (8) font-face

##### O que é?
O font-face é uma das funcionalidades que foram mais aguardadas. Ela permite que você utilize famílias de fonts fora do padrão do sistema. 

##### Onde usar:
Pode ser utilizada em qualquer elemento que tenha a opção de definição de fonte. 

##### Como usar:
A diretiva @font-face adota uma sintaxe semelhante à sintaxe da regra CSS, contudo a terminologia difere. A especificação da diretiva nomeia o par descriptor: value (descritivo: valor) e não property: value (propriedade: valor) como nas CSS.
Assim, a sintaxe geral e sua terminologia é:

```css
@font-face {
	descritivo: valor;
	descritivo: valor;
	...
	}
```
Na primeira linha você define um nome para a font importada.
Na segunda linha, você inclue o endereço de onde a font se encontra.

##### Exemplo de uso	

```html
<html lang="pt-br">
<head>
   <title>CSS font-face</title>
   <meta charset="utf-8">
</head>
<body>
	<div class="div1">
		<p>Testando css font-face!</p>
	</div>
</body>
</html>
```
```css
@font-face {
	font-family: "RegencyScriptFLF Regular";
	src: url("http://site/fontes/RegencyScriptFLF-Regular.eot"); /* para IE */
	src: url("http://site/fontes/RegencyScriptFLF-Regular.ttf");
}

p { 
	font-family: "RegencyScriptFLF Regular", Cursive; 
}
```
##### Referências:
[http://tableless.com.br/font-face-fonts-externas-na-web/] (http://tableless.com.br/font-face-fonts-externas-na-web/) </br>
[http://www.maujor.com/tutorial/transparencia.php] (http://www.maujor.com/tutorial/transparencia.php)

</br></br>

##### Funcionalidade: (9) Flexbox

##### O que é?
Flexbox, ou Flexible Box Layout, é um novo modo de layout em CSS3, projetado para leiautar aplicações complexas e páginas web.
Flexbox é similar ao layout em bloco (block), exceto que ele não tem muitas das propriedades que podem ser usadas num layout em bloco, como floats e columns. Flexbox também é mais flexível por distribuir espaço e alinhar conteúdo em formas que aplicações web e páginas web complexas geralmente precisam. Isso resolve diversos outros problemas de layout que desenvolvedores front-end temos lutado e tentando resolver ao longo dos anos — como centralização vertical, por exemplo, dentro muitos outros.

##### Onde usar:
Pode ser utilizada em qualquer página que utilize css3.

##### Como usar:
O Flexbox possui uma série de propriedades abaixo citadas. Essas proriedades devem ser incluídas no style do componente.
flex-direction
flex-wrap
flex-flow
justify-content
align-items
align-content
order
align-self
flex-grow
flex-shrink
flex-basis
flex

```css
.container {
  display: -webkit-flex;
  display: flex;
}
```

##### Exemplo de uso	

```html
<html lang="pt-br">
<head>
   <title>CSS font-face</title>
   <meta charset="utf-8">
</head>
<body>
<input type="radio" name="flex-direction" id="row" checked 
	onclick="var container=document.getElementById('container'); 
               container.style.WebkitFlexDirection = 'row'; 
               container.style.flexDirection = 'row';" >
  <label for="row">flex-direction: row;</label>
  
  <br>
  
  <input type="radio" name="flex-direction" id="row-reverse" 
  	onclick="var container=document.getElementById('container'); 
                 container.style.WebkitFlexDirection = 'row-reverse'; 
                 container.style.flexDirection = 'row-reverse';" >

	<div class="container" id="container" >
	  <div class="item">1</div>
	  <div class="item">2</div>
	  <div class="item">3</div>
	  <div class="item">4</div>
	  <div class="item">5</div>
	</div>
</body>
</html>
```
```css
.container {
    margin: 150px auto;
    max-width: 800px;
    padding: 20px;
    -webkit-display: -webkit-box;
    -webkit-display: -webkit-flex;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    background-color: #594255;
}
```
##### Referências:
[http://desenvolvimentoparaweb.com/css/flexbox/#section_flex-direction] (http://desenvolvimentoparaweb.com/css/flexbox/#section_flex-direction) </br>
[http://tableless.com.br/flexbox-organizando-seu-layout/] (http://tableless.com.br/flexbox-organizando-seu-layout/)

</br></br>

##### Funcionalidade: (10) RGBA

##### O que é?
A declaração de cores com uso de RGB (red, green, blue) está prevista na atual versão das CSS e nós desenvolvedores já estamos usando-a há algum tempo, pois é bem suportada pelos navegadores atuais. 
O Módulo CSS3 para Cores estendeu o uso de RGB criando RGBA (red, green, blue, alpha-opacity) acresentando mais um argumento na declaração da cor, que permite definir a opacidade em uma escala decimal de 0 a 1. Os valores RGB podem ser declarados em escala numérica de 0 a 255 ou percentual de 0 a 100%.

##### Onde usar:
Em qualquer elemento que tenha a possibilidade de alteração da cor tais como background-color e color.


##### Como usar:
Syntax básica: rgba(r, g, b, a);
```css
#exemplo {
	background:rgba(255,100,60,0.4);
}
```

##### Exemplo de uso	
```html
<html lang="pt-br">
<head>
   <title>CSS font-face</title>
   <meta charset="utf-8">
</head>
<body>
	<div class="exemplo" >
	  	<p> Testando RGBA </p>
	</div>
</body>
</html>
```
```css
div.exemplo { 
  width: 300px;
  height: 150px;
  border: 2px solid black;
  background: rgba(0, 0, 0, 0.5); 
  }
```
##### Referências:
[http://www.maujor.com/tutorial/css3-modulo-para-cores.php] (http://www.maujor.com/tutorial/css3-modulo-para-cores.php)
